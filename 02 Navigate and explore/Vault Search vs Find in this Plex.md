---
aliases:
- Vault Search vs Find in this Plex
tags:
- kplex-help/how-to
- kplex/navigation
- kplex/search
Related:
- '[[04 Filter and focus/Quick Filter]]'
Previous:
- '[[02 Navigate and explore/Navigating the Plex]]'
Next:
- '[[02 Navigate and explore/Past nodes and pins]]'
---
![[Image - Search.png]]

There are two search tools because they answer **different questions**.

| | Search Vault | Find in this Plex |
| --- | --- | --- |
| Question | Where should I go? | Where is something on this map? |
| Scope | Vault-wide names, aliases, paths, supported files and discovered URLs | Nodes and ontology labels in the displayed Plex |
| Open | The toolbar search box or your configured Vault Search shortcut | The local magnifier or Control+F / Command+F while the graph has focus |
| Result | Navigate to another center | Reveal local matches without moving the center |

## Use Search Vault to navigate

K-Plex fuzzy-matches names, display names, paths, aliases and URL substrings. Full filename/path lookup can work while richer indexing is in progress. URL discovery may still be incomplete.

**Next release:** Search includes folders and hierarchical tags, with type icons to distinguish results. Type **#** before a query to search tags only. Search, history and pins retain full tag paths, so similarly named child tags are easier to distinguish.

Make a folder the center to explore its location and contents. Make a hierarchical tag the center to see its parent, child tags and associated notes—even when tags are hidden in ordinary note neighborhoods. Native folders and tags already known to Obsidian can appear during startup without waiting for the complete richer index.

To change membership or move files rather than simply navigate, see [[03 Build and edit/Drag drop and reclassify]].

## Use Find in this Plex to locate

Local Find searches the projected graph, including ontology labels. Turn on **Include paths** to include file paths. Use Enter and Shift+Enter to cycle through matches; Escape closes and clears Find.

Select **Filter matching notes** to retain label-matching nodes and reflow the local Plex. Switch it off to restore the previous filter/layout; editing Filters and lenses manually takes ownership of that temporary filter. Matching a note does not automatically highlight all its surrounding connections.

**Try it:** Use Vault Search to navigate to **Ontology and relationship fields**, then local Find to locate **Child** in its displayed Plex. See [[10 Discover by topic/02 Find and navigate knowledge]].

## A third choice: type to select

With the graph focused, type a phrase to select matching displayed node labels and use Tab/Shift+Tab to cycle through them. This is temporary selection, not Vault Search or a Find filter. See [[02 Navigate and explore/Type to select visible nodes]].

The node highlight is shared by keyboard selection and Find, making it easier to follow the selected item when switching methods. Neither alone changes the Plex center.

**Shortcut note:** Defaults and saved assignments can differ. Alt+/ on Windows or Option+/ on macOS is a fresh graph-local Vault Search default; F4 can remain in upgraded or customized vaults, including the supplied help configuration. Control+F / Command+F remains the editor's normal Find command when an editor has focus.

Sources: [earlier Find refinement #108](https://github.com/zsviczian/kplex/pull/108), [next-release search and tag navigation #177](https://github.com/zsviczian/kplex/pull/177), [reviewed navigation guide](https://github.com/zsviczian/kplex/blob/10760685552fdbafe089a58fc8d80d318853ff31/README.md#search-history-and-pins).
