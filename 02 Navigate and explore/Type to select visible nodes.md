---
tags:
- kplex-help/how-to
- kplex/navigation
- kplex/search
- kplex/keyboard
Guide:
- '[[02 Navigate and explore/Keyboard navigation]]'
Related:
- '[[02 Navigate and explore/Vault Search vs Find in this Plex]]'
- '[[02 Navigate and explore/K-Plex command palette]]'
---
# Type to select visible nodes

Can you see the right neighborhood but not the note you need? Type part of its label to select it without scanning every node.

![[Assets/Screenshot - Type to select.png]]

*Typing gather selects the visible workshop-material note. The center stays on the plan.*

1. Focus the Plex graph with **Ctrl/Cmd+Shift+G** or click empty graph space.
2. Type part of a **displayed node label**. K-Plex looks for a contiguous phrase, ignores letter case and keeps the typed spaces. It searches the *currently displayed graph occurrences*, not the entire vault or hidden/off-screen pages.
3. As characters are added, selection advances through matching visible nodes. **Tab** goes to the next match; **Shift+Tab** goes back.
4. **Backspace** removes the last typed character; **Escape** clears the phrase. **Enter** can then activate the selected node using normal graph navigation.

The query is temporary. It highlights and reveals matches without filtering the graph, changing the center or adding history entries. A configured local character shortcut takes precedence over using that character to start a query.

| Need | Use |
| --- | --- |
| Find a note anywhere in the vault | [[02 Navigate and explore/Vault Search vs Find in this Plex|Search Vault]] |
| Highlight a currently shown node by its name or ontology | [[02 Navigate and explore/Vault Search vs Find in this Plex|Find in Plex]] |
| Jump through currently displayed labels without opening another field | **Type to select** |

> [!note] Text entry belongs to editors
> K-Plex deliberately does not capture typing or composition inside native editors, input fields, dialogs or search boxes. Explicitly focus the graph first.
