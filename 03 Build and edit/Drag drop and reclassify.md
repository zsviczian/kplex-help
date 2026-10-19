---
aliases:
- Drag drop and reclassify
- Move files and assign tags from the graph
tags:
- kplex-help/how-to
- kplex/relationships
- kplex/interaction
Friend:
- '[[02 Navigate and explore/Past nodes and pins]]'
- '[[07 Use cases/Build a Map of Content]]'
- '[[07 Use cases/Garden your vault]]'
Previous:
- '[[03 Build and edit/Create notes and placeholders]]'
Next:
- '[[03 Build and edit/Connection details and evidence]]'
---
K-Plex uses drag-and-drop to navigate, create relationships and reorganize knowledge. Some drops change note properties or physically move files; they are not just visual rearrangements.

## Available in 0.1.3

Drag a file from Obsidian's file explorer onto the central node to navigate to it, or into a Parent, Friend, Challenger or Child area to open the linking dialog with that role selected. Drag an existing direct neighbor to another relationship area to reclassify it. Drag a gate to a pin or Past nodes entry to create that gate's relationship.

Valid drop areas light up. After reclassifying a connection with several sources, inspect [[03 Build and edit/Connection details and evidence|Connection details]] rather than assuming every source has changed.

## Next release: bring notes into and out of the Plex

Resolved note links from **Bases** use the same center/relationship-area destinations as file-explorer notes. Dropping a sibling into a relationship area adds a direct relationship to the center without removing its shared parent or other relationships.

Drag a note, attachment, URL or placeholder **node body** into a Markdown editor to insert its link. Tags insert `#tag` text. Drag supported nodes into another Plex to navigate or start a relationship there. Gates retain their connection gestures.

Use the toolbar **+** or **New K-Plex tab** to open an adjacent Plex. Its central editor/normal-node choice and Markdown mode belong to that view. Document synchronization is not yet fully isolated between views; see [[05 Personalize and workspace/Note-tab synchronization]].

## Next release: move files into folders

Drag a file or folder's **gate** onto a folder to move it there. With a folder in the center, you can also drag its gate onto a file or attachment to bring that item into the folder.

Review the source and destination in the confirmation. Holding **Alt** on Windows or **Option** on macOS bypasses that confirmation, not collision or folder-ancestry checks. Obsidian updates links according to its file settings.

A folder's Child gate dragged into empty space still creates a note inside that folder. Folder membership is physical location: it does not offer an Unlink or Hidden action that would pretend to remove the relationship without moving the file.

## Next release: assign a tag or Note Type

Drag a Markdown note onto a tag in history or pins to add it to the note's `tags` property. A tag's gate can also be dropped onto a Markdown note in the Plex, history or pins. A tag from another Plex can be dropped into a note's Parents area.

Where offered, choose **Tag** or **Note Type**. A Note Type keeps the tag in the YAML `tags` list and also uses the configured Style property. A note has one Note Type; replacing an existing type requires an explicit choice, with the other remaining an ordinary tag.

Tag connector menus can change between ordinary Tag and Note Type. Editable YAML membership can be removed; inline tag evidence remains inspectable rather than being silently rewritten. Note Type links are twice the ordinary tag-link width by default and have a separate styling control.

These are merged improvements, not features of the published 0.1.3 bundle. Sources: [#171](https://github.com/zsviczian/kplex/pull/171), [#177](https://github.com/zsviczian/kplex/pull/177), and the [reviewed navigation and editing guide](https://github.com/zsviczian/kplex/blob/10760685552fdbafe089a58fc8d80d318853ff31/README.md#search-history-and-pins).
