---
aliases:
  - "What K-Plex is not"
tags:
  - "kplex-help/caution"
  - "kplex/concepts"
  - "kplex/limits"
Friend:
  - "[[01 Core concepts/What K-Plex is]]"
  - "[[04 Filter and focus/Graph Lenses are local]]"
  - "[[06 Indexing and troubleshooting/How indexing works]]"
---
K-Plex is deliberately **not** an arbitrary whole-vault force graph or a replacement for every search/query workflow.

Its core working surface is the **current neighborhood around one center**. Graph Lenses evaluate the currently visible Plex; they do not run a deep arbitrary graph query over the entire vault. Section expansion is temporary; it does not permanently turn every heading into a global node. On-demand indexing can also mean that background-derived information arrives after the immediately useful local graph.

These boundaries are strengths when your goal is navigation: they keep the graph readable, make spatial meaning predictable, and let foreground actions receive priority over full-vault maintenance.

If you need a whole-vault inventory, combine K-Plex with Obsidian search, Bases, Dataview, or other tools built for global queries.
