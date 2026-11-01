---
aliases:
- kplexAPI examples
- window.kplexApi
- Query relationships with JavaScript
tags:
- kplex-help/reference
- kplex/automation
Guide:
- '[[12 Automation/Automation and scripting]]'
Friend:
- '[[12 Automation/Use K-Plex through Obsidian CLI]]'
- '[[03 Build and edit/Connection details and evidence]]'
Related:
- https://github.com/zsviczian/kplex/blob/main/docs/PUBLIC_API.md
---
# K-Plex API examples

Find a research topic, inspect its relationships, or hand a map's context to a script. These examples use the public API inside Obsidian: run each complete block in the developer console, or pass it as JavaScript to Obsidian CLI `eval`.

The entry point is **`window.kplexApi.v1`**, not `window.kplexAPI`. Read methods return `{ok, value, revision, coverage, truncated}` on success and `{ok: false, error, revision}` on failure. Actions return promises. The examples use independent scopes so you can run them more than once.

## Learn the vocabulary before suggesting a relationship

```js
(() => {
  const api = window.kplexApi?.v1;
  if (!api) throw new Error('Enable K-Plex to use API v1');
  return {
    capabilities: api.capabilities(),
    status: api.status(),
    guide: api.ontologyGuide({format: 'markdown'}),
  };
})()
```

In this vault, the guide explains fields such as **Guide**, **Explains** and **Related**, their roles and inverse partners. Your own vault supplies its own vocabulary. An absent description means no meaning has been authored; a script should not invent one. Configured ontology is readable before the graph finishes preparing.

## Find a topic and inspect its neighbors

```js
(() => {
  const api = window.kplexApi?.v1;
  if (!api) throw new Error('Enable K-Plex to use API v1');
  const matches = api.search({query: 'Workshop plan', limit: 10});
  if (!matches.ok) return {matches};
  // Review the matches when adapting this to your own vault.
  const topic = matches.value.items.find(
    item => item.path === '09 Showcase examples/Example - Workshop plan.md'
  );
  if (!topic) return {matches, message: 'The example is not in these results'};
  return {
    matches,
    neighbors: api.neighbors({id: topic.id, role: 'child', limit: 20}),
  };
})()
```

Use the returned `id` exactly; it is case-sensitive and need not be a path. Navigation uses a separate physical file path. API roles are `parent`, `child`, `left` (Friend), `right` (Challenger), `previous` and `next`.

Check `coverage` and `truncated` on **both** results. Reads inspect already published facts and do not fetch missing sources. `requireComplete: true` rejects incomplete or truncated reads with `INDEX_INCOMPLETE`; it does not make them complete. Normal graph result limits default to 40 and allow at most 200. Larger requests can still be limited by work and output budgets.

## Ask why two notes connect

```js
(() => {
  const api = window.kplexApi?.v1;
  if (!api) throw new Error('Enable K-Plex to use API v1');
  const matches = api.search({query: 'Workshop plan', limit: 10});
  if (!matches.ok) return {matches};
  const topic = matches.value.items.find(
    item => item.path === '09 Showcase examples/Example - Workshop plan.md'
  );
  if (!topic) return {matches};
  const neighbors = api.neighbors({id: topic.id, role: 'child', limit: 20});
  if (!neighbors.ok || !neighbors.value.items.length) return {matches, neighbors};
  const connection = neighbors.value.items[0];
  return {
    matches,
    neighbors,
    evidence: api.evidence({
      sourceId: connection.sourceId,
      targetId: connection.targetId,
      limit: 128,
    }),
  };
})()
```

Evidence identifies the owning note, physical field or source location, active decisions and overridden contributions. It does not return note bodies or authorize deleting a source. Compare the result with [[03 Build and edit/Connection details and evidence|Connection details]] when investigating an unexpected direction.

## Describe one open canvas

First run this to list open canvases and choose the intended `id`:

```js
window.kplexApi.v1.canvases()
```

Then replace `RETURNED_CANVAS_ID` below with that exact value:

```js
(() => {
  const api = window.kplexApi.v1;
  const canvasId = 'RETURNED_CANVAS_ID';
  return {
    snapshot: api.canvas({canvasId}),
    context: api.context({canvasId}),
  };
})()
```

Canvas context is Markdown describing the map, not a note-body export. The snapshot distinguishes canonical `nodeId` values from visual occurrence `id` values. The same note can have several occurrences. `included` and `inViewport` are separate: an offscreen note is not necessarily filtered out.

Canvas IDs expire when a canvas closes or the plugin reloads. Multiple canvases require an explicit choice; omission returns `AMBIGUOUS_CANVAS`. Reacquire the API after a reload, too.

## Navigate a chosen canvas, then check it

This changes the selected canvas's center. Replace the canvas ID and use an existing physical file in your vault.

```js
(async () => {
  const api = window.kplexApi.v1;
  const canvasId = 'RETURNED_CANVAS_ID';
  const action = await api.navigate({
    canvasId,
    path: '09 Showcase examples/Example - Workshop plan.md',
  });
  return {action, snapshot: api.canvas({canvasId})};
})()
```

An `accepted` receipt can precede the finished transition. A `completed` receipt observes the requested metadata, not finished animation. Re-read the snapshot until the intended `canvas.attention`/`canvas.root` and view are present and `scenePending` is false; check `motionPending` when camera settling matters. Use a bounded wait and report a pending result rather than retrying navigation repeatedly.

To choose a view, await `api.selectView({canvasId, viewId: 'mindmap'})`. The built-in IDs are `classic` (Compass), `mindmap` and `wuxing` (Facets). Use `api.selectPreset({canvasId, presetId})` for an available preset in the current view; obtain IDs from `api.configuration.list()` rather than guessing display labels.

## Return a Mind Map as Markdown

With the chosen canvas already showing a settled Mind Map:

```js
(() => {
  const api = window.kplexApi.v1;
  const canvasId = 'RETURNED_CANVAS_ID';
  const snapshot = api.canvas({canvasId});
  if (!snapshot.ok) return {snapshot};
  if (snapshot.value.scenePending) return {snapshot, message: 'Read again after the scene settles'};
  return {
    snapshot,
    exported: api.exportMarkdown({canvasId, expectedRevision: snapshot.revision}),
  };
})()
```

Inspect `exported.value.markdown` and `exported.value.warnings` after checking `exported.ok`. The API uses visible ontology labels by default and returns text without writing a file or copying to the clipboard. Use `subtreeOccurrenceId` with an exact occurrence ID from that canvas to export one admitted branch. Current filters and folds limit scope; offscreen constructed rows are retained.

PNG export is available in K-Plex's interface, **not** through API v1. Check `capabilities()` for supported exporters. The native Markdown dialog works in all three views; the API's Markdown operation requires a committed Mind Map.

## Combine read queries with GraphQL

```js
window.kplexApi.v1.query({
  query: `query Find($q: String!) {
    search(query: $q, limit: 10) {
      items { id name kind path }
      truncated
      coverage { scope complete pending }
    }
  }`,
  variables: {q: 'Workshop'},
  operationName: 'Find',
})
```

Check the outer `ok` **and** `value.errors`. A successful envelope can contain individual field errors. GraphQL supplies read queries, not mutations or subscriptions. The [API reference](https://github.com/zsviczian/kplex/blob/main/docs/PUBLIC_API.md) documents schema discovery, revision checks, configuration import and limits.
