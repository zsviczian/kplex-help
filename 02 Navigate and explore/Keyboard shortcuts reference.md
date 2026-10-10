---
tags:
- kplex-help/reference
- kplex/navigation
- kplex/keyboard
Guide:
- '[[02 Navigate and explore/Navigate and explore]]'
Related:
- '[[05 Personalize and workspace/Actions and shortcuts]]'
- '[[02 Navigate and explore/Keyboard navigation]]'
- '[[02 Navigate and explore/K-Plex command palette]]'
---
These are the current **fresh-install defaults** when the relevant K-Plex surface has keyboard focus. Existing vaults can retain older assignments (such as **F4** for Search Vault), explicit disables and custom bindings. Your own settings and the in-app **Keyboard help** are authoritative for your installation.

## Focus, selection and movement

| Shortcut | Action |
| --- | --- |
| **Ctrl/Cmd+Shift+G** | Focus the graph. |
| **Ctrl/Cmd+Shift+E** | Focus the existing embedded or Sidecar editor. |
| **Arrow keys** | Select another visible node within the area. |
| **Alt/Option+arrows** | Switch relationship areas. |
| **Alt/Option+0** | Select the center. |
| **Enter** | Activate selected node; rename if the central file is selected. |
| **Ctrl/Cmd+Enter** | Center the selected note and open/ensure its Sidecar. |
| **Type a label** | Select matching visible nodes (graph focus). |
| **Tab / Shift+Tab** | Next / previous typed match (only while a type-to-select phrase is active). |
| **Backspace** | Edit active typed phrase; otherwise return in Plex history. |
| **Shift+Backspace** | Move forward in Plex history when not typing a search phrase. |
| **Escape** | Clear active phrase first; otherwise follow the focused UI's cancellation behavior. |

## Actions and graph tools

| Shortcut | Action |
| --- | --- |
| **Alt/Option+.** | Open the K-Plex command palette. |
| **Alt/Option+?** | Open the read-only Keyboard help. |
| **Alt/Option+/** | Focus Search Vault on the Plex. |
| **Ctrl/Cmd+F** | Focus Find in Plex when the graph has focus; in an editor it stays the editor's Find. |
| **Alt/Option+R** | Rename selected node, or center. |
| **Alt/Option+P** | Pin / unpin selected node, or center. |
| **Alt/Option+B** | Open complete pins picker. |
| **Alt/Option+H** | Open complete Past nodes picker. |
| **Alt/Option+C** | Connect selected node / center to an existing node. |
| **Alt/Option+M** | Open selected node / center context menu. |
| **Ctrl/Cmd+↑** | Start **Add parent** from the center. |
| **Ctrl/Cmd+↓** | Start **Add child** from the center. |
| **Ctrl/Cmd+←** | Start **Add friend** from the center. |
| **Ctrl/Cmd+→** | Start **Add challenger** from the center. |

## Field and dialog focus matters

- **Search Vault:** Up/Down chooses search results, Enter opens one, Escape dismisses results. **Find in Plex:** Enter/Shift+Enter cycles matches; Escape clears and closes Find.
- **Graph:** Arrow navigation and type-to-select apply only while the graph owns focus. Native editors, note input fields and modal controls keep their own key behavior.
- **Relationship dialog:** **Ctrl/Cmd+Enter** submits when its inputs can accept the shortcut; **Ctrl/Cmd+Shift+Enter** creates/connects another while retaining the captured origin. Accept an open suggestion first.
- Shortcut bindings and command publication are independent. No global Obsidian hotkey is installed automatically for these local graph actions.

> [!tip] Your keyboard may differ
> The Alt/Option punctuation shortcuts use physical-key defaults so modified letters or punctuation that produce accents can still work. Check **Keyboard help** and [[05 Personalize and workspace/Actions and shortcuts|Actions and shortcuts]] for active mappings, alternate layouts, disabled commands or collisions.

Full feature guidance: [[02 Navigate and explore/Keyboard navigation|Keyboard navigation]], [[02 Navigate and explore/Type to select visible nodes|Type to select visible nodes]], and [[02 Navigate and explore/K-Plex command palette|K-Plex command palette]].
