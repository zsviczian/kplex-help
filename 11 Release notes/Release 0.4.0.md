---
aliases:
- K-Plex 0.4.0 release notes
tags:
- kplex-help/release-notes
Note type: ReleaseNotes
Guide:
- '[[11 Release notes/Releases 0.4]]'
Previous:
- '[[11 Release notes/Release 0.3.1]]'
Next:
- '[[11 Release notes/Release 0.4.1]]'
Explains:
- '[[03 Build and edit/Export and share a canvas]]'
- '[[12 Automation/Automation and scripting]]'
- '[[03 Build and edit/Manage and clean up ontology]]'
- '[[02 Navigate and explore/Navigating the Plex]]'
- '[[02 Navigate and explore/Editor node and web pages]]'
- '[[03 Build and edit/Create notes and placeholders]]'
- '[[01 Core concepts/Canvas views]]'
- '[[07 Use cases/Bring a connected outline into your writing]]'
Related:
- '[[02 Navigate and explore/Vault Search vs Find in this Plex]]'
- '[[05 Personalize and workspace/Note-tab synchronization]]'
---
# K-Plex 0.4.0 — Put your map to work

Take an outline into your writing, share a picture of your thinking, or let a local script explore your notes' relationships. K-Plex 0.4.0 adds export and automation alongside easier ways to open, navigate and edit your maps.

## Share the map you have built

**Export a PNG** from Compass, Mind Map or Facets. Choose **Export image** in the toolbar, **Export → Canvas to image** in the canvas context menu, or **Export canvas as image** in the Command Palette. Preview the whole canvas or just the current viewport, choose 1×, 2× or 3× image scale, and copy or save the result. A transparent background makes the image easier to use in a presentation or document.

Whole-canvas images include content beyond the edge of your current view. Scrolling areas keep their current visible portion, and folded branches stay folded. The preview warns about hidden rows, unavailable media or reduced resolution.

**Export an outline** with **Export → Canvas to MindMap Markdown**. This works in all three views: copy or save the whole constructed map, or select a branch and export that part. Keep the visible ontology labels, include all active labels even when hidden, or leave labels out. Links and cross-links keep the outline connected to your notes. You can use it in Markdown or bring it into Excalidraw's MindMap Builder.

**Export your route** with **Export → Breadcrumbs to Markdown**. This copies the current canvas's Footprints, newest first, including repeated visits.

See [[03 Build and edit/Export and share a canvas|Export and share a canvas]], or try [[07 Use cases/Bring a connected outline into your writing|bringing a connected outline into your writing]].

## Give scripts and assistants the context of your notes

The new public API lets local scripts and plugins read your configured ontology, search indexed nodes, inspect relationships and their sources, and read the context of a particular open canvas. Scripts can also navigate that canvas, switch its view or select a Facets preset.

Use `window.kplexApi.v1` inside Obsidian, or call it through Obsidian CLI from tools such as Codex or Claude. Examples cover finding a research topic, checking why notes connect, and taking an open Mind Map into Markdown. A ready-to-use skill file explains how an assistant can work with the API and interpret incomplete results.

The API works locally. It does not create a web service or send your notes to an AI provider. It reports how complete each result is; reading a partially indexed neighborhood does not silently start a whole-vault indexing pass. Note creation and relationship edits still use Obsidian's normal note and property tools.

Start with [[12 Automation/Automation and scripting|Automation and scripting]].

## Explain what your relationship fields mean

Add an optional **Description** when editing an ontology field. Each member of a pair has its own wording: for example, explain when to use **Guide** separately from **Explains**. Descriptions appear in the manager and suggestions, and scripts can read the same guidance through the API.

This helps you choose a field by its intended use, without renaming properties or changing existing relationships. See [[03 Build and edit/Manage and clean up ontology|Manage and clean up ontology]].

## Open the right map from where you are

Right-click a file in Obsidian's file explorer, its tab, or a resolved file link and use the **K-Plex** submenu. Open it in K-Plex, a new tab, a split to the right, a side panel or a new window. Destinations adapt to your device: tablets omit new windows, and phones offer the side panel.

K-Plex tabs now show the centered file's name with the K-Plex icon, making independent maps easier to tell apart. From a node's **Open** menu, reveal its file in Obsidian's file navigation or your desktop system's file explorer.

Right-click empty canvas space and use **View** to change between Compass, Mind Map and Facets; Facets offers its presets in a submenu. See [[02 Navigate and explore/Navigating the Plex|Navigating the canvas]] and [[01 Core concepts/Canvas views|Choose a canvas view]].

## Create drawings with a familiar starting point

When creating an Excalidraw drawing from a relationship, a folder's Child gate or a placeholder, choose a **Drawing template** from your configured templates. Relative paths distinguish templates with the same name. Choose **Blank drawing** when you want to start fresh.

K-Plex remembers the last successfully used choice across these dialogs and restarts. Cancelling leaves that choice unchanged. See [[03 Build and edit/Create notes and placeholders|Create notes and placeholders]].

## Move and edit with less friction

Enable **Trackpad navigation** under **Settings → K-Plex → Plex behavior → Navigation & interaction** to pan with ordinary scrolling. Pinch, or hold Control on Windows or Command on macOS while scrolling, to zoom around the pointer. The default remains wheel-to-zoom. Native editors and lists keep their normal scrolling.

Node editors open consistently across all three views, including Mind Map roots. Hold Alt on Windows or Option on macOS while opening a node editor to open it maximized. Titles and recovery controls remain reachable when an editor is large or panned, and images, audio and video use Obsidian's native viewers. An unpinned, ungrouped File properties pane follows the open node editor, then returns to the map's root or center when it closes.

K-Plex also remembers more of a note's view state when you revisit it during the session. Passive document following reuses existing panes. Mobile Rename keeps its controls within reach of the on-screen keyboard.

## A clearer, steadier canvas

Dense maps handle camera movement with less redraw work. Connectors to rows hidden inside scrolling areas no longer collect at the area boundary; scrolling the rows back into view restores their connections. Vault Search does less work to find its best matches, and result rows use a lighter appearance.

Other fixes preserve attachment backlinks and local gate counts, recognize web links with escaped or balanced brackets in their labels, and keep connection-focus dimming consistent while arriving at a new center.
