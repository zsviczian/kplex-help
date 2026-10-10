---
aliases:
- Sidecar
tags:
- kplex-help/how-to
- kplex/workspace
- kplex/navigation
Friend:
- '[[02 Navigate and explore/Editor node and web pages]]'
Previous:
- '[[05 Personalize and workspace/Images in nodes]]'
Next:
- '[[05 Personalize and workspace/Note-tab synchronization]]'
---
![[Image - Sidecar.png]]

The **Sidecar** is a companion **normal Obsidian document pane** beside K-Plex. You can keep the map visible while reading or editing the note in focus.

- Place the Sidecar to the left, right, above or below the graph.
- Let it follow the current center, fold K-Plex to make room, move the pane, or detach it as an independent tab.
- Continue using normal Obsidian Markdown views and supported plugin-owned file views such as Excalidraw.
- Close K-Plex without automatically closing the note you were reading.

K-Plex does not take over an arbitrary neighboring tab. After an Obsidian restart, it only reconnects when it can identify the appropriate pane; ambiguous layouts are left alone.

**Try it:** With this note centered, open the Sidecar. Navigate to [[05 Personalize and workspace/Images in nodes|Images in nodes]], then edit or read that note while retaining the graph for context.

For a different behavior, see [[05 Personalize and workspace/Note-tab synchronization|Note-tab synchronization]] — that controls pairing with normal note tabs rather than the dedicated Sidecar.

**Shortcuts and focus:** **Ctrl/Cmd+Shift+E** focuses the existing embedded/Sidecar editor, **Ctrl/Cmd+Shift+G** returns focus to the graph, and **Ctrl/Cmd+Enter** centers a selected note while ensuring the Sidecar is open. [[05 Personalize and workspace/Fullscreen and Zen mode|Fullscreen and Zen]] preserve existing context without opening a new graph.

## Keeping the right Excalidraw view

If you explicitly opened a drawing as Markdown (or as its canvas), merely refocusing the same file through a linked Obsidian tab should no longer switch the Sidecar back to another representation. The initial embedded Markdown choice follows Excalidraw's `excalidraw-open-md` preference where applicable.

See [[03 Build and edit/Excalidraw integration|Excalidraw integration]] and [[05 Personalize and workspace/Note-tab synchronization|Note-tab synchronization]].

[Change: PR #112](https://github.com/zsviczian/kplex/pull/112).
