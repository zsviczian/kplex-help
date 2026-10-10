---
aliases:
- Troubleshooting checklist
tags:
- kplex-help/caution
- kplex/indexing
- kplex/troubleshooting
Related:
- '[[03 Build and edit/Connection details and evidence]]'
- '[[05 Personalize and workspace/Layout density and typography]]'
- '[[08 About/Community GitHub and contributing]]'
Previous:
- '[[06 Indexing and troubleshooting/Rebuild purge and diagnostics]]'
---
![[Image - Graph troubleshooting.png]]

Start with the **smallest affected scope**. A missing URL, an unfamiliar relationship and a stale graph do not have the same cause.

## What do you observe?

| Symptom | Start here |
| --- | --- |
| **One link points the wrong way** | [[03 Build and edit/Connection details and evidence|Inspect Connection details…]] and the source ontology. |
| **One note seems stale** | Revisit the note or use **Refresh** before rebuilding anything. |
| **A web link is missing** | Check [[06 Indexing and troubleshooting/Web link indexing|Web link discovery]]; the URL inventory can lag behind local readiness. |
| **Gate count says ≥ or is incomplete** | Check [[06 Indexing and troubleshooting/How indexing works|local readiness]] and whether the neighborhood is still preparing. |
| **Some nodes vanish after filtering** | Clear [[04 Filter and focus/Quick Filter|Quick Filter]] or a [[04 Filter and focus/Graph Lenses|Graph Lens]] first. |
| **The layout is crowded** | Try [[04 Filter and focus/Keep layout vs Reflow|Reflow]], depth, or [[05 Personalize and workspace/Layout density and typography|layout controls]]. |
| **Persistent source data seems wrong** | Use [[06 Indexing and troubleshooting/Rebuild purge and diagnostics|Rebuild index]] and consider a cache purge only as a later step. |

## If the issue persists

Write down steps to reproduce, expected/actual behavior, Obsidian and K-Plex versions, and device type. Use **Copy index diagnostics** for indexing issues, then report the problem through [[08 About/Community GitHub and contributing|GitHub issues]].

> [!warning] Do not purge first
> Purging deletes K-Plex's derived IndexedDB index, not the source notes, but requires an Obsidian restart and makes K-Plex rebuild data. Try inspection, Refresh and Rebuild first.

## Recent status and editor-suggester fixes

The index status display now catches up when K-Plex is revealed and no longer presents on-demand local publication as `x of y` vault files. Check [[06 Indexing and troubleshooting/Understanding index status|Understanding index status]] before diagnosing a stuck counter. Long-paste ontology autocomplete has also been hardened; if editor pastes still freeze, capture a reproduction as described in [[03 Build and edit/Ontology autocomplete|Ontology autocomplete]].

## When startup appears stuck

If the local Plex is already usable but the cache indicator remains active, first inspect the status details and allow background work to proceed. K-Plex can now retire some **inactive restore operations** rather than wait forever for a cache-loading promise. The restore watchdog checks for lack of progress; it does not declare a healthy large vault broken after a fixed total time.

Only rebuild or purge the persistent index after checking [[06 Indexing and troubleshooting/Understanding index status|Understanding index status]] and [[06 Indexing and troubleshooting/Rebuild purge and diagnostics|Rebuild, purge and diagnostics]].

[Change: PR #95](https://github.com/zsviczian/kplex/pull/95).
