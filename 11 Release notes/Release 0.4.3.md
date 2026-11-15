---
aliases:
- K-Plex 0.4.3 release notes
tags:
- kplex-help/release-notes
Note type: ReleaseNotes
Guide:
- '[[Releases 0.4]]'
Previous:
- '[[Release 0.4.2]]'
Next:
- '[[Release 0.4.4]]'
Explains:
- '[[Date properties and daily notes]]'
- '[[Past nodes and pins]]'
- '[[Create notes and placeholders]]'
- '[[How indexing works]]'
- '[[Understanding index status]]'
- '[[Rebuild purge and diagnostics]]'
- '[[Navigating the Plex]]'
Related:
- https://github.com/zsviczian/kplex/releases/tag/0.4.3
- https://github.com/zsviczian/kplex/compare/0.4.2...0.4.3
---
# K-Plex 0.4.3 — Daily notes and a steadier map


Find a day in your journal, bridge a gap between entries, and keep exploring while K-Plex catches up with edits and Sync changes.

released on:: [[2026-11-09]]

Published November 9, 2026. This is a reader-focused summary of the [published release](https://github.com/zsviczian/kplex/releases/tag/0.4.3).

## Jump to a day or connect across a gap

The calendar beside Pins marks days with existing Daily Notes. Select a day to navigate there, or review creation of a missing note using your Obsidian Daily Notes folder, format and template. A matching daily-note placeholder also offers Daily note creation.

Daily-note context menus offer **Connect to previous daily note** and **Connect to next daily note**. They find the nearest existing entry, including notes in nested folders, and open a relationship review rather than writing a connection automatically. See [[Date properties and daily notes]].

## Keep pins compact

The pencil button switches Pins into editing mode to expose reorder handles and remove controls. Drag a pin's body horizontally to scroll; use its handle to reorder. The calendar button can be hidden in Pins settings. See [[Past nodes and pins]].

## Keep working while the index catches up

Warm starts reuse saved index data more reliably. Foreground navigation takes priority over background work, processed files stop re-entering catch-up queues unnecessarily, and ordinary edits cause fewer disruptive changes to the visible map. Date property and Daily Notes configuration changes receive more targeted updates.

Index status distinguishes preparation, pending cache saves and completed work. Diagnostic summaries retain useful history from previous sessions without retaining note contents or filenames. Reports are never submitted automatically. See [[How indexing works]], [[Understanding index status]] and [[Rebuild purge and diagnostics]].

## Reliability and polish

- Templater finishes creating a note before K-Plex adds relationships or opens it; drawing templates benefit from the same waiting behavior.
- Canvas zoom and manual position are preserved more consistently when resizing panes or opening Sidecar.
- Numeric sliders and node-style counts refresh more reliably, while Ontology Manager preserves more of your selection and focus during background updates.
- Deleted notes can remain navigable as placeholders when other notes still reference them.

The living guides explain the current controls, including improvements made after this release.
