---
aliases:
  - "Rebuild purge and diagnostics"
tags:
  - "kplex-help/how-to"
  - "kplex/indexing"
  - "kplex/troubleshooting"
Friend:
  - "[[08 About/Community GitHub and contributing]]"
Previous:
  - "[[06 Indexing and troubleshooting/Large vault behavior]]"
Next:
  - "[[06 Indexing and troubleshooting/Troubleshooting checklist]]"
---
Use maintenance tools in increasing order of disruption:

1. **Refresh** the current K-Plex view if graph data looks stale.
2. Run **K-Plex: Rebuild index** when you want K-Plex to re-evaluate derived graph data.
3. Use **Indexing config → Purge index cache** when you need to delete the persistent IndexedDB cache. Your notes are not changed, but you must restart Obsidian before continuing with K-Plex.
4. Run **K-Plex: Copy index diagnostics** when reporting a performance/indexing problem. The report is designed to avoid vault paths while exposing useful state.

The cache-size display in Settings is an approximate logical payload estimate, not necessarily the physical disk allocation.
