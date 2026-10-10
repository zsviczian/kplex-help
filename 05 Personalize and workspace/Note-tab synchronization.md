---
aliases:
  - "Note-tab synchronization"
tags:
  - "kplex-help/reference"
  - "kplex/workspace"
  - "kplex/navigation"
Friend:
  - "[[02 Navigate and explore/Past nodes and pins]]"
Previous:
  - "[[05 Personalize and workspace/Sidecar]]"
Next:
  - "[[05 Personalize and workspace/Visibility and connector styling]]"
---
K-Plex and normal note tabs can be paired in three modes:

- **Independent** — K-Plex navigation and note-tab navigation do not drive each other.
- **Most recent note tab** — K-Plex links to the most recently used note tab.
- **Pinned to one fixed note tab** — K-Plex stays paired with a specific note tab.

One-shot commands can send the current K-Plex note to the recent tab or bring the recent tab into K-Plex. **Show linked/pinned tab** activates the actual connected tab and briefly outlines its pane so you can identify it.

This synchronization is controlled from the live K-Plex toolbar rather than duplicated in Settings.

## Linked Excalidraw tab behavior

If a linked tab or Sidecar is displaying an Excalidraw file, **passive same-file synchronization** now preserves the chosen **drawing vs Markdown** representation. An explicit open command or a direct drawing/Markdown toggle can still switch representations; navigating to a different file still follows the configured sync behavior. This prevents routine pane-follow updates from unexpectedly replacing an intentional editing view.

[Change: PR #112](https://github.com/zsviczian/kplex/pull/112).
