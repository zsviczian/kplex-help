---
aliases:
- Editor node and web pages
tags:
- kplex-help/how-to
- kplex/navigation
- kplex/web
Friend:
- '[[05 Personalize and workspace/Sidecar]]'
Previous:
- '[[02 Navigate and explore/Past nodes and pins]]'
Next:
- '[[02 Navigate and explore/Mobile and touch]]'
---
# Editor node and web pages

Read a note or website without losing the ideas around it. Open it inside the canvas and keep the surrounding map visible.

![[Assets/Screenshot - Read inside the center.png]]

*Reading view expands the document inside the central node; its surrounding connections remain part of the map.*

Images fit both dimensions without cropping. The editor's **Open menu** exposes the same opening destinations as the normal node context menu. Maximizing the editor temporarily hides local Find and preserves its query.

On desktop, websites use a webview with normal browser authentication behavior. On Obsidian mobile, websites use an iframe. YouTube and Vimeo links use embedded players; YouTube Shorts use a portrait frame.

> [!privacy]
> Expanding a website loads that site. It receives normal browser requests and may store its own cookies.

Try the URL friend attached to [[08 About/Community GitHub and contributing|Community GitHub and contributing]] once URL nodes are visible.

**Keyboard focus:** **Ctrl/Cmd+Shift+E** focuses an existing editor associated with K-Plex; **Ctrl/Cmd+Shift+G** returns keyboard focus to the graph. In the editor, **Ctrl/Cmd+F** remains native Find rather than K-Plex Find. Read [[02 Navigate and explore/Keyboard navigation|Keyboard navigation]] for details.

## Edit a note where it belongs

Eligible Markdown notes expose a node-editor corner action. In Compass and Mind Map, a neighboring note can open in place without moving the focus of the map. Facets keeps its editor attached to the current focus. There is one node editor at a time; opening another saves and closes the first. A failed save leaves the existing editor available for recovery.

Switching the canvas view also saves and closes the existing node editor first. In Mind Map, close it before changing the root or folding away its branch. Use the normal document pane or Sidecar when you want to read other files beside the canvas.

Alt/Option-select **Use editor as central node** to open directly in expanded editor mode. The regular action retains its normal behavior.
