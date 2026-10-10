---
tags:
- kplex-help/how-to
- kplex/navigation
- kplex/keyboard
Guide:
- '[[02 Navigate and explore/Navigate and explore]]'
Related:
- '[[02 Navigate and explore/Keyboard navigation]]'
- '[[02 Navigate and explore/Keyboard shortcuts reference]]'
- '[[05 Personalize and workspace/Actions and shortcuts]]'
- '[[03 Build and edit/Create a relationship]]'
---
K-Plex has a **local command palette for the current Plex**. It is distinct from **Obsidian's Command Palette**, which lists published commands from all plugins.

## Run an action

1. Focus a K-Plex graph and press **Alt/Option+.** (period), or use the published **K-Plex command palette** action from Obsidian's Command Palette.
2. Type a command name. The palette searches available actions and shows descriptions and local shortcut hints.
3. Choose an action. K-Plex carries forward the originating Plex and its selected node when relevant; actions that require an unavailable target are not offered.

Try searching for **Pin**, **Rename**, **Connect**, **Open**, **History**, **Zoom**, or **Zen**. The palette also includes creation, connection inspection, section folding, filters/lenses, view options, and navigation, depending on the current context.

> [!important] Current selection versus center
> Some operations use the **selected node**, some use the **center**. A command explicitly titled **selected node** requires a selection; a selected-or-center action falls back to the center when nothing is selected. The palette captures the origin before opening its modal, avoiding accidental retargeting.

## Local commands versus Obsidian commands

- The **K-Plex palette** acts in a particular Plex and shows context-appropriate actions. Its default graph shortcut is **Alt/Option+.**.
- **Obsidian's Command Palette** contains actions **published** by K-Plex plus commands from other plugins. Published actions can receive Obsidian-wide hotkeys under **Settings → Hotkeys**.
- Publishing an action does not automatically create a global shortcut. Hiding a command from Obsidian does **not** disable its graph-local shortcut or local palette availability.

You can manage both dimensions from [[05 Personalize and workspace/Actions and shortcuts|Actions and shortcuts]]. For a quick read-only list of your current bindings, press **Alt/Option+?** to open **Keyboard help** while the graph is focused.

**Try it:** Highlight a node, open the palette, search for **Pin**, then navigate elsewhere and use [[02 Navigate and explore/Past nodes and pins|pins]] to return.
