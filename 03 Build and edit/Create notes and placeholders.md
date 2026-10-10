---
aliases:
  - "Create notes and placeholders"
tags:
  - "kplex-help/how-to"
  - "kplex/relationships"
  - "kplex/placeholders"
Friend:
  - "[[01 Core concepts/Node types]]"
Previous:
  - "[[03 Build and edit/Create a relationship]]"
Next:
  - "[[03 Build and edit/Drag drop and reclassify]]"
---
A **placeholder** is an unresolved relationship with only the intended note name. No file exists yet. This is useful when the structure of an idea is clear before the content is ready.

When you later materialize the placeholder, K-Plex creates the Markdown note and the graph can keep the conceptual position you already established. Placeholders cannot persist aliases because there is no file metadata to store them.

When folder nodes are visible, drag outward from a folder's **Child gate** to create a new Markdown note directly in that folder. The file-tree relationship supplies the folder connection, so K-Plex does not add a redundant note-to-note property merely to represent file location.

Web links are different: adding one requires a Markdown origin because the relationship is persisted in document properties.
