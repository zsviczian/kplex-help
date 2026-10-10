---
aliases:
- Navigating the Plex
tags:
- kplex-help/how-to
- kplex/navigation
Friend:
- '[[01 Core concepts/The spatial relationship model]]'
Next:
- '[[02 Navigate and explore/Vault Search vs Find in this Plex]]'
---
- **Single-click / tap** a node to make it the center.
- **Double-click** a file-backed node to open it in Obsidian.
- Double-click a URL to open it in the browser.
- Double-click an unresolved link to create the missing Markdown note.
- Drag empty graph space to pan; use the wheel or pinch to zoom.
- Right-click or long-press for context menus.
- Click empty graph space to clear temporary highlights.
- Use **Fit graph** to bring the visible Plex back into view.

K-Plex animates navigation so nodes shared by the old and new scene visibly move to their new semantic position. Animation speed is configurable under **Plex behavior** and can be disabled.

> [!practice]
> Center [[00 Start Here/K-Plex Help|K-Plex Help]], then click this note, [[02 Navigate and explore/Vault Search vs Find in this Plex|Vault Search vs Find in this Plex]], and back. Watch how shared nodes move rather than being redrawn as unrelated points.

## Prefer the keyboard?

[[02 Navigate and explore/Keyboard navigation|Keyboard navigation]] covers graph focus, selecting nodes with arrows and switching areas; [[02 Navigate and explore/Type to select visible nodes|Type to select visible nodes]] jumps to displayed labels. The [[02 Navigate and explore/K-Plex command palette|K-Plex command palette]] makes graph actions searchable. For an uncluttered workspace, use [[05 Personalize and workspace/Fullscreen and Zen mode|Fullscreen and Zen mode]].

## Interpreting relationship counts

The small number beside a directional gate is a relationship count, not the number of line segments drawn. A correction in the current K-Plex keeps **filtered gate badges** aligned with the actual semantic endpoints, including relationships displayed on different connector sides. Partial counts can still be marked while source data is loading.

For each connector's underlying sources, open [[03 Build and edit/Connection details and evidence|Connection details and evidence]].

[Correction: PR #112](https://github.com/zsviczian/kplex/pull/112).
