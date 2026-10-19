---
aliases:
- Create notes and placeholders
tags:
- kplex-help/how-to
- kplex/relationships
- kplex/placeholders
Friend:
- '[[01 Core concepts/Node types]]'
Previous:
- '[[03 Build and edit/Create a relationship]]'
Next:
- '[[03 Build and edit/Drag drop and reclassify]]'
---
A **placeholder** is an unresolved link to an intended note. No file exists yet. It lets you capture a useful relationship before you are ready to write the note.

## Available in 0.1.3

Create a note or placeholder from a relationship gate or an Add parent/child/friend/challenger action. Excalidraw creation is available when its plugin is installed. Later, materialize a placeholder as a real note to develop the idea in the context already established.

When folder nodes are visible, drag outward from a folder's **Child gate** to create a note in that folder. Physical location supplies the folder relationship; K-Plex does not need a redundant note-to-note property to represent it. A web relationship needs a Markdown origin in which to store the link.

## Next release: choose the destination and the next action

Creation and placeholder materialization use a folder selector. Choose the destination deliberately; identical filenames are allowed in different folders, but an existing file at the exact destination is not overwritten.

A placeholder can retain its intended path and a link display alias, for example `[[folder/path/filename|filename]]`. The alias belongs to the referring link, not to frontmatter in a nonexistent file. Materialization retains the calculated destination while letting you review it.

**Control-click** on Windows or **Command-click** on macOS opens a placeholder's creation dialog without moving the originating Plex center. Double-click also provides the normal materialization route.

The **After saving** control states what will happen:

| Choice | Result |
| --- | --- |
| Return | Finish and return without following the new node. |
| Create another | Keep creating related material. |
| Follow node | Make the new node the center. |
| Edit note | Center the new note and open it in the companion Sidecar's normal Markdown editor. |

Folder-child creation produces a real Markdown note or Excalidraw drawing, not a placeholder: an unresolved link has no physical folder membership yet.

## When creation or refresh is still pending

A saved file and a fully refreshed graph are different things. If a file was created but linking or opening did not finish, use the dialog's recovery controls for that existing file rather than creating a duplicate. A saved relationship may offer a targeted refresh while indexing catches up.

Merged improvements also make newly created drawings and external notes discoverable without waiting for all background indexing. They do not mean every relationship is already fully indexed at the instant a file appears.

Sources for next-release behavior: [#168](https://github.com/zsviczian/kplex/pull/168), [#172](https://github.com/zsviczian/kplex/pull/172), [#177](https://github.com/zsviczian/kplex/pull/177), and the [reviewed creation guide](https://github.com/zsviczian/kplex/blob/10760685552fdbafe089a58fc8d80d318853ff31/README.md).
