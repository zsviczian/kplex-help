---
aliases:
- What changed
- Recent features
tags:
- kplex-help/section
- kplex/getting-started
- kplex/navigation
Child:
- '[[02 Navigate and explore/K-Plex command palette]]'
- '[[02 Navigate and explore/Keyboard navigation]]'
- '[[05 Personalize and workspace/Actions and shortcuts]]'
- '[[05 Personalize and workspace/Fullscreen and Zen mode]]'
- '[[03 Build and edit/Date properties and daily notes]]'
- '[[03 Build and edit/Ontology autocomplete]]'
- '[[06 Indexing and troubleshooting/Understanding index status]]'
- "[[03 Build and edit/Remove one relationship source]]"
- "[[08 About/Sketch Your Mind book]]"
Friend:
- '[[00 Start Here/Choose a topic]]'
- '[[00 Start Here/Glossary]]'
---
This is a quick route to capabilities introduced in the recent merged updates. For detailed steps, open the linked guide. This is **not** a version-specific changelog: the notes describe behavior in the current K-Plex source.

| New or improved | What to try |
| --- | --- |
| [[05 Personalize and workspace/Fullscreen and Zen mode|Fullscreen and Zen]] | Maximize K-Plex inside desktop Obsidian; hide its toolbars independently in Zen mode. |
| [[02 Navigate and explore/K-Plex command palette|K-Plex command palette]] | Run graph actions with **Alt/Option+.** while the graph has focus. |
| [[02 Navigate and explore/Keyboard navigation|Keyboard navigation]] | Use arrows to select, Alt/Option+arrows to change relationship areas, and Enter to navigate. |
| [[02 Navigate and explore/Type to select visible nodes|Type to select visible nodes]] | Type a name on the focused graph and move between matching visible nodes with Tab. |
| [[02 Navigate and explore/Keyboard shortcuts reference|Keyboard shortcuts reference]] | Review current defaults and the differences between a graph shortcut and an Obsidian hotkey. |
| [[05 Personalize and workspace/Actions and shortcuts|Actions and shortcuts]] | Record, disable, reset and publish actions; inspect saved conflicts. |
| [[03 Build and edit/Date properties and daily notes|Date property roles]] | Choose a default Date relationship while keeping explicit field ontology in control. |
| [[03 Build and edit/Ontology autocomplete|Ontology autocomplete]] | Add ontology fields with the editor suggester; long pastes no longer trigger the former pathological matcher. |
| [[06 Indexing and troubleshooting/Understanding index status|Index status]] | Check local readiness separately from full indexing and URL discovery. |

## Choose a hands-on route

- [[10 Discover by topic/11 Work without the mouse|Work without the mouse]] — keyboard navigation, local palette and custom actions.
- [[10 Discover by topic/12 Connect dates and daily notes|Connect dates and daily notes]] — a Date property and an existing daily note.
- [[10 Discover by topic/13 Present and concentrate|Present and concentrate]] — fullscreen, Zen and uncluttered layouts.

**Source references:** [Fullscreen and Zen #86](https://github.com/zsviczian/kplex/pull/86), [Action Manager #85](https://github.com/zsviczian/kplex/pull/85), [keyboard navigation #80](https://github.com/zsviczian/kplex/pull/80), [Date role #94](https://github.com/zsviczian/kplex/pull/94), [status fix #82](https://github.com/zsviczian/kplex/pull/82), [index responsiveness #78](https://github.com/zsviczian/kplex/pull/78), [ontology suggester #87](https://github.com/zsviczian/kplex/pull/87).

## Improvements from the most recent merged PRs

| Improvement | Start here |
| --- | --- |
| **Sharper typography controls** independent of density and clearer narrow-pane sliders | [[05 Personalize and workspace/Layout density and typography|Layout density and typography]] |
| **Windows fullscreen and Zen control placement** | [[05 Personalize and workspace/Fullscreen and Zen mode|Fullscreen and Zen mode]] |
| **Remove one eligible frontmatter source**, with confirmation | [[03 Build and edit/Remove one relationship source|Remove one relationship source]] |
| **Consistent node highlight** for Find and keyboard navigation | [[02 Navigate and explore/Vault Search vs Find in this Plex|Search Vault vs Find]] |
| **Correct filtered gate counts** based on semantic endpoints | [[02 Navigate and explore/Navigating the Plex|Navigating the Plex]] |
| **Keep Excalidraw drawing/Markdown choice** while Sidecar follows the same note | [[03 Build and edit/Excalidraw integration|Excalidraw integration]] |
| **More responsive dense URL indexing and cache restoration** | [[06 Indexing and troubleshooting/Large vault behavior|Large vault behavior]] |
| **Sketch Your Mind — the book and project links** | [[08 About/Sketch Your Mind book|Sketch Your Mind book]] |

Source changes: [PR #95](https://github.com/zsviczian/kplex/pull/95), [#102](https://github.com/zsviczian/kplex/pull/102), [#104](https://github.com/zsviczian/kplex/pull/104), [#105](https://github.com/zsviczian/kplex/pull/105), [#108](https://github.com/zsviczian/kplex/pull/108) and [#112](https://github.com/zsviczian/kplex/pull/112). Documentation-only PR #103 does not change the help's end-user features.
