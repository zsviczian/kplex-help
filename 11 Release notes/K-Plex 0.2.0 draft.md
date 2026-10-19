---
aliases:
- K-Plex 0.2.0 release draft
tags:
- kplex-help/release-notes
- kplex/unreleased
Guide:
- '[[11 Release notes/Release notes]]'
Explains:
- '[[03 Build and edit/Drag drop and reclassify]]'
- '[[03 Build and edit/Create notes and placeholders]]'
- '[[05 Personalize and workspace/Note-tab synchronization]]'
- '[[02 Navigate and explore/Footprints and breadcrumbs]]'
- '[[05 Personalize and workspace/Colors and themes]]'
- '[[05 Personalize and workspace/Visibility and connector styling]]'
- '[[05 Personalize and workspace/Sidecar]]'
- '[[06 Indexing and troubleshooting/Understanding index status]]'
---
# K-Plex 0.2.0 — draft release notes

> [!warning] Draft — not published
> Proposed version **0.2.0**. These features are based on accepted, merged changes since [0.1.3](https://github.com/zsviczian/kplex/releases/tag/0.1.3), reviewed October 19, 2026. This is a starting point for editing and screenshots, **not** the final release announcement. Verify the final release tag before publication.

## Your knowledge, your workspace

K-Plex is becoming more than a way to navigate connected notes. Organize knowledge directly from the graph, keep different tasks in separate Plex views, retrace an exploration, and make the workspace fit your preferred appearance.

### Organize your vault while exploring

Bring notes from Obsidian into K-Plex and drag them between views or into a Markdown draft. Move supported notes or folders to folder destinations, assign tags, and create new notes or placeholders in a chosen location. The graph becomes a place to **do the organizing**, not merely inspect its result.

Learn more: [[03 Build and edit/Drag drop and reclassify]] · [[03 Build and edit/Create notes and placeholders]]. [Implementation: PR #177](https://github.com/zsviczian/kplex/pull/177).

### Keep two lines of thought open

Work with multiple independent Plex views and their own document synchronization and Sidecar associations. For example, keep your project or article centered in one Plex while following references in another. Fold the Plex tab group when you want more room for the document.

Learn more: [[05 Personalize and workspace/Note-tab synchronization]] · [[05 Personalize and workspace/Sidecar]]. [PR #187](https://github.com/zsviczian/kplex/pull/187) · [PR #173](https://github.com/zsviczian/kplex/pull/173).

### Retrace your visit trail with Footprints

Each Plex now records its own **complete session visit trail**, including repeated visits. Revisit earlier stops, start a fresh trail, or copy it as Markdown. Footprints is **not persisted**, unlike the shared saved Past nodes history and pins. A branching visual map of the journey is not included.

Learn more: [[02 Navigate and explore/Footprints and breadcrumbs]]. [PR #187](https://github.com/zsviczian/kplex/pull/187).

### Make K-Plex look and feel like your Obsidian workspace

Use native Obsidian theme colors, named appearances and paired light/dark colors. Reset basic colors independently from the semantic styles of your nodes and relationships. Adjust the layout and reduce visual noise with more deliberate hover behavior, including Alt/Option previews of crosslinks that are normally hidden.

Learn more: [[05 Personalize and workspace/Colors and themes]] · [[05 Personalize and workspace/Visibility and connector styling]] · [[05 Personalize and workspace/Layout density and typography]]. [PR #158](https://github.com/zsviczian/kplex/pull/158) · [PR #181](https://github.com/zsviczian/kplex/pull/181).

## Under the hood: fewer interruptions

Settings updates arriving through Obsidian Sync can apply to the running plugin without immediately writing the same settings back. Navigation, indexing and graph presentation behave more consistently during startup, late ontology processing and normal Markdown autosaves. Diagnostics now capture more useful session activity when reporting a problem.

Learn more: [[06 Indexing and troubleshooting/Understanding index status]] · [[06 Indexing and troubleshooting/Rebuild purge and diagnostics]]. Sources: [#182](https://github.com/zsviczian/kplex/pull/182), [#180](https://github.com/zsviczian/kplex/pull/180), [#183](https://github.com/zsviczian/kplex/pull/183), [#186](https://github.com/zsviczian/kplex/pull/186), [#174](https://github.com/zsviczian/kplex/pull/174).

## Before publishing

Add screenshots captured in Obsidian, verify every workflow against the actual 0.2.0 build, update the bundled help plugin deliberately, and replace this warning with the published release date and tag. Document any known platform limitations rather than implying all interactions were manually tested.
