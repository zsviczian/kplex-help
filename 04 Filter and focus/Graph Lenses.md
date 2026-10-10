---
aliases:
  - "Graph Lenses"
tags:
  - "kplex-help/concept"
  - "kplex/filtering"
  - "kplex/lenses"
Friend:
  - "[[03 Build and edit/Connection details and evidence]]"
Watch out:
  - "[[04 Filter and focus/Graph Lenses are local]]"
Previous:
  - "[[04 Filter and focus/Quick Filter]]"
Next:
  - "[[04 Filter and focus/Graph Lenses are local]]"
---
![[Screenshot - Filters and Lenses.png]]

A **Graph Lens** is a reusable filter or styling rule for the **currently visible Plex**. You can keep several perspectives ready rather than re-entering a Quick Filter each time.

A lens has three decisions:

1. **Scope:** match a **Note** (such as tag/path/property), a resolved **Relationship** (role or ontology), or its supporting **Evidence** (source occurrence).
2. **Effect:** **Show matching**, **Hide matching**, or **Style matching**.
3. **Conditions:** define what qualifies for that scope.

The normal editor is a visual rule builder. Advanced expression mode is declarative; it is **not JavaScript execution**.

## Examples in this help

The bundled settings include disabled example lenses for how-to notes, cautions, and Challenger relationships. You can inspect and enable them without losing the original content.

> [!important] A Lens is not a whole-vault query
> It does not fetch disconnected notes merely because they match a condition. Read [[04 Filter and focus/Graph Lenses are local|Graph Lenses are local]] for the scope limit.

**Try it:** With [[00 Start Here/K-Plex Help|K-Plex Help]] centered, open **Filters and lenses** and inspect the example named **Help · How-to notes**. Compare its filter effect with **Style matching**. Then learn [[04 Filter and focus/Keep layout vs Reflow|Keep layout vs Reflow]].
