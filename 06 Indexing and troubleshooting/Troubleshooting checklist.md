---
aliases:
- Troubleshooting checklist
tags:
- kplex-help/caution
- kplex/indexing
- kplex/troubleshooting
Related:
- '[[Connection details and evidence]]'
- '[[Layout density and typography]]'
- '[[Community GitHub and contributing]]'
Previous:
- '[[Rebuild purge and diagnostics]]'
---
# Troubleshooting checklist

Something on the map does not look right? Match the symptom to a small check before restarting or rebuilding the index.

![[Screenshot - Report a problem.png]]

*Report a bug copies diagnostics and opens this review dialog. Nothing is submitted automatically.*

![[Image - Graph troubleshooting.png]]

## What do you observe?

| Symptom | Start here |
| --- | --- |
| **One link points the wrong way** | [Inspect Connection details…](<Connection details and evidence.md>) and the source ontology. |
| **One note seems stale** | Revisit the note or use **Refresh** before rebuilding anything. |
| **A web link is missing** | Check [Web link discovery](<Web link indexing.md>); the URL inventory can lag behind local readiness. |
| **Gate count says ≥ or is incomplete** | Check [local readiness](<How indexing works.md>) and whether the neighborhood is still preparing. |
| **Some nodes vanish after filtering** | Clear [[Quick Filter]] or a [Graph Lens](<Graph Lenses.md>) first. |
| **The layout is crowded** | Try [Reflow](<Keep layout vs Reflow.md>), depth, or [layout controls](<Layout density and typography.md>). |
| **Persistent source data seems wrong** | Use [Rebuild index](<Rebuild purge and diagnostics.md>) and consider a cache purge only as a later step. |

## If the issue persists

Write down steps to reproduce, expected/actual behavior, Obsidian and K-Plex versions, and device type. Use **Copy index diagnostics** for indexing issues, then report the problem through [[Community GitHub and contributing|GitHub issues]].

> [!warning] Do not purge first
> Purging deletes K-Plex's derived IndexedDB index, not the source notes, but requires an Obsidian restart and makes K-Plex rebuild data. Try inspection, Refresh and Rebuild first.

## Recent status and editor-suggester fixes

If loading appears stuck, [[Understanding index status|read the status]] and capture diagnostics before resetting anything.

## When startup appears stuck

If the local canvas is already usable but the cache indicator remains active, first inspect the status details and allow background work to proceed. K-Plex can now retire some **inactive restore operations** rather than wait forever for a cache-loading promise. The restore watchdog checks for lack of progress; it does not declare a healthy large vault broken after a fixed total time.

Only rebuild or purge the persistent index after checking [[Understanding index status|Understanding index status]] and [[Rebuild purge and diagnostics|Rebuild, purge and diagnostics]].
