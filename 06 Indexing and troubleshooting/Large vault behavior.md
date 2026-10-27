---
aliases:
  - "Large vault behavior"
tags:
  - "kplex-help/concept"
  - "kplex/indexing"
  - "kplex/performance"
Friend:
  - "[[06 Indexing and troubleshooting/On demand vs Eager]]"
  - "[[06 Indexing and troubleshooting/Troubleshooting checklist]]"
Previous:
  - "[[06 Indexing and troubleshooting/Web link indexing]]"
Next:
  - "[[06 Indexing and troubleshooting/Rebuild purge and diagnostics]]"
---
# Large vault behavior

Have a large vault and want to get to work without waiting for everything? Start with the note you need while K-Plex prepares more context in the background.

![[Assets/Screenshot - Index status.png]]

*The status details explain the current preparation phase. This capture shows the real update in progress while the help notes were being edited.*

Filename/path search and Obsidian-known relationships can appear while indexing continues. A note that belongs to a large tag or folder does not require all of its siblings to load before the note opens. A **≥** gate count means relationships prepared so far are shown, with more potentially arriving as the neighborhood loads.

When every K-Plex surface is hidden, automatic indexing pauses and waiting changes are gathered for later. Showing K-Plex again catches up. Incoming updates preserve your position on the map instead of repeatedly recentering the graph.

If one note exceeds the supported relationship-loading bound, K-Plex can report that its local graph counts are unavailable without implying that the entire index has failed.

## If the graph still looks incomplete

Check the [[06 Indexing and troubleshooting/Understanding index status|status indicator]] and try navigating to the particular note you need. If a result stays wrong, [[06 Indexing and troubleshooting/Rebuild purge and diagnostics|capture diagnostics]] before restarting.

## Keep useful progress while notes change

K-Plex reuses valid completed indexing work as notes are edited, rather than repeatedly starting the whole operation again. Reopening the vault can also reuse cached information after validation. This reduces repeated background work; the amount of time saved depends on the vault and cache state.

Ordinary autosaves retain stable gate counts when relationships have not changed. Actual relationship changes still update the counts. Tag and folder nodes show zero for Friend and Challenger relationships that do not apply to them.
