---
tags:
- kplex-help/how-to
- kplex/navigation
- kplex/keyboard
Guide:
- '[[02 Navigate and explore/Navigate and explore]]'
Explains:
- '[[02 Navigate and explore/Type to select visible nodes]]'
- '[[02 Navigate and explore/Keyboard shortcuts reference]]'
Related:
- '[[02 Navigate and explore/K-Plex command palette]]'
- '[[05 Personalize and workspace/Actions and shortcuts]]'
- '[[02 Navigate and explore/Past nodes and pins]]'
---
# Keyboard navigation

Explore and connect notes without reaching for the mouse. Give the graph focus, select a nearby node and navigate or run an action from the keyboard.

![[Assets/Screenshot - Keyboard help.png]]

*The built-in keyboard reference shows the effective shortcuts in this vault. Your saved keys can differ from fresh-install defaults.*

## Choose and move

1. Press an **arrow key** to highlight a visible node in the current relationship area. Arrows move selection without moving the center or changing Past nodes.
2. Press **Alt/Option+arrow** to move to another relationship area. The **Move across section boundaries** preference controls whether plain arrows also cross at the end of an area. New installs enable that behavior; upgraded configurations keep their existing choice.
3. Press **Enter** to center a selected neighbor. On a selected central file it opens **Rename**. The selected node may be revealed inside a scrollable area first.
4. **Ctrl/Cmd+Up / Down / Left / Right** starts a Parent / Child / Friend / Challenger relationship from the **canvas center**.
5. Press **Ctrl/Cmd+Enter** on a selected note to center it and ensure its Sidecar is open. **Alt/Option+0** selects the center.

Selection follows what is currently displayed, including filtering and repacked areas. It does not inspect off-screen notes not included in the visible projection.

## Find a visible node by typing

Just type part of its displayed label while the **graph** is focused. See [[02 Navigate and explore/Type to select visible nodes|Type to select visible nodes]] for Tab, Backspace and Escape behavior. This is not Vault search or Find in canvas.

## Do more without leaving the graph

Use **Alt/Option+.** to open the [[02 Navigate and explore/K-Plex command palette|K-Plex command palette]], **Alt/Option+?** for keyboard help, and [[02 Navigate and explore/Keyboard shortcuts reference|Keyboard shortcuts reference]] for the default bindings. All local actions can be customized in [[05 Personalize and workspace/Actions and shortcuts|Actions and shortcuts]].

> [!tip] When keys do not move the graph
> Check whether the caret is in a Search/Find/editor input, and use **Ctrl/Cmd+Shift+G** to focus the graph deliberately. A remapped, disabled or conflicting shortcut may also explain a missing action.

## Selection consistency with Find

Finding a node in the current canvas and selecting one with arrow keys now share a common visual highlight. This makes the selection easier to track after switching between the Find box and graph-keyboard navigation; **Enter** still performs the navigation/activation separately.
