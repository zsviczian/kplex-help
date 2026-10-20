---
aliases:
- Indexing and troubleshooting
tags:
- kplex-help/section
- kplex/indexing
Child:
- '[[06 Indexing and troubleshooting/How indexing works]]'
- '[[06 Indexing and troubleshooting/On demand vs Eager]]'
- '[[06 Indexing and troubleshooting/Web link indexing]]'
- '[[06 Indexing and troubleshooting/Large vault behavior]]'
- '[[06 Indexing and troubleshooting/Rebuild purge and diagnostics]]'
- '[[06 Indexing and troubleshooting/Troubleshooting checklist]]'
- '[[06 Indexing and troubleshooting/Understanding index status]]'
Friend:
- '[[01 Core concepts/What K-Plex is not]]'
---
K-Plex makes **foreground tasks useful before every background job is finished**. A visible local neighborhood, a complete URL inventory, and a fully prepared index are different states.

## Understand readiness

- [[06 Indexing and troubleshooting/How indexing works|How indexing works]] — local graph versus background work.
- [[06 Indexing and troubleshooting/On demand vs Eager|On demand vs Eager]] — when semantic data is prepared.
- [[06 Indexing and troubleshooting/Web link indexing|Web link indexing]] — why URLs can appear after notes.
- [[06 Indexing and troubleshooting/Large vault behavior|Large vault behavior]] — cached data, incremental updates and gate counts.

## When something looks wrong

Start with [[06 Indexing and troubleshooting/Troubleshooting checklist|Troubleshooting checklist]], and move to [[06 Indexing and troubleshooting/Rebuild purge and diagnostics|Rebuild, purge and diagnostics]] only if needed.

**Try this:** Open **Settings → K-Plex → Indexing config** and review the startup and strategy choices for each device. You do not need to wait for URL discovery to explore local notes.

Follow [[10 Discover by topic/08 Indexing and problem solving|Indexing and problem solving]] for a practical sequence.

## Reading the indicator

[[06 Indexing and troubleshooting/Understanding index status|Understanding index status]] distinguishes the selected local graph, full-index progress and independent URL discovery. In **On demand**, an `x of y` vault-indexing ratio would be misleading; in **Eager** mode genuine whole-index progress can be shown.
