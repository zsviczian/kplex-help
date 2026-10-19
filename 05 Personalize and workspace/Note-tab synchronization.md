---
aliases:
- Note-tab synchronization
tags:
- kplex-help/reference
- kplex/workspace
- kplex/navigation
Friend:
- '[[02 Navigate and explore/Past nodes and pins]]'
Previous:
- '[[05 Personalize and workspace/Sidecar]]'
Next:
- '[[05 Personalize and workspace/Visibility and connector styling]]'
---
K-Plex and normal note tabs can be paired in three modes:

- **Independent** — graph navigation and note-tab navigation do not drive each other.
- **Most recent note tab** — K-Plex links to the most recently used note tab.
- **Pinned to one fixed note tab** — K-Plex stays paired with a specific note tab.

One-shot commands can send the current graph note to the recent tab or bring the recent tab into K-Plex. **Show linked/pinned tab** activates the actual connected tab and briefly outlines its pane so you can identify it. These controls live in the K-Plex toolbar, rather than being duplicated in Settings.

## Keep a reference while exploring

Use a fixed reference tab or independent navigation when a draft should stay open while you investigate other notes. Use a following Sidecar when the document should change with the central node. These are different intentions; linking every open pane is rarely helpful.

Passive same-file synchronization preserves an Excalidraw note's chosen drawing or Markdown representation. An explicit open command or drawing/Markdown toggle can still change it; navigation to another file follows the chosen sync behavior.

## Next release: more Plex views, with an important boundary

The toolbar **+** and **New K-Plex tab** command open another Plex in an adjacent tab group. Each view keeps its own center representation and Markdown reading/editing choice, including workspace restoration. Nodes can be dragged between views.

However, the reviewed main still shares document-sync mode/target state. Do not assume that two Plexes can safely operate as two fully independent following Sidecar pairs. **Pins and saved navigation history are global and persisted**, not separate per-view collections.

Independent document synchronization and a nonpersisted per-view **Footprints** list are proposed in [PR #187](https://github.com/zsviczian/kplex/pull/187). They are not implemented in the reviewed baseline. Footprints is not the same as a future branching or metro-map visualization.

## Next release: edit properties in context

An open, unpinned and ungrouped Obsidian **File properties** pane follows the central file while K-Plex is active. Pinned or grouped Properties panes retain their own file. A folder, tag or other non-file center clears the unpinned pane instead of leaving unrelated metadata on display.

This supports [[07 Use cases/Garden your vault]] without making the Properties pane a second note editor or changing how ordinary note tabs are linked.

Sources: [earlier Excalidraw behavior #112](https://github.com/zsviczian/kplex/pull/112), [File properties #171](https://github.com/zsviczian/kplex/pull/171), [additional Plex views #177](https://github.com/zsviczian/kplex/pull/177). Status reviewed October 19, 2026; see [[00 Start Here/Recently added features]].
