---
aliases:
- Indexing and troubleshooting
tags:
- kplex-help/section
- kplex/indexing
Child:
- '[[How indexing works]]'
- '[[On demand vs Eager]]'
- '[[Web link indexing]]'
- '[[Large vault behavior]]'
- '[[Rebuild purge and diagnostics]]'
- '[[Troubleshooting checklist]]'
- '[[Understanding index status]]'
Friend:
- '[[What K-Plex is not]]'
Related:
- '[[08 Indexing and problem solving]]'
---
# Indexing and troubleshooting

Is a connection missing, or are you unsure what is still loading? Check the current graph's readiness, then follow the smallest useful recovery step.

## Understand readiness

- [[How indexing works|How indexing works]] — local graph versus background work.
- [[On demand vs Eager|On demand vs Eager]] — when relationships are prepared.
- [[Web link indexing|Web link indexing]] — why URLs can appear after notes.
- [[Large vault behavior|Large vault behavior]] — cached data, incremental updates and gate counts.

## When something looks wrong

Start with [[Troubleshooting checklist|Troubleshooting checklist]], and move to [[Rebuild purge and diagnostics|Rebuild, purge and diagnostics]] only if needed.

**Try this:** Open **Settings → K-Plex → Indexing config** and review the startup and strategy choices for each device. You do not need to wait for URL discovery to explore local notes.

Follow [[08 Indexing and problem solving|Indexing and problem solving]] for a practical sequence.

## Reading the indicator

[[Understanding index status|Understanding index status]] distinguishes the selected local graph, full-index progress and independent URL discovery. In **On demand**, an `x of y` vault-indexing ratio would be misleading; in **Eager** mode genuine whole-index progress can be shown.
