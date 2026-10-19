---
aliases:
- K-Plex 0.1.0 release notes
tags:
- kplex-help/release-notes
- kplex/released
Guide:
- '[[11 Release notes/Release notes]]'
Previous:
- '[[11 Release notes/K-Plex 0.0.5]]'
Next:
- '[[11 Release notes/K-Plex 0.1.1]]'
Explains:
- '[[02 Navigate and explore/Navigate and explore]]'
- '[[03 Build and edit/Build and edit]]'
- '[[04 Filter and focus/Graph Lenses]]'
- '[[06 Indexing and troubleshooting/Understanding index status]]'
---
# K-Plex 0.1.0 — release notes

**Published:** 2026-10-07 · [Original GitHub release](https://github.com/zsviczian/kplex/releases/tag/0.1.0)

## Explore these changes in K-Plex Help

- [[02 Navigate and explore/Navigate and explore]]
- [[03 Build and edit/Build and edit]]
- [[04 Filter and focus/Graph Lenses]]
- [[06 Indexing and troubleshooting/Understanding index status]]

## Original published release notes

> [!note] Historical record
> The text below comes from the published GitHub release, not a retrospective reconstruction. Follow the links above to the living Help pages, which may describe newer behavior.

# K-Plex 0.1.0

<img width="1358" height="1000" alt="image" src="https://github.com/user-attachments/assets/a2a985be-4466-41cb-912b-2d53c10ed63d" />

K-Plex 0.1.0 is a major usability, navigation, editing, and performance release.

The biggest change is that K-Plex no longer needs to finish processing your entire vault before it becomes useful. Search, navigation, local graphs, and relationship editing are prioritized, while broader indexing continues cooperatively in the background.

This release also adds a much richer center editor, new search and layout tools, improved drag-and-drop workflows, multilingual UI, and stronger ExcaliBrain migration support.

## 🚀 Faster startup and more responsive indexing

K-Plex now prioritizes what you are working with instead of treating full-vault indexing as a prerequisite.

- **On-demand indexing is now the default.** K-Plex prepares the current Plex and the information needed for your immediate actions first.
- **Eager indexing remains available** if you prefer K-Plex to process the full vault in the background.
- Search becomes available very early during startup, before complete indexing.
- Cached graphs can be displayed and used while background verification continues.
- Navigation, creating notes, editing relationships, and visible graph updates take priority over background work.
- Local graphs remain stable while additional relationships and counts are discovered instead of being replaced by incomplete intermediate results.
- High-degree URL nodes are significantly more responsive during indexing.
- Web-link discovery now has its own persisted cache and can restore independently.
- Changing ontology, inference, filters, styling, or other presentation settings no longer unnecessarily invalidates the underlying source index.
- Indexing progress now reports more meaningful phases and counts.
- Index progress and compatible cached data survive restarts more reliably.
- Creating or changing a note no longer causes unnecessary full-vault rebuilds.

A new **Settings → Indexing config** section provides:

- **Indexing mode:** On-demand or Eager
- **Background indexing speed:** Responsive, Balanced, or Faster
- **Purge index cache**, including an estimate of the current cache size

The default configuration is **On-demand + Responsive**.

While K-Plex is still discovering information, some global counts and relationships may fill in progressively. The index indicator shows the current state.

## ✏️ A much richer center

<img width="1380" height="806" alt="image" src="https://github.com/user-attachments/assets/53d4e74f-2e41-478a-bf8e-af75522c3989" />

The center of the Plex can now become a working editor instead of only representing the current note.

For Markdown and Excalidraw notes you can switch between the compact node and an **embedded Obsidian editor** without leaving K-Plex.

The embedded center now supports:

- Markdown reading and editing
- Excalidraw drawings, including Markdown/drawing switching and zoom-to-fit
- Canvas files
- Images with contain-fit display
- Websites
- Video-aware web layouts

The surrounding Plex automatically makes room for the editor, including when it is resized or expanded.

Links opened from embedded content continue to work with K-Plex navigation and Obsidian's normal tab/pane behavior.

## 🔎 Better search

K-Plex now has two clearly separated search experiences.

### Vault search — `F4`

Vault search works across the vault, not just the currently indexed Plex.

It can find:

- Markdown notes
- Attachments, including orphan files
- Canvas files
- URLs
- URL aliases

### Find in Plex — `Ctrl/Cmd+F`

Find in Plex searches only the graph currently on screen.

It can:

- Find displayed note names and ontology labels
- Optionally include file paths
- Reveal matches hidden inside scrollable areas
- Move between matches with Enter / Shift+Enter
- Temporarily **filter matching notes and reflow the Plex** around the center

Vault search and Find in Plex are independent, so finding something locally no longer changes your main navigation search.

## 🔗 Faster relationship workflows

Creating and changing relationships now requires fewer modal steps.

- Drag a **relationship gate onto a Past node or pinned note** to create that relationship directly.
- Drag a node body onto history or a pinned note to choose the relationship type.
- Drag files from Obsidian's File Explorer onto K-Plex:
  - drop on the center to navigate there
  - drop on a relationship area to create a relationship
- Eligible drop targets highlight while dragging.
- Relationship edits remain available while indexing continues.
- Unlinking works immediately even while cached/source data is being reconciled.
- Ordinary visible nodes now receive more accurate directional relationship counts.

The Add Link / Add Child dialog is also **draggable on desktop**.

## 🧭 Improved navigation

Several smaller changes make K-Plex fit better into an Obsidian workspace.

- Drag a Markdown note from File Explorer onto K-Plex to make it the center.
- Node context menus now include an **Open** submenu for:
  - an existing tab
  - a new tab
  - an adjacent pane
  - a pop-out window where available
- Recent-tab synchronization now correctly remembers inactive tabs inside tab groups.
- URL nodes respect Obsidian's Web Viewer/browser preference.
- URL nodes can be opened with **double-tap on touch devices**.
- A new **About vault** view provides useful vault and indexing information.

## 🎛️ More control over the Plex layout

Layout can now be adjusted directly from the Plex.

New controls include:

- Horizontal density
- Vertical density
- 1–3 parent columns
- Child columns
- Base font size
- Maximum node width
- Label wrapping
- More flexible long and two-line labels

Relationship areas can be resized directly by dragging their boundaries. **Area settings** can expose resize handles for all areas, including empty ones.

Filters and lenses can also be repositioned, and the Plex Find filter can temporarily hide non-matching nodes and reflow the graph.

Numerous spacing, wrapping, clipping, toolbar, theme contrast, thumbnail, Canvas zoom, and resize behaviors have also been refined.

## 🌍 K-Plex now speaks more languages

K-Plex now includes complete UI translations for:

- German
- French
- Spanish
- Dutch
- Japanese
- Traditional Chinese
- Russian

English remains the fallback for unsupported locales.

## 🧠 Improved ExcaliBrain migration

The remaining ExcaliBrain compatibility path has been cleaned up and focused on what is useful when moving to K-Plex.

Import now preserves:

- Ontology configuration
- Node styles
- Tag-based node styles
- Relationship/link styles
- Relevant graph styling

Imported styles are also visible and editable in K-Plex's style managers.

K-Plex-specific UI, navigation, editor, indexing, and other local preferences remain under K-Plex's control rather than being overwritten by ExcaliBrain settings.

K-Plex now consistently uses K-Plex naming and canonical K-Plex command IDs. If you previously assigned hotkeys to legacy ExcaliBrain command IDs, review your Obsidian hotkey settings after upgrading.

## 🛠️ Fixes and polish

0.1.0 also includes many smaller corrections, including:

- More stable graphs while background indexing progresses
- Correct restoration of visible node styling, including Excalidraw styling
- Reduced flicker and repeated updates around heavily referenced URLs
- Better index-status behavior on narrow layouts
- More reliable cache restoration and recovery
- Improved imported ExcaliBrain style handling
- More consistent touch interactions
- Improved image thumbnails and previews
- Better Canvas resize and zoom behavior
- Improved toolbar wrapping and theme contrast
- More reliable live relationship counts and filtering
- Numerous mobile, tablet, Sidecar, pop-out, and desktop layout fixes

---

**Full Changelog:** https://github.com/zsviczian/kplex/compare/0.0.5...0.1.0

## What's Changed
* feat: refactor - establish portable graph core and refactor guardrails through C14 by @zsviczian in https://github.com/zsviczian/kplex/pull/38
* fix: imported ExcaliBrain styles and add migration regression coverage by @zsviczian in https://github.com/zsviczian/kplex/pull/39
* feat(i18n): extract user-facing strings to English catalog by @zsviczian in https://github.com/zsviczian/kplex/pull/40
* feat(ui): draggable desktop dialog shell for related-note modal by @zsviczian in https://github.com/zsviczian/kplex/pull/41
* feat(i18n): bundle German, French, Spanish, Dutch, Japanese, Traditional Chinese and Russian translations by @zsviczian in https://github.com/zsviczian/kplex/pull/42
* feat: Open K-Plex on a note dropped from File Explorer by @zsviczian in https://github.com/zsviczian/kplex/pull/43
* feat: Add file opening submenu to Plex node context menus by @zsviczian in https://github.com/zsviczian/kplex/pull/44
* feat: Show a useful graph and search results sooner during startup by @zsviczian in https://github.com/zsviczian/kplex/pull/45
* feat: Show live indexing progress from the status indicator by @zsviczian in https://github.com/zsviczian/kplex/pull/46
* fix: Open URL nodes correctly and support touch double-tap by @zsviczian in https://github.com/zsviczian/kplex/pull/47
* feat: improve indexing status feedback and persist startup notice dismissal by @zsviczian in https://github.com/zsviczian/kplex/pull/48
* feat: resize Plex relationship areas directly by @zsviczian in https://github.com/zsviczian/kplex/pull/49
* feat: add an embedded central editor with Excalidraw support by @zsviczian in https://github.com/zsviczian/kplex/pull/52
* fix: avoid full vault rebuilds when creating notes by @zsviczian in https://github.com/zsviczian/kplex/pull/53
* fix: preserve recent tab history within tab groups by @zsviczian in https://github.com/zsviczian/kplex/pull/55
* feat: complete K-Plex naming and ExcaliBrain graph import by @zsviczian in https://github.com/zsviczian/kplex/pull/58
* fix: preserve large-vault index progress across restarts by @zsviczian in https://github.com/zsviczian/kplex/pull/57
* Make indexing independent of ontology and settings by @zsviczian in https://github.com/zsviczian/kplex/pull/72
* Improve search, embedded editors and relationship workflows by @zsviczian in https://github.com/zsviczian/kplex/pull/74
* Keep search and graph editing available during indexing by @zsviczian in https://github.com/zsviczian/kplex/pull/75
* Improve Plex layout controls and relationship interactions by @zsviczian in https://github.com/zsviczian/kplex/pull/76
* Keep local graphs responsive during indexing by @zsviczian in https://github.com/zsviczian/kplex/pull/78

## New Contributors
* @zsviczian made their first contribution in https://github.com/zsviczian/kplex/pull/38

**Full Changelog**: https://github.com/zsviczian/kplex/compare/0.0.5...0.1.0

## Previous and next

← [[11 Release notes/K-Plex 0.0.5|Previous release]] · [[11 Release notes/Release notes|All releases]] · [[11 Release notes/K-Plex 0.1.1|Next release →]]
