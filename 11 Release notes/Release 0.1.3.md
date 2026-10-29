---
aliases:
tags:
  - kplex-help/release-notes
  - kplex/released
Guide:
  - "[[11 Release notes/Release notes]]"
Previous:
  - "[[Release 0.1.2]]"
Next:
  - "[[Release 0.2.0]]"
Explains:
  - "[[02 Navigate and explore/Wander]]"
  - "[[05 Personalize and workspace/Sidecar]]"
  - "[[05 Personalize and workspace/Fullscreen and Zen mode]]"
  - "[[05 Personalize and workspace/Images in nodes]]"
Related:
  - https://community.sketch-your-mind.com/
  - https://github.com/zsviczian/kplex
  - https://github.com/zsviczian/kplex/compare/0.1.2...0.1.3
  - https://github.com/zsviczian/kplex/pull/120
  - https://github.com/zsviczian/kplex/pull/121
  - https://github.com/zsviczian/kplex/pull/122
  - https://github.com/zsviczian/kplex/pull/123
  - https://github.com/zsviczian/kplex/pull/136
  - https://github.com/zsviczian/kplex/pull/137
  - https://github.com/zsviczian/kplex/pull/138
  - https://github.com/zsviczian/kplex/pull/139
  - https://github.com/zsviczian/kplex/pull/140
  - https://github.com/zsviczian/kplex/pull/141
  - https://github.com/zsviczian/kplex/pull/142
  - https://github.com/zsviczian/kplex/pull/146
  - https://github.com/zsviczian/kplex/pull/152
  - https://github.com/zsviczian/kplex/releases/tag/0.1.3
  - https://img.youtube.com/vi/ii15UwpsvtU/maxresdefault.jpg
  - https://ko-fi.com/zsolt
  - https://www.youtube.com/watch?v=ii15UwpsvtU
Note type: ReleaseNotes
---
# K-Plex 0.1.3 — release notes

Checking what changed in this version? Read the published notes below, or follow the guide links for current instructions.

