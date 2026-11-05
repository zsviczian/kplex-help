---
aliases:
- How indexing works
tags:
- kplex-help/concept
- kplex/indexing
- kplex/performance
Friend:
- '[[01 Core concepts/Relationship sources and inference]]'
- '[[06 Indexing and troubleshooting/Rebuild purge and diagnostics]]'
Next:
- '[[06 Indexing and troubleshooting/On demand vs Eager]]'
---
# How indexing works

Know whether you can start exploring while K-Plex is still preparing. Your current neighborhood can be usable before every relationship and website has been discovered.

![[Assets/Screenshot - Index status.png]]

*The status details explain the current preparation phase. This capture shows the real update in progress while the help notes were being edited.*

![[Image - indexing approach.png]]

## Two different readiness questions

- **Can I work in the current canvas?** Often yes before indexing is complete. Filename/path lookup and Obsidian-known local relationships can become available early.
- **Is every relationship or URL discovered?** Not necessarily. Wider preparation and web-link discovery can continue while you navigate.

K-Plex prioritizes **navigation and explicit edits**, then the current requested neighborhood, over unrelated background maintenance. Cached data can accelerate later starts; it does not mean K-Plex has already revalidated every source.

In **On demand** mode, local counts can reflect only prepared relationships; body-only links may be added as more notes are indexed. The UI may report **Preparing local graph**, **Local graph ready**, or **Local graph counts unavailable**. A **≥** gate count signals a lower bound, not a guaranteed total.

## What do I need to do?

Usually nothing. Explore the current note. If you need relationships throughout the vault, review [[06 Indexing and troubleshooting/On demand vs Eager|On demand vs Eager]]. If a particular source looks wrong, inspect [[03 Build and edit/Connection details and evidence|Connection details]] before taking the more disruptive maintenance steps in [[06 Indexing and troubleshooting/Troubleshooting checklist|Troubleshooting checklist]].

## What the index indicator is measuring

The local graph can be **ready** even as web links or full indexing continue. In **On demand** mode, the status describes the neighborhood you are using. **Eager** full-index work can show an `x of y` count. See [[06 Indexing and troubleshooting/Understanding index status|Understanding index status]].

## Keep useful progress while notes change

K-Plex reuses valid completed indexing work as notes are edited, rather than repeatedly starting the whole operation again. Reopening the vault can also reuse cached information after validation. This reduces repeated background work; the amount of time saved depends on the vault and cache state.

Ordinary autosaves retain stable gate counts when relationships have not changed. Actual relationship changes still update the counts. Tag and folder nodes show zero for Friend and Challenger relationships that do not apply to them.

## Reopen a saved graph while Sync catches up

When a compatible saved graph is available, K-Plex can display it while validating changes received through Obsidian Sync. Cached relationships are useful context, but they are not a claim that every incoming edit has already been checked. Wider validation can continue without withholding all local work.

After Eager preparation finishes, file changes update affected relationships instead of routinely turning the whole graph into unprepared neighborhoods. Canvas edits and the area you are actively using take priority over unrelated work. Source recovery also reuses valid information to reduce repeated cache reads.

Timing still depends on vault size, changed files, disk access and Sync activity. If preparation repeatedly restarts or a gate stays at **…**, capture diagnostics with the active note and recent actions before rebuilding or purging.
