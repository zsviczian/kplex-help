---
aliases:
- What changed
- Recent features
- Changes since K-Plex 0.1.3
tags:
- kplex-help/section
- kplex/getting-started
- kplex/navigation
Child:
- '[[02 Navigate and explore/Wander]]'
- '[[02 Navigate and explore/Footprints and breadcrumbs]]'
- '[[05 Personalize and workspace/Colors and themes]]'
- '[[03 Build and edit/Drag drop and reclassify]]'
- '[[03 Build and edit/Create notes and placeholders]]'
- '[[05 Personalize and workspace/Sidecar]]'
- '[[05 Personalize and workspace/Note-tab synchronization]]'
- '[[05 Personalize and workspace/Layout density and typography]]'
- '[[05 Personalize and workspace/Visibility and connector styling]]'
- '[[06 Indexing and troubleshooting/Understanding index status]]'
- '[[06 Indexing and troubleshooting/Rebuild purge and diagnostics]]'
- '[[02 Navigate and explore/K-Plex command palette]]'
- '[[02 Navigate and explore/Keyboard navigation]]'
- '[[05 Personalize and workspace/Actions and shortcuts]]'
- '[[05 Personalize and workspace/Fullscreen and Zen mode]]'
- '[[03 Build and edit/Date properties and daily notes]]'
- '[[03 Build and edit/Ontology autocomplete]]'
- '[[03 Build and edit/Remove one relationship source]]'
- '[[08 About/Sketch Your Mind book]]'
Friend:
- '[[00 Start Here/Choose a topic]]'
- '[[00 Start Here/Glossary]]'
- '[[07 Use cases/Use cases]]'
---
# Changes since K-Plex 0.1.3

For versioned release notes, including the **proposed 0.2.0 draft**, see [[11 Release notes/Release notes]]. This page remains a rolling summary, not the release record.

