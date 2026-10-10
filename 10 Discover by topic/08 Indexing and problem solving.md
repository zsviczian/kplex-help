---
aliases:
- Indexing and problem solving
tags:
- kplex-help/path
- kplex/discovery
- kplex/indexing
- kplex/troubleshooting
Explains:
- '[[06 Indexing and troubleshooting/How indexing works]]'
- '[[06 Indexing and troubleshooting/On demand vs Eager]]'
- '[[06 Indexing and troubleshooting/Large vault behavior]]'
- '[[06 Indexing and troubleshooting/Web link indexing]]'
- '[[06 Indexing and troubleshooting/Troubleshooting checklist]]'
- '[[06 Indexing and troubleshooting/Rebuild purge and diagnostics]]'
- '[[06 Indexing and troubleshooting/Understanding index status]]'
Related:
- '[[10 Discover by topic/09 Work with web sources]]'
- '[[10 Discover by topic/12 Connect dates and daily notes]]'
---
> **Your goal:** Know what is ready, what is still loading, and what to try when results look incomplete.

You have a large vault, changing files, stale results or incomplete web-link inventory.

## Follow the trail

These are existing help notes, presented here in a useful order. You can follow the wikilinks in Markdown or open this path in K-Plex and explore its **Children**.

1. **[[06 Indexing and troubleshooting/How indexing works|How indexing works]]** — Separate local usability from background completeness.
2. **[[06 Indexing and troubleshooting/On demand vs Eager|On demand vs Eager]]** — Choose when semantic relationships are prepared.
3. **[[06 Indexing and troubleshooting/Large vault behavior|Large vault behavior]]** — Read incomplete counts and incremental updates.
4. **[[06 Indexing and troubleshooting/Web link indexing|Web link indexing]]** — Understand why URLs can arrive later than local notes.
5. **[[06 Indexing and troubleshooting/Troubleshooting checklist|Troubleshooting checklist]]** — Start with the least disruptive diagnostic.
6. **[[06 Indexing and troubleshooting/Rebuild purge and diagnostics|Rebuild purge and diagnostics]]** — Use cache actions only when appropriate.


## New capabilities on this route

- [[06 Indexing and troubleshooting/Understanding index status|Understanding index status]] — separate local readiness, full indexing and URL inventory

## Try it in your own vault

Open **Settings → K-Plex → Indexing config**. Check the mode and web-link status before considering a rebuild. Do not purge a healthy cache to complete this exercise.

## Additional exercise

Check the index indicator after changing centers; do not interpret on-demand local readiness as whole-vault `x of y` progress.

## Continue discovering

- [[10 Discover by topic/09 Work with web sources|Work with web sources]] — a useful neighboring path.
- [[00 Start Here/Choose a topic|All discovery paths]] — choose another goal.
- [[00 Start Here/K-Plex Help|Help home]] — return to the main map.

## Cache recovery changes

Follow [[06 Indexing and troubleshooting/Web link indexing|Web link indexing]] and [[06 Indexing and troubleshooting/Large vault behavior|Large vault behavior]] for recent improvements in URL-heavy startup and source replay. Cache inactivity watchdogs now retire stalled restores without treating a healthy long-running index as failed after a fixed total duration.
