---
aliases:
- Editor node and web pages
tags:
- kplex-help/how-to
- kplex/navigation
- kplex/web
Friend:
- '[[Sidecar]]'
Previous:
- '[[Past nodes and pins]]'
Next:
- '[[Mobile and touch]]'
---
# Editor node and web pages

Read a note or website without losing the ideas around it. Open it inside the canvas and keep the surrounding map visible.

![[Screenshot - Read inside the center.png]]

*Reading view expands the document inside the central node; its surrounding connections remain part of the map.*

Images fit both dimensions without cropping. The editor's **Open menu** exposes the same opening destinations as the normal node context menu. Maximizing the editor temporarily hides local Find and preserves its query.

On desktop, websites use a webview with normal browser authentication behavior. On Obsidian mobile, websites use an iframe. YouTube and Vimeo links use embedded players; YouTube Shorts use a portrait frame.

> [!privacy]
> Expanding a website loads that site. It receives normal browser requests and may store its own cookies.

Try the URL friend attached to [[Community GitHub and contributing|Community GitHub and contributing]] once URL nodes are visible.

**Keyboard focus:** **Ctrl/Cmd+Shift+E** focuses an existing editor associated with K-Plex; **Ctrl/Cmd+Shift+G** returns keyboard focus to the graph. In the editor, **Ctrl/Cmd+F** remains native Find rather than K-Plex Find. Read [[Keyboard navigation|Keyboard navigation]] for details.

## Edit a note where it belongs

Eligible Markdown notes expose a node-editor corner action. In Compass, Mind Map and Facets, a neighboring note opens in place without moving the focus of the map. In Facets it stays in its category. There is one node editor at a time; opening another saves and closes the first. A failed save leaves the existing editor available for recovery.

The containing area grows temporarily in width and height to fit the complete editor, including its controls. Opening or resizing reveals it within a scrollable area; ordinary scrolling afterward remains yours. Closing the editor restores the configured area dimensions. This does not change your saved area settings or the note's category.

Switching the canvas view also saves and closes the existing node editor first. In Mind Map, when the central note is open in the editor, clicking another Markdown note saves the previous note and opens the new center in the same reading or editing mode and dimensions. A failed save keeps the current editor available. Close an editor before folding away its branch. Use the normal document pane or Sidecar when you want to read other files beside the canvas.

Hold **Alt** on Windows or **Option** on macOS while selecting a node-editor corner action or **Use editor as central node** to open it maximized. This works for Mind Map roots as well as neighboring nodes. The regular action retains its normal behavior.

## Keep the document and its controls within reach

The editor title stays on one line while the document scrolls independently. Large or panned editors keep recovery controls reachable, including collapse and minimize. Maximizing keeps the same native document open; it does not replace your editor with a copy.

Images, audio and video use Obsidian's native file viewers inside the node editor. An unpinned, ungrouped **File properties** pane follows the file in the open node editor, including a neighbor that is not the map center. Closing the editor returns Properties to the current map root or center. Pinned or grouped Properties panes retain their own target.

When you revisit a note in a canvas view, K-Plex can restore its reading/editing and editor view state during the current session. This temporary memory is bounded and is not a permanent bookmark or a copy of the note's contents.
