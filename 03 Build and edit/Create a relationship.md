---
aliases:
- Create a relationship
tags:
- kplex-help/how-to
- kplex/relationships
Related:
- '[[01 Core concepts/Ontology and relationship fields]]'
- '[[01 Core concepts/Relationship roles]]'
Next:
- '[[03 Build and edit/Create notes and placeholders]]'
---
![[Image - Connections.png]]

Create Parent, Child, Friend and Challenger relationships from a gate, the Command Palette, or context menus.

The add-related dialog can:

- fuzzy-search existing notes;
- fuzzy-search ontology fields, or browse the full ontology list;
- create a new Markdown note;
- create an Excalidraw note when the Excalidraw plugin is available;
- remember the last ontology field used for each role;
- optionally open the new note for editing;
- create a name-only **Placeholder** instead of a file;
- accept a web link when the origin is a Markdown note.

When K-Plex creates a new relationship property, it adds that property at the bottom of the document property list.

> [!practice]
> In a test note, run **K-Plex: Add friend** and use `Related` as the ontology. The node should appear on the left because this help `data.json` classifies `Related` as Friend ontology.

**Keyboard option:** while the graph owns focus, **Ctrl/Cmd+↑/↓/←/→** starts a Parent/Child/Friend/Challenger relationship from the **center**. The [[02 Navigate and explore/K-Plex command palette|K-Plex command palette]] also offers relationship actions, including context-dependent selected-node operations. Configure keys under [[05 Personalize and workspace/Actions and shortcuts|Actions and shortcuts]].
