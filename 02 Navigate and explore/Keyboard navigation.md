---
tags:
- kplex-help/how-to
- kplex/navigation
- kplex/keyboard
Guide:
- '[[Navigate and explore]]'
Explains:
- '[[Type to select visible nodes]]'
- '[[Keyboard shortcuts reference]]'
Related:
- "[[Screenshot - Canvas keyboard shortcuts.png]]"
- '[[K-Plex command palette]]'
- '[[Actions and shortcuts]]'
- '[[Past nodes and pins]]'
---
# Keyboard navigation

Explore and connect notes without reaching for the mouse. Give the graph focus, select a nearby node and navigate or run an action from the keyboard.

![[Screenshot - Canvas keyboard shortcuts.png]]

*The current desktop keyboard reference shows effective canvas shortcuts, including Enter to center a note and Alt+Enter to fold a supported branch or section. Saved shortcuts and platform labels can differ.*

## Choose and move

1. Press an **arrow key** to highlight a visible node in the current relationship area. Arrows move selection without moving the center or changing Past nodes.
2. Plain arrows cross to another area at its boundary. Use **Alt/Option+arrow** to move directly to another relationship area.
3. Press **Enter** to center a selected neighbor. In Mind Map this also starts the map from that note. Use **Alt/Option+R** for Rename.
4. **Ctrl/Cmd+Up / Down / Left / Right** starts a Parent / Child / Friend / Challenger relationship from the **canvas center**.
5. Press **Ctrl/Cmd+Enter** to open a selected note in a new native tab. **Alt/Option+Enter** folds or unfolds a supported branch or section; **Alt/Option+0** selects the center.

Selection follows what is currently displayed, including filtering and repacked areas. It does not inspect off-screen notes not included in the visible projection.

## Find a visible node by typing

Just type part of its displayed label while the **graph** is focused. See [[Type to select visible nodes|Type to select visible nodes]] for Tab, Backspace and Escape behavior. This is not Vault search or Find in canvas.

## Do more without leaving the graph

Use **Alt/Option+.** to open the [[K-Plex command palette|K-Plex command palette]], **Alt/Option+?** for keyboard help, and [[Keyboard shortcuts reference|Keyboard shortcuts reference]] for the default bindings. All local actions can be customized in [[Actions and shortcuts|Actions and shortcuts]].

> [!tip] When keys do not move the graph
> Check whether the caret is in a Search/Find/editor input, and use **Ctrl/Cmd+Shift+G** to focus the graph deliberately. A remapped, disabled or conflicting shortcut may also explain a missing action.

## Selection consistency with Find

Finding a node in the current canvas and selecting one with arrow keys now share a common visual highlight. This makes the selection easier to track after switching between the Find box and graph-keyboard navigation; **Enter** still performs the navigation/activation separately.
