---
tags:
  - kplex-help/release-notes
Guide:
  - "[[11 Release notes/Release notes]]"
Explains:
  - "[[05 Personalize and workspace/Sidecar]]"
  - "[[02 Navigate and explore/Editor node and web pages]]"
  - "[[05 Personalize and workspace/Visibility and connector styling]]"
  - "[[06 Indexing and troubleshooting/How indexing works]]"
Previous:
  - "[[Release 0.2.3]]"
Next:
  - "[[Release 0.3.0]]"
Related:
  - https://github.com/zsviczian/kplex/releases/tag/0.2.4
  - https://github.com/zsviczian/kplex/pull/210
  - https://github.com/zsviczian/kplex/pull/211
  - https://github.com/zsviczian/kplex/pull/213
  - https://github.com/zsviczian/kplex/pull/212
  - https://github.com/zsviczian/kplex/pull/214
  - https://github.com/zsviczian/kplex/compare/0.2.3...0.2.4
Note type: ReleaseNotes
---
# K-Plex 0.2.4 — More room for your work

Give a document or its map more space with one action, and keep exploring while edits are indexed. This update improves Sidecar controls, framing, editor shortcuts and gate-count stability.

Published **2026-10-24**. The original GitHub release text is reproduced below.

## Original published notes

## Navigation and Layout

### Improved Sidecar Controls
- **One-click maximize:** ALT/OPT+click the Sidecar controls to expand either the Sidecar or K-Plex in one action, without manually folding and unfolding panels.
- **Automatic recentering:** K-Plex now recenters the graph when the Sidecar opens or closes, making better use of the available space.
- **Smarter zoom behavior:** Automatic recentering respects your Autozoom setting, preserving your zoom level when Autozoom is disabled.

### Faster Access to the Central Editor
- ALT/OPT+click **Use editor as central node** to open directly in expanded editor mode.
- Regular clicks continue to work as before.

### Cleaner Visibility Controls
- The nine graph visibility switches now use a three-column layout when space allows.
- The layout automatically adjusts to two or one column in narrower panels.
- Subtle dividers make the controls easier to scan.

## Graph Stability

### Stable Gate Counters
- Gate counters no longer briefly disappear, show zero, or display incomplete counts during ordinary Markdown autosaves.
- Counters remain stable when relationships have not changed and update when actual changes occur.
- Folder and tag nodes now correctly display zero for friend and challenger relationships that do not apply to them.
- Improved handling of folder and tag membership keeps structural relationship counts accurate during edits.

### Cleaner Tooltips
- Removed overlapping and duplicate tooltips from central editor controls.
- Improved accessibility labels and hover behavior.

## Indexing and Performance

### More Efficient Indexing During Edits
- K-Plex now preserves completed indexing work when files or metadata change during indexing.
- Avoids repeatedly restarting large indexing operations when only a few notes have changed.
- Reduces unnecessary full graph rebuilds during startup.
- Keeps the graph responsive while indexing catches up with ongoing changes.

### Faster Cache Restoration
- Improved reuse of previously indexed data when reopening K-Plex.
- Reduced redundant database operations during warm starts.
- Maintains the existing cache validation and relationship consistency checks.

These improvements target unnecessary background work and resource consumption, particularly during startup and active note editing.

## What's Changed
* Preserve valid indexing progress through source event bursts by @zsviczian in https://github.com/zsviczian/kplex/pull/210
* Keep autosave gate counters stable and show structural lateral zeros by @zsviczian in https://github.com/zsviczian/kplex/pull/211
* Maximize Sidecar or K-Plex with modifier-click by @zsviczian in https://github.com/zsviczian/kplex/pull/213
* Share clean warm source-head selection by @zsviczian in https://github.com/zsviczian/kplex/pull/212
* Polish Sidecar framing, editor shortcuts and visibility controls by @zsviczian in https://github.com/zsviczian/kplex/pull/214


**Full Changelog**: https://github.com/zsviczian/kplex/compare/0.2.3...0.2.4
