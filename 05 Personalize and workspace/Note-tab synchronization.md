---
aliases:
- Note-tab synchronization
tags:
- kplex-help/reference
- kplex/workspace
- kplex/navigation
Friend:
- '[[02 Navigate and explore/Past nodes and pins]]'
- '[[02 Navigate and explore/Footprints and breadcrumbs]]'
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

## Next release: independent Plex views and document pairs

The toolbar **+** and **New K-Plex tab** command open another Plex in an adjacent tab group. Each view keeps its own center representation and Markdown reading/editing choice, including workspace restoration. Nodes can be dragged between views.

**Merged [PR #187](https://github.com/zsviczian/kplex/pull/187)** adds independent **Off, Recent and Pinned** document-sync intent and targets for each native Plex. Two Plexes can now follow different note tabs or own separate Sidecars. Switching one view's sync mode does not silently replace another view's pairing. Recent does not take over a companion Sidecar owned by another Plex. Obsidian's workspace restores the individual pairs when their saved native targets are available; duplicated Plex views start with fresh ownership rather than inheriting a live claim.

**Pins and saved Past nodes history stay global and persisted** across Plexes. By contrast, [[02 Navigate and explore/Footprints and breadcrumbs|Footprints (session breadcrumbs)]] is **owned by each Plex** and keeps every accepted visit, including repetitions, **in memory only**. Its trail stays with that Plex across window moves and is cleared when the Plex closes or Obsidian restarts.

Footprints is a visit list, not an automatically branching or metro-map navigation diagram. Copy it explicitly as Markdown if you want to retain the exploration in a note.

## Next release: edit properties in context

An open, unpinned and ungrouped Obsidian **File properties** pane follows the central file while K-Plex is active. Pinned or grouped Properties panes retain their own file. A folder, tag or other non-file center clears the unpinned pane instead of leaving unrelated metadata on display.

This supports [[07 Use cases/Garden your vault]] without making the Properties pane a second note editor or changing how ordinary note tabs are linked.

Sources: [earlier Excalidraw behavior #112](https://github.com/zsviczian/kplex/pull/112), [File properties #171](https://github.com/zsviczian/kplex/pull/171), [additional Plex views #177](https://github.com/zsviczian/kplex/pull/177), [independent sessions and Footprints #187](https://github.com/zsviczian/kplex/pull/187). Status reviewed October 19, 2026; see [[00 Start Here/Recently added features]].
