---
aliases:
tags:
  - kplex-help/release-notes
Guide:
  - "[[11 Release notes/Release notes]]"
Explains:
  - "[[04 Filter and focus/Group nodes by note type]]"
  - "[[04 Filter and focus/Graph Lenses]]"
Previous:
  - "[[Release 0.2.0]]"
Next:
  - "[[Release 0.2.3]]"
Related:
  - https://github.com/zsviczian/kplex/releases/tag/0.2.2
  - https://github.com/zsviczian/kplex/pull/199
  - https://github.com/zsviczian/kplex/pull/200
Note type: ReleaseNotes
---
# K-Plex 0.2.2 — A clearer map, easier styling

Get an overview of a busy neighborhood before opening its individual notes. Fixed Graph Lens style editor bug where color editor appeared behind the lens settings.

Published **2026-10-21**. This is a reader-facing summary of [the published 0.2.2 release](https://github.com/zsviczian/kplex/releases/tag/0.2.2).

## Open the detail you need

The new **Group nodes by note type** toggle sits beside **Expanded view** in the toolbar. Related Markdown notes with the same note type become one named, styled group; attachments, links, placeholder notes, tags and folders form their own groups. A small number outside each group shows its item count. Single items stay visible individually.

Select a group to unfold it without leaving the current center. Keep other groups compact, navigate to another note to start grouped again, or turn grouping off to reveal every group member. Parents and Children group separately; One-sided layout groups the shared lateral area together.

This is a way to explore the current map without rewriting your notes or their relationships. See [[04 Filter and focus/Group nodes by note type|how to group a busy neighborhood]].

![[Assets/Screenshot - Grouped workshop relations.png]]

*A desktop workshop example shows the new grouping toggle, note-type colors and member counts. Open one group when you need its individual notes.*

## Choose lens colors without moving panels aside

When editing a **Style matching** Graph Lens, the fill, border and text color editors now open in front of **Filters and lenses**. You can reach the color controls directly, including the theme-color chooser, without dragging the lens panel out of the way.

See [[04 Filter and focus/Graph Lenses|Graph Lenses]] for reusable views and styling rules.

## About 0.2.1

0.2.1 was a technical republication following a release hiccup. It has no separate user-facing release-note page; [[Release 0.2.0|the 0.2.0 notes]] describe that update's features.

## Sources

- [Grouping by note type and kind — PR #199](https://github.com/zsviczian/kplex/pull/199)
- [Lens color editors above the filter panel — PR #200](https://github.com/zsviczian/kplex/pull/200)
