---
aliases:
- K-Plex 0.4.2 release notes
tags:
- kplex-help/release-notes
Note type: ReleaseNotes
Guide:
- '[[11 Release notes/Releases 0.4]]'
Previous:
- '[[11 Release notes/Release 0.4.1]]'
Explains:
- '[[03 Build and edit/Create notes and placeholders]]'
- '[[03 Build and edit/Drag drop and reclassify]]'
- '[[03 Build and edit/Connection details and evidence]]'
- '[[02 Navigate and explore/Past nodes and pins]]'
- '[[04 Filter and focus/Define a Facets workflow]]'
- '[[01 Core concepts/The spatial relationship model]]'
- '[[03 Build and edit/Manage and clean up ontology]]'
- '[[12 Automation/K-Plex API examples]]'
- '[[02 Navigate and explore/Navigating the Plex]]'
- '[[05 Personalize and workspace/Sidecar]]'
- '[[06 Indexing and troubleshooting/How indexing works]]'
Related:
- https://github.com/zsviczian/kplex/releases/tag/0.4.2
- https://github.com/zsviczian/kplex/compare/0.4.1...0.4.2
---
# K-Plex 0.4.2 — Create, organize and return to your work

Capture notes in the right folder, bring outside material into your map, and keep today's work one click away. K-Plex 0.4.2 adds folder workflows, periodic pins and more control over relationships, alongside steadier indexing during Obsidian Sync.

Published November 5, 2026. This page summarizes the [published release](https://github.com/zsviczian/kplex/releases/tag/0.4.2); the guides below explain how to use the changes.

## Create and organize without leaving the map

Drag from a folder's Child gate into empty canvas space to **Create note** or **Create subfolder**. The dialog remembers the tab you last used. Choose **Move…** on a real file or folder's node to change its location; Obsidian applies its normal link-maintenance settings.

Drag a folder from Obsidian Files onto the center to explore it, or use its **Open in K-Plex** context-menu action. Bring files or whole folders from your computer onto a supported note or folder: review one destination and, for a note target, one editable relationship choice for the batch. Originals stay on your computer.

**After saving** remembers separate choices for creating notes and linking existing notes or web links. Newly created notes wait for Templater's creation processing before K-Plex adds relationship properties. Today's pin also uses the core Daily Notes template when configured.

See [[03 Build and edit/Create notes and placeholders|Create notes and placeholders]] and [[03 Build and edit/Drag drop and reclassify|Drag, drop and organize]].

## Make the relationship you intend

The gate where your drag starts supplies the relationship direction, even when you drop onto a different gate. K-Plex remembers the last ontology separately within each direction. Hold a modifier while dragging from a Friend or Challenger gate to start a Previous or Next connection.

In **Connection details**, edit the selected ontology or use **Flip owner** on an eligible property source. A before-and-after preview shows which note will contain the property; save to move that selected declaration while keeping other properties and Markdown links. Ontology selectors show descriptions beneath names and let you edit or create fields from the same workflow.

See [[03 Build and edit/Connection details and evidence|Connection details and evidence]].

## Keep today's work within reach

Enable **Today**, **This week** or **This month** under **Canvas behavior → Pins**. They follow this device's date. Today can use the folder, date format and template already configured in Obsidian Daily Notes. A missing note opens a creation confirmation; choose whether to return, edit in the Sidecar, or use another offered destination. K-Plex remembers that opening choice.

Drag pins into your preferred order, or use **Move left** and **Move right** in their menus. A drop marker makes the destination visible, and the order is shared across canvases.

See [[02 Navigate and explore/Past nodes and pins|Past nodes and pins]].

## Choose how your map reads

Each Facets preset has two independent options: **Display active note in matching container** puts the focus note in its matching category as a larger card; **Hide gates, connect links from node centers** draws a simpler view without gates. Save either or both per preset.

Compass adds **Flip East–West axis**. Friends and Previous move to the right; Challengers and Next move to the left. Relationship meanings stay the same.

See [[04 Filter and focus/Define a Facets workflow|Define a Facets workflow]] and [[01 Core concepts/The spatial relationship model|The spatial relationship model]].

## Find the right word for a connection

Ontology suggestions also search field descriptions, so an alternative term can help you find the canonical field name. Scripts and local assistants can look up documents using a field, inspect its exact occurrences in selected notes, and preview reviewed changes to ontology definitions, descriptions and inverse pairs. These operations distinguish changing configuration from editing note text.

An ontology-completion API also lets integrations offer K-Plex's configured vocabulary without waiting for graph indexing. Start with [[03 Build and edit/Manage and clean up ontology|Manage and clean up ontology]] or [[12 Automation/K-Plex API examples|the API examples]].

## Navigate with fewer interruptions

- **Obsidian URI links** are indexed and searchable; opening an `obsidian://` link uses Obsidian's own handling.
- **Readable web-link labels** in frontmatter survive indexing and cache reloads.
- **Copy link** follows Obsidian's link-format and path preferences. Opening a section targets its own file and heading more reliably.
- **Visibility settings** offer bulk enable/disable actions where available.
- **Page Preview** follows one K-Plex preference across tabs, sidebars and popout windows.
- **Sidecar attachment arrows** appear for the visible neighboring tab even when another tab in that group is the attached Sidecar. An empty tab offers only the center-to-pane action; the active Sidecar itself needs neither arrow.

Dialogs and settings use more consistent Obsidian controls, spacing and icon buttons. See [[02 Navigate and explore/Navigating the Plex|Navigating the canvas]] and [[05 Personalize and workspace/Sidecar|Sidecar]].

## Keep working during Sync and recovery

Compatible cached graphs can be shown while changes received through Obsidian Sync are checked. Recovery does less repeated cache reading, and local relationship changes can become available before wider validation finishes. Progress and diagnostic details give more information when preparation takes time.

See [[06 Indexing and troubleshooting/How indexing works|How indexing works]]. The [full changelog](https://github.com/zsviczian/kplex/compare/0.4.1...0.4.2) records the individual changes and contributors.
