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

| | **Search Vault** | **Find in this Plex** |
| --- | --- | --- |
| **Question** | Where should I go? | Where is something on this map? |
| **Scope** | Vault-wide names, aliases, paths, supported files and discovered URLs | Nodes and ontology labels in the *currently visible* Plex |
| **Open** | **Alt/Option+/** (fresh default), your configured key, or the Search Vault box | **Ctrl/Cmd+F** or the local magnifier |
| **Result** | Navigate to another center | Highlight local matches without moving the center |

## Use Search Vault to navigate

K-Plex fuzzy-matches names, display names, paths, aliases and URL substrings. Full filename/path lookup can work even while richer indexing is in progress. URL discovery may still be incomplete.

## Use Find in this Plex to locate

Local Find searches the **projected graph**, including ontology labels. Turn on **Include file paths** to extend its scope. Use **Enter** and **Shift+Enter** to cycle through matches. **Escape** closes and clears Find.

Select **Filter matching notes** to temporarily retain only label-matching nodes and reflow the local Plex. Switch it off to restore the previous filter/layout; editing **Filters and lenses** manually takes ownership of that temporary filter.

**Try it:** Press **Alt/Option+/** (or your configured search shortcut), search for **Ontology and relationship fields**, then Ctrl/Cmd+F and look for **Child** on its visible Plex. See [[10 Discover by topic/02 Find and navigate knowledge|Find and navigate knowledge]].

## A third choice: type to select

When the graph itself has focus, you can simply type a phrase to **select matching displayed node labels** and use Tab/Shift+Tab to cycle them. This is a temporary selection, not an indexed Vault search or a Find filter. Details: [[02 Navigate and explore/Type to select visible nodes|Type to select visible nodes]].

**Shortcut note:** the fresh graph-local default for **Search Vault** is **Alt/Option+/**; F4 can remain active in upgraded or customized vaults. **Ctrl/Cmd+F** opens **Find in Plex** from the graph, but remains the normal Find key inside an editor.

## One selection highlight for Find and keyboard movement

The same **node highlight** is used when you move a selection with the keyboard and when **Find in Plex** reveals a match. If you switch between these methods, you can follow the highlighted item instead of looking for two separate selection indicators. This only changes local presentation: it does not expand Find to whole-vault search or change the selected center by itself.

[Refinement: PR #108](https://github.com/zsviczian/kplex/pull/108).
