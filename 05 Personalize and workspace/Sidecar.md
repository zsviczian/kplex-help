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

The **Sidecar** is a companion **normal Obsidian document pane** beside K-Plex. Keep the map visible while reading or editing the note in focus.

## Available in 0.1.3

Place the Sidecar left, right, above or below the graph. It can follow the center, use normal Markdown views or supported plugin-owned file views such as Excalidraw, and be detached as an independent tab. Closing K-Plex does not automatically close the document you were reading.

Sidecar controls can attach an eligible adjacent document pane, send the current graph note to the Sidecar, or bring its document into the Plex. Deliberate attachment is different from silently taking over an arbitrary neighboring tab. On restart, K-Plex reconnects only when it can identify the appropriate restored pane; ambiguous layouts are left alone.

The Sidecar control stays on its chosen edge after closing the companion, so you can reopen it there. Try opening it with this note centered, then navigate to [[05 Personalize and workspace/Images in nodes]].

**Focus shortcuts:** Control+Shift+E on Windows or Command+Shift+E on macOS focuses the existing embedded/Sidecar editor; the corresponding Shift+G chord returns to the graph. Control+Enter / Command+Enter centers the selected note and ensures its Sidecar is open. Saved action bindings can override defaults; see [[05 Personalize and workspace/Actions and shortcuts]].

## Next release: fold the entire Plex tab group safely

**Fold K-Plex tab group** temporarily hides the complete group containing the graph—including any other tabs in that group—while keeping those tabs open. It gives the paired Sidecar group more room; it does not merely collapse the K-Plex tab's content.

Use **Unfold K-Plex tab group** on the surviving group's edge, or repeat the fold command, to restore it. The recovery control remains available when you select another tab in the Sidecar group.

Closing the exact managed Sidecar restores the folded group while leaving unrelated tabs open. Closing an unrelated sibling tab does not end the fold. Activating a tab in the hidden group reveals it and respects that selection. Fullscreen restores a folded group first; leaving fullscreen does not fold it again.

If several pairs could be targeted, the command uses a picker. Layouts that cannot preserve unrelated panes remain expanded. Folding does not depend on which graph node is central or on indexing being complete.

## Keep the chosen Excalidraw representation

Passive synchronization of the same drawing preserves an intentional Markdown or drawing view. Explicit opening commands can still change representation. The initial embedded choice follows Excalidraw's `excalidraw-open-md` preference where applicable.

**Next release:** Ordinary Markdown autosaves retain an equivalent graph layout instead of temporarily reclassifying relationships or replaying navigation animation. Genuine content or relationship changes can still update the graph.

Several Plex views do not yet guarantee independent companion-sync pairs. See [[05 Personalize and workspace/Note-tab synchronization]] for that boundary.

Related guides: [[03 Build and edit/Excalidraw integration]] and [[05 Personalize and workspace/Fullscreen and Zen mode]]. Sources: [release 0.1.3](https://github.com/zsviczian/kplex/releases/tag/0.1.3), [folding #173](https://github.com/zsviczian/kplex/pull/173), [autosave continuity #180](https://github.com/zsviczian/kplex/pull/180), [earlier representation fix #112](https://github.com/zsviczian/kplex/pull/112).
