---
aliases:
- Opening this vault
tags:
- kplex-help/reference
- kplex/getting-started
Guide:
- '[[00 Start Here/K-Plex Help]]'
---
# K-Plex Help

An **end-user guide and live showcase** for K-Plex in Obsidian. The notes themselves form a navigable graph through relationships, tags, topic-based routes, screenshots and images.

Start with [What You Can Do with K-Plex](07%20Use%20cases/Use%20cases.md): practical workflows, from building a topic map and developing an article to running a project, recovering meeting context and making forgotten ideas useful again.

## Open this vault

1. Download and extract this repository, then open the extracted repository folder as an Obsidian vault. Keep its hidden `.obsidian` folder when copying it.
2. Review the included community plugins before enabling them. **This repository includes executable plugin files**, not just documentation and settings. This checkout includes a **development build from main**, deployed October 20, 2026, to demonstrate the draft features. Its unchanged manifest still says **0.1.2**; that label does not identify the development code.
3. Update K-Plex to the latest published release for released workflows. Back up the supplied settings before changing plugin versions; the help's ontology and appearance live in `.obsidian/plugins/k-plex/data.json`.
4. Open K-Plex and use the toolbar Vault Search box to find **K-Plex Help**. Saved shortcuts can differ from new-install defaults; this help configuration retains F4 for Vault Search.
5. Begin at [[00 Start Here/First 5 minutes|First 5 minutes]], [[07 Use cases/Use cases|What You Can Do with K-Plex]], or [[00 Start Here/Choose a topic|Choose a topic]].

## Documentation and release boundary

**Reviewed October 20, 2026.** The latest published K-Plex release is [0.1.3](https://github.com/zsviczian/kplex/releases/tag/0.1.3), released October 13. This update also documents merged changes through [K-Plex main at f646c75](https://github.com/zsviczian/kplex/commit/f646c75bc7d2a4b8ca2f64af43cb8826a30afab9), including paired ontology, document-use cleanup and device-specific indexing.

**Available** refers to released 0.1.3 behavior. **Next release** marks implemented, merged changes that are not in 0.1.3. **Missing** marks capabilities not provided by the reviewed baseline. The draft is not a publication announcement.

A published 0.1.3 installation will not have every draft control described here. The bundled development `main.js` and `styles.css` let you try those controls in this demo vault. This does **not** mean 0.2.0 has been released. The manifest was deliberately left unchanged. The demo ontology now pairs Guide/Explains, Parent/Child and Previous/Next; existing visual assets and semantic styles are preserved.

See [Changes since K-Plex 0.1.3](00%20Start%20Here/Recently%20added%20features.md) for the release-aware overview and source references.

## Release history

Browse [[11 Release notes/Release notes|K-Plex release notes]] for the published history from 0.0.1 through 0.1.3 and the clearly marked **0.2.0 draft**. Release pages use the Help vault's existing **Explains** relationship to link directly to feature guides, so release notes are part of the navigable graph. The bundled development build supports the newly documented workflows; the draft remains a record of proposed release scope.

## Explore by outcome or technique

The **practical use cases** focus on results, with examples, short workflows and a “Done when” finishing point. They reuse and expand existing help pages rather than creating a second disconnected manual.

The **13 discovery paths** in [[00 Start Here/Choose a topic]] teach techniques through the same reference notes. Browse the vault through folders, Markdown links or K-Plex's Parent/Child, Friend/Challenger and Previous/Next relationships. [[00 Start Here/K-Plex Help]] is the home base.

Newly documented areas include Wander, [[02 Navigate and explore/Footprints and breadcrumbs|Footprints (session breadcrumbs)]], independent Plex document pairs, themes and semantic color resets, native dragging, folders and tags, note-creation destinations, safe Sidecar folding, One-sided layout, modifier cross-link previews, live settings and clearer diagnostics.

## Start with the new demonstrations

- [[03 Build and edit/Manage and clean up ontology|Find the documents behind a relationship property]], then inspect a configured pair.
- [[06 Indexing and troubleshooting/On demand vs Eager|Choose startup and indexing behavior per device]].
- [[04 Filter and focus/Expand a note into sections|Explore a long note by heading]].

Fresh screenshots in the guides show the actual development build running in this vault. Existing conceptual illustrations remain as visual introductions.

## Preserved showcase configuration

The existing help settings keep siblings hidden, cross-link opacity at 50%, the regular label limit at 100 and thinner node/relationship/Lens strokes. The October 10 visual update reduced existing numeric stroke widths by one, with a 0.5 minimum; this documentation update does not apply that reduction again.

In the reviewed plugin, **Show cross-links** remains a view-local toggle rather than a persisted setting. Turn it off manually in Filters and lenses to hide those additional lines. Its opacity setting is separate.

The official Sketch Your Mind book cover is referenced online; existing local help assets remain in the repository. Remote images used inside K-Plex nodes require the separate **Allow remote node images** permission in 0.1.3. See [[05 Personalize and workspace/Images in nodes]].

## Official resources

[K-Plex](https://github.com/zsviczian/kplex) · [Obsidian Excalidraw](https://github.com/zsviczian/obsidian-excalidraw-plugin) · [Sketch Your Mind Community](https://community.sketch-your-mind.com/) · [Ko-fi](https://ko-fi.com/zsolt) · [Sketch Your Mind book](https://community.sketch-your-mind.com/sym).
