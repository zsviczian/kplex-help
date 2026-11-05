---
aliases:
- Create notes and placeholders
tags:
- kplex-help/how-to
- kplex/relationships
- kplex/placeholders
Friend:
- '[[Node types]]'
Previous:
- '[[Create a relationship]]'
Next:
- '[[Drag drop and reclassify]]'
---
# Create notes and placeholders

Capture an idea before you lose it. Create a note now, or add a placeholder so you can connect the idea first and write it later.

![[Screenshot - Choose a folder.png]]

*The folder input searches parts of an existing path and shows the matching folder across the available width.*

## Try it

Create a note or placeholder from a relationship gate or an Add parent/child/friend/challenger action. Excalidraw creation is available when its plugin is installed. Later, materialize a placeholder as a real note to develop the idea in the context already established.

When folder nodes are visible, drag outward from a folder's **Child gate** into empty canvas space. Choose **Create note** or **Create subfolder**; K-Plex remembers the last tab. Enter a name, then create it in that folder. Physical location supplies the folder relationship; K-Plex does not need a redundant note-to-note property to represent it. A web relationship needs a Markdown origin in which to store the link.

## Choose the destination and the next action

Creation and placeholder materialization use a folder selector. Choose the destination deliberately; identical filenames are allowed in different folders, but an existing file at the exact destination is not overwritten.

A placeholder can retain its intended path and a link display alias, for example `[[folder/path/filename|filename]]`. The alias belongs to the referring link, not to frontmatter in a nonexistent file. Materialization retains the calculated destination while letting you review it.

**Control-click** on Windows or **Command-click** on macOS opens a placeholder's creation dialog without moving the originating canvas center. Double-click also provides the normal materialization route.

The **After saving** control states what will happen:

| Choice | Result |
| --- | --- |
| Return | Finish and return without following the new node. |
| Create another | Keep creating related material. |
| Follow node | Make the new node the center. |
| Edit in sidecar | Center the note and open it in the adjacent Sidecar. |
| Edit in editor view | Center the note and open its editor inside K-Plex. |
| Edit in editor view maximized | Open that editor maximized. |
| Open in new tab | Open the file in a native Obsidian tab. |
| Open in popout window | Open a separate desktop window. |

K-Plex remembers one After saving choice for **creation** and another for **linking existing notes or web links**. Switching between those tasks restores the appropriate choice. Destinations adapt to the target and device: web links do not offer note editors, popouts are desktop-only, and a canvas in a side panel does not offer Sidecar. Placeholder materialization omits Create another and Follow node.

Folder-child creation produces a real Markdown note or Excalidraw drawing, not a placeholder: an unresolved link has no physical folder membership yet.

## Start a drawing from a template

When creating an Excalidraw drawing, choose **Drawing template** in the related-note composer, folder-child dialog or placeholder creation dialog. Choices come from the template file or folder configured in Excalidraw. Folder entries show relative paths so templates with the same name are distinguishable. **Blank drawing** explicitly starts without a template.

K-Plex remembers the last selection after a drawing is successfully created. The choice is shared across these dialogs and survives restarts; cancelling does not change it. With no previous choice, the first configured template is selected. If a remembered template has disappeared, the first available template is used. A remembered **Blank drawing** choice stays blank.

For example, configure planning and sketch templates in Excalidraw. Create a related drawing using the planning template, then open a folder-child drawing dialog: the planning choice is ready to reuse. Choose Blank drawing when the next idea needs a fresh page.

## When creation or refresh is still pending

A saved file and a fully refreshed graph are different things. If a file was created but linking or opening did not finish, use the dialog's recovery controls for that existing file rather than creating a duplicate. A saved relationship may offer a targeted refresh while indexing catches up.

Newly created notes and drawings can become searchable while wider indexing continues. Their full relationships may still be loading.

## Let templates finish before linking

If Templater applies a folder or file-creation template, K-Plex waits for that processing before adding aliases, display names or relationship properties to the new note. This also matters when the new note will own a reversed relationship. The dialog can show **Waiting for the note template to finish…** while template commands run.

Use the normal creation recovery flow if template processing fails; check the actual saved file before trying again. A template command that depends on whichever editor currently has focus can target a different pane when a note opens in Sidecar. Such automation should target the created file or its specific view.
