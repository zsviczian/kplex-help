---
tags:
- kplex-help/how-to
- kplex/workspace
- kplex/navigation
Guide:
- '[[05 Personalize and workspace/Personalize and workspace]]'
Related:
- '[[02 Navigate and explore/Navigating the Plex]]'
- '[[05 Personalize and workspace/Sidecar]]'
- '[[05 Personalize and workspace/Layout density and typography]]'
- '[[05 Personalize and workspace/Actions and shortcuts]]'
---
Fullscreen and Zen solve different problems. They are **independent** and can be used together; neither changes note relationships or starts a reindex.

| Mode | What changes | Where |
| --- | --- | --- |
| **Fullscreen** | K-Plex covers the **Obsidian workspace inside its current window**. The existing pane is restored when fullscreen ends. It is **not** the operating system's/browser fullscreen mode. | Desktop only. |
| **Zen mode** | Hides K-Plex's **top toolbar, pins and bottom Past nodes/history**, keeping the graph and its bottom-right controls. | Desktop, tablet and phone. |

## Turn a mode on or off

1. On the bottom-right graph controls, beside **Fit to screen**, choose **Maximize** to enter fullscreen; choose **Minimize** to restore the original layout.
2. Choose **Expand** for Zen; choose **Shrink** to show the toolbars again.
3. You can also find **Toggle fullscreen** and **Toggle Zen mode** in the [[02 Navigate and explore/K-Plex command palette|K-Plex command palette]] or assign custom shortcuts in [[05 Personalize and workspace/Actions and shortcuts|Actions and shortcuts]].

K-Plex keeps the **same graph, camera zoom/pan, selection and navigation history** when toggling either mode. Nothing is automatically fitted; use **Fit to screen** yourself if needed. Bottom-right graph controls remain available in Zen.

## Exiting safely

With graph focus, **Escape** exits Zen **first**, then fullscreen when pressed again, provided no other interface has claimed Escape. An active query, menu, native editor/dialog or connection session has its own Escape priority. Switching to another Obsidian pane or closing the K-Plex view exits fullscreen; closing/unloading the view also cleans up its temporary modes.

Neither state is a saved vault preference. Modes last for **this view session**; reopening the view starts with its normal layout. On a phone or tablet the fullscreen button is unavailable, but Zen still works.

**Try it:** Center a note, pan or zoom slightly, enter Zen, then fullscreen (desktop), and exit both. The camera should be retained throughout; press **Fit to screen** only if you want a new framing.

## Windows and narrow-window controls

Recent control layout refinements keep **fullscreen and Zen buttons clear of Windows' native window controls**, including the maximized Zen editor. In smaller panes, control arrangement adapts to avoid collisions. Fullscreen still covers the owning Obsidian workspace rather than changing the operating system's fullscreen state. Toggling either mode should preserve the current camera and selected note.

[Change: PR #108](https://github.com/zsviczian/kplex/pull/108).
