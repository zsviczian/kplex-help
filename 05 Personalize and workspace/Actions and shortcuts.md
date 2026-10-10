---
tags:
  - kplex-help/how-to
  - kplex/settings
  - kplex/keyboard
Guide:
  - "[[05 Personalize and workspace/Personalize and workspace]]"
Related:
  - "[[02 Navigate and explore/Keyboard shortcuts reference]]"
  - "[[02 Navigate and explore/K-Plex command palette]]"
  - "[[02 Navigate and explore/Keyboard navigation]]"
  - "[[05 Personalize and workspace/Fullscreen and Zen mode]]"
---
Use **Settings → K-Plex → Actions and shortcuts** to adapt the same actions used by the graph buttons, context menus, local command palette and keyboard.

## Find and change a shortcut

1. Open **Actions and shortcuts**. Search for an action name, or use the keyboard/search-by-hotkey control to find a shortcut.
2. Choose **All**, **Assigned**, **Assigned by me**, **Unassigned**, or **Conflicts** to narrow the list. The **Conflicts** count includes local clashes and relevant Obsidian-wide overlaps.
3. Record a new binding with the native shortcut control. K-Plex supports **up to four graph-local shortcuts per action**; you can also remove a binding, explicitly disable an action's local shortcuts, or reset it to the current default.
4. Choose **Physical key** for position-based matching or **Logical key** to match the character your keyboard produces. Physical matching is the starting choice when recording, especially useful for Option/Alt combinations that produce accented characters. Changes save immediately.
5. Use the separate **Publish as an Obsidian command** control to expose or hide a command from Obsidian's Command Palette. For globally active shortcuts, open **Obsidian Settings → Hotkeys** and assign one to that published command.

## Resolve conflicts before relying on keys

- **Red shortcut chips** identify collisions with another K-Plex local action. The relevant action names appear inline; two locally ambiguous bindings run **neither** action until you resolve the conflict.
- Warnings with a **globe** describe a shortcut also used by an Obsidian command. They are advisory and separate from a K-Plex/K-Plex local collision. A same-action published Obsidian binding is informational.
- Some physical-key versus character-key overlaps depend on your keyboard layout and are marked as *possible*.
- K-Plex does **not** delete either conflicting saved assignment automatically. Remove, change or reset one yourself.

## Focus and compatibility

Graph-local shortcuts need a focused K-Plex surface. You can always start with **Ctrl/Cmd+Shift+G** for graph focus or **Ctrl/Cmd+Shift+E** for the associated editor. Choose whether to allow unmodified **character shortcuts** and whether arrows **move across section boundaries**. The editor and native modal inputs keep their own keyboard interaction.

Existing customized shortcuts, explicitly disabled bindings and published-command choices survive plugin updates. Importing graph settings from ExcaliBrain does **not** import its commands or hotkeys. A new default that clashes with your preserved choice can remain unbound until you choose it explicitly.

> [!important] Local and global are different
> A graph-local shortcut is scoped to K-Plex; Obsidian's **Settings → Hotkeys** applies to published commands. Turning off command publication does not remove the local action. Some actions require a selected node or live Plex and will be unavailable without it.

See [[02 Navigate and explore/Keyboard shortcuts reference|Keyboard shortcuts reference]] for examples and [[02 Navigate and explore/K-Plex command palette|K-Plex command palette]] for using the catalog without memorizing keys.

## Local shortcuts and Obsidian command publication

The two settings are deliberately independent:

| Want to… | Configure |
| --- | --- |
| Use a key only while K-Plex owns keyboard focus | A **local shortcut** for an action. |
| Make an action appear in Obsidian's regular Command Palette | **Publish as an Obsidian command** for that action. |
| Trigger a published command from anywhere Obsidian permits | Assign a **global hotkey** under Obsidian's own **Settings → Hotkeys**. |

Removing a local key should **not** silently unpublish the command, and unpublishing should **not** erase a local key assignment. Review the separate warnings when an action overlaps an Obsidian global hotkey.

[Refinement: PR #108](https://github.com/zsviczian/kplex/pull/108).