**Review date: October 19, 2026.** The latest published release is [0.1.3, released October 13](https://github.com/zsviczian/kplex/releases/tag/0.1.3). This help update reviews accepted K-Plex source through [main at 3df08a1](https://github.com/zsviczian/kplex/commit/3df08a15f7002ed60a2452286ee1f8044cb97203), including merged [PR #187](https://github.com/zsviczian/kplex/pull/187).

**Available** means shipped in 0.1.3. **Next release** means implemented and merged by this review but not shipped in 0.1.3. **Missing** means the reviewed baseline does not provide it. A merged PR is not itself a published plugin release; no next version number or release date is assumed.

> [!important] The bundled plugin is older than these docs
> This help repository currently includes a K-Plex **0.1.2** manifest and bundled plugin files. Update the installed plugin to 0.1.3 for the released workflows. Next-release sections require a corresponding newer build. This documentation update does not replace plugin executables, settings or workspace files.

## Start with something useful

[[07 Use cases/Use cases|What You Can Do with K-Plex]] now offers nine everyday workflows: build a topic map, run a project, develop an article, test a proposal, recover meeting context, follow a procedure, garden neglected notes, rediscover ideas and develop visual notes. Each starts with an outcome rather than a list of controls.

## Already available in 0.1.3

[[02 Navigate and explore/Wander|Wander]] explores connected notes with pause, speed and stop controls. [[05 Personalize and workspace/Sidecar|Sidecar]] adds practical adjacent-pane attachment and send/pull actions. The graph's background menu gives direct access to settings, display modes, background color, Wander and bug reporting.

The release also improves navigation continuity, relationship editing and deletion feedback. [[05 Personalize and workspace/Images in nodes|Remote node images require explicit permission]] and are off by default; local node images remain available. See the release notes for the complete shipped changes.

## Next release: organize and work with less friction

| What improves | Where to try it |
| --- | --- |
| **Bring research into a draft or another Plex.** Drag supported node links into the Markdown editor or between views. Resolved Bases links can enter the Plex, and a sibling can become a direct relation without losing its other context. | [[03 Build and edit/Drag drop and reclassify]] |
| **File and tag knowledge where you find it.** Supported gate drops move files/folders or assign tags and Note Types. Actual moves require confirmation unless the modifier bypass is used; safety checks still apply. | [[03 Build and edit/Drag drop and reclassify]] |
| **Capture ideas in the right place.** Choose creation/materialization folders and an explicit After saving outcome. Preserve intended placeholder paths and link aliases; recover partial creation without duplicating the file. | [[03 Build and edit/Create notes and placeholders]] |
| **Find structure, not only filenames.** Search folders and hierarchical tags, use a # query for tags, and distinguish full tag paths in search/history/pins. | [[02 Navigate and explore/Vault Search vs Find in this Plex]] |
| **Keep multiple graph and document contexts independent.** The + button opens an adjacent Plex. Each view now owns its document-sync mode, exact target and Sidecar association, so two Plexes can follow different notes. | [[05 Personalize and workspace/Note-tab synchronization]] |
| **Retrace a session without changing shared history.** Footprints retains every visit in each Plex, including repetitions. Revisit earlier stops, start a fresh local trail or copy it as Markdown before closing. | [[02 Navigate and explore/Footprints and breadcrumbs]] |
| **Edit metadata in context.** An unpinned, ungrouped File properties pane follows the central file and clears for non-file centers. | [[05 Personalize and workspace/Note-tab synchronization]] |
| **Make room for the document.** Fold the entire Plex tab group and restore it from the surviving Sidecar edge, with safeguards for other tabs and ambiguous layouts. | [[05 Personalize and workspace/Sidecar]] |
| **Use a narrower graph.** One-sided layout places Friends and Challengers in separate left-hand groups, with device/main-tab/side-panel preferences. | [[05 Personalize and workspace/Layout density and typography]] |

These changes are covered by [#171](https://github.com/zsviczian/kplex/pull/171), [#173](https://github.com/zsviczian/kplex/pull/173), [#177](https://github.com/zsviczian/kplex/pull/177) and [#187](https://github.com/zsviczian/kplex/pull/187). **PRs #177 and #187 are merged**; folder/tag actions and per-Plex Footprints are no longer missing proposals.

## Next release: make the graph fit your way of working

[[05 Personalize and workspace/Colors and themes|Colors and themes]] covers native Obsidian colors, named K-Plex themes, Light/Dark pairs, separate base/semantic resets and optional directional tint. Existing custom appearances are preserved. Note Type tag links have their own style, and shared style controls include paired previews and inheritance resets. Sources: [#158](https://github.com/zsviczian/kplex/pull/158), [#177](https://github.com/zsviczian/kplex/pull/177).

[[05 Personalize and workspace/Visibility and connector styling|Modifier highlighting]] keeps hover effects and area outlines intentional. Alt/Option-hover can temporarily reveal eligible cross-links for a displayed node or its exact gate even when normal cross-links are off. It does not reveal filtered-out nodes or change the toggle. Sources: [#170](https://github.com/zsviczian/kplex/pull/170), [#171](https://github.com/zsviczian/kplex/pull/171), [#181](https://github.com/zsviczian/kplex/pull/181).

Settings received from another device update the running plugin without an immediate save-back. Conflicting open appearance drafts need to be reopened before reapplying them; simultaneous cross-device edits still depend on the sync service's conflict handling. See [[05 Personalize and workspace/Colors and themes]] and [#182](https://github.com/zsviczian/kplex/pull/182).

## Next release: clearer saves, startup and diagnostics

[[06 Indexing and troubleshooting/Understanding index status|Startup and live updates]] better preserve the requested center and history while cached/background data arrives. New notes and drawings become discoverable earlier; late ontology updates refresh a stationary Plex. Ordinary prose autosaves preserve an equivalent graph layout. Settings saves distinguish accepted storage from pending graph work, and ontology-field editing no longer initiates the former work on every keystroke.

[[06 Indexing and troubleshooting/Rebuild purge and diagnostics|Diagnostics]] adds a bounded passive activity summary to both report routes. Capture it before a restart and review it before sharing. Local readiness, URL discovery, saved data and CPU usage are different questions; these changes do not establish a universal speedup or prove the reported whole-application Settings freeze fixed.

Sources: [#147](https://github.com/zsviczian/kplex/pull/147), [#168](https://github.com/zsviczian/kplex/pull/168), [#172](https://github.com/zsviczian/kplex/pull/172), [#174](https://github.com/zsviczian/kplex/pull/174), [#179](https://github.com/zsviczian/kplex/pull/179), [#180](https://github.com/zsviczian/kplex/pull/180), [#183](https://github.com/zsviczian/kplex/pull/183), [#185](https://github.com/zsviczian/kplex/pull/185), [#186](https://github.com/zsviczian/kplex/pull/186). The [source comparison](https://github.com/zsviczian/kplex/compare/0.1.3...3df08a15f7002ed60a2452286ee1f8044cb97203) also includes supporting cache/indexing changes, validation and documentation work, which are not separate user-facing features.

## Not part of the reviewed implementation

Per-Plex session Footprints and independent document sync are implemented in merged [#187](https://github.com/zsviczian/kplex/pull/187), but a **visual branching or metro-map trail** is not part of this MVP. Footprints is not automatically persisted; pins and saved Past nodes history remain shared and persisted. The section-link correction in [#162](https://github.com/zsviczian/kplex/pull/162) and reciprocal ontology syntax in [#154](https://github.com/zsviczian/kplex/pull/154) are not merged and are not presented here as fixes or available syntax.

The use cases also do not depend on checkbox-task projection, automatic whole-vault Lens queries, custom layout engines or Excalidraw focus-frame selection.

## Earlier guides remain useful

For established workflows, follow [[10 Discover by topic/11 Work without the mouse]], [[10 Discover by topic/12 Connect dates and daily notes]] or [[10 Discover by topic/13 Present and concentrate]]. The existing keyboard, command palette, shortcut, Date, autocomplete, source-removal and [[08 About/Sketch Your Mind book|book]] guides remain linked in this note's children.
