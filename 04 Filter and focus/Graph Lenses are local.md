---
aliases:
  - "Graph Lenses are local"
tags:
  - "kplex-help/caution"
  - "kplex/filtering"
  - "kplex/limits"
Friend:
  - "[[01 Core concepts/What K-Plex is not]]"
Previous:
  - "[[04 Filter and focus/Graph Lenses]]"
Next:
  - "[[04 Filter and focus/Keep layout vs Reflow]]"
---
A Graph Lens evaluates the **currently visible K-Plex neighborhood**. It does not transform K-Plex into a deep whole-vault graph query engine.

This is an important boundary. A note that is not part of the projected Plex cannot be revealed merely because a lens condition would match it somewhere else in the vault. Use Obsidian's global search/Bases/Dataview-style tools when your question begins with “find every note in the vault that…”.

Within the visible Plex, however, lenses can reason about information normal note filters cannot easily express — especially **relationship role**, **relationship definition**, and **evidence source**.