**Published:** 2026-10-13 · [Original GitHub release](https://github.com/zsviczian/kplex/releases/tag/0.1.3)

## Explore these changes in K-Plex Help

- [[02 Navigate and explore/Wander]]
- [[05 Personalize and workspace/Sidecar]]
- [[05 Personalize and workspace/Fullscreen and Zen mode]]
- [[05 Personalize and workspace/Images in nodes]]

## Original published release notes

> [!note] Historical record
> The text below comes from the published GitHub release, not a retrospective reconstruction. See the release archive for links to current guides; older announcements describe their original published state.

This release brings a new way to explore your knowledge graph, smoother navigation, better Sidecar integration, and a collection of fixes that make K-Plex more reliable and enjoyable to use.

[![Watch the video](https://img.youtube.com/vi/ii15UwpsvtU/maxresdefault.jpg)](https://www.youtube.com/watch?v=ii15UwpsvtU)


## ✨ What's New

### 🚶 Wander — Explore Your Knowledge Graph

Introducing **Wander**, a new way to explore your knowledge graph.

Instead of deciding where to go next, let K-Plex take you on a journey through connected notes. Discover connections, revisit forgotten ideas, and see where your knowledge leads you.

Wander includes dedicated controls and smooth transitions as you move between notes.

### 🔗 Smarter Sidecar Integration

Working with K-Plex alongside your notes is now more intuitive.

* **Attach an existing adjacent pane as your Sidecar** using the new directional controls.

* Open the central K-Plex note in your Sidecar, or bring the Sidecar's note into the center of K-Plex.

* Switching between notes no longer causes duplicate Sidecar openings.

* Rapid navigation now reliably follows your latest selection rather than jumping back to an earlier note.

* Improved Sidecar layout and behavior when reopening panels.

### 🎯 Smoother Navigation and Better Automatic Fitting

K-Plex now does a better job keeping your graph in view as you explore.

* Smoother visual transitions when navigating between nodes.

* The central node stays centered as surrounding connections appear during background indexing.

* Manual zooming and panning take priority over automatic fitting.

* Embedded Excalidraw drawings automatically adjust to their available space when appropriate.

### 🎨 More Control Over Your Workspace

The graph background context menu now provides quick access to useful actions:

* Open K-Plex settings.

* Switch to Zen or full-screen mode.

* Customize the graph background color.

* Report a bug.

Tooltips have also been refined for better readability, including controls near the bottom of the screen.

## 🛠️ Fixes and Improvements

### More Reliable Note and Relationship Management

* **Note deletion is safer:** K-Plex cleans up configured ontology references while leaving unrelated properties and ordinary Markdown links untouched unless explicitly requested.

* **Renamed notes stay connected:** Renaming a note now correctly updates its identity and labels in the graph without leaving stale references.

* **Correct relationship arrows:** Explicit ontology relationships retain their intended direction, even when ordinary links point the other way.

* **Clearer Hide Connection behavior:** Dialogs now explain which perspective will hide a relationship, while preserving the original links.

* **Reliable style editing:** Saving or deleting node and relationship styles now completes correctly without getting stuck waiting for unrelated background updates.

### Better Mobile Experience

* Reopening K-Plex in the mobile sidebar now follows the latest relevant note.

* Double-tapping the central node opens its note in the main workspace.

* Improved readability of stacked layout controls on smaller screens.

### Better Privacy and Image Handling

A new **Allow remote node images** setting gives you control over whether K-Plex loads images from external websites.

Remote image loading is disabled by default. Images stored locally in your vault continue to work without requiring this permission.

### Improved Responsiveness and Stability

* Reduced redundant file reads during startup and background indexing.

* Improved consistency when navigation and indexing happen simultaneously.

* Fixed menu positioning so toolbar menus open beside the correct controls.

* Improved handling of graph views and menus when moving between windows.

* Improved indexing status information, including cleaner callouts without overlapping tooltips.

## ❤️ Thank You!

K-Plex is evolving quickly, and your feedback, bug reports, and ideas are helping shape its direction.

If you encounter an issue, use **Report a bug** from K-Plex to collect diagnostic information that can help me investigate.

If you enjoy K-Plex, please consider supporting its development:

* [Support K-Plex on Ko-fi](https://ko-fi.com/zsolt)

* [Join the Sketch Your Mind Community](https://community.sketch-your-mind.com/)

* [K-Plex on GitHub](https://github.com/zsviczian/kplex)

Happy exploring!

**Zsolt**

## What's Changed
* Add Wander navigation and improve Plex controls and automatic fitting by @zsviczian in https://github.com/zsviczian/kplex/pull/120
* Support Windows Obsidian CLI testing by @zsviczian in https://github.com/zsviczian/kplex/pull/121
* Document K-Plex issue assessment and agent draft-PR handoff workflow by @zsviczian in https://github.com/zsviczian/kplex/pull/122
* Fix mobile sidebar follow and central-note opening by @zsviczian in https://github.com/zsviczian/kplex/pull/123
* Fix #114: preserve explicit ontology arrow direction by @zsviczian in https://github.com/zsviczian/kplex/pull/136
* Require explicit consent for remote node images by @zsviczian in https://github.com/zsviczian/kplex/pull/137
* Fix duplicate startup reads after foreground cancellation by @zsviczian in https://github.com/zsviczian/kplex/pull/142
* Fix graph identity and labels after note rename by @zsviczian in https://github.com/zsviczian/kplex/pull/139
* Fix toolbar menu anchoring and migration cleanup by @zsviczian in https://github.com/zsviczian/kplex/pull/138
* fix: scope node deletion and quote content references by @zsviczian in https://github.com/zsviczian/kplex/pull/141
* Avoid duplicate Sidecar opens and preserve latest navigation by @zsviczian in https://github.com/zsviczian/kplex/pull/140
* Complete style saves and deletes reliably by @zsviczian in https://github.com/zsviczian/kplex/pull/146
* Add adjacent Sidecar attachment and fix indexing callouts by @zsviczian in https://github.com/zsviczian/kplex/pull/152


**Full Changelog**: https://github.com/zsviczian/kplex/compare/0.1.2...0.1.3

## Previous and next

← [[Release 0.1.2|Previous release]] · [[11 Release notes/Release notes|All releases]] · [[Release 0.2.0|Next release →]]
