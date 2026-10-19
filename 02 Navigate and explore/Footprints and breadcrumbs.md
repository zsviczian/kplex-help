---
aliases:
- Breadcrumbs
- Footprints
- Session breadcrumbs
- Complete visit trail
tags:
- kplex-help/how-to
- kplex/navigation
Guide:
- '[[02 Navigate and explore/Navigate and explore]]'
Friend:
- '[[02 Navigate and explore/Past nodes and pins]]'
- '[[05 Personalize and workspace/Note-tab synchronization]]'
- '[[07 Use cases/Rediscover and remember your notes]]'
---
# Breadcrumbs: follow your Footprints

**Outcome:** Find a place you visited earlier in this exploration, or capture the route you took before closing the Plex.

**Status:** **Next release** — merged in [K-Plex PR #187](https://github.com/zsviczian/kplex/pull/187), but not part of published 0.1.3. The control is labeled **Footprints** in K-Plex.

## Revisit a stop on your trail

Navigate from one note to another in the same Plex. Select the **Footprints icon**, next to **Find in Plex** in the upper-right corner. It opens a scrollable list of this Plex's visits, **newest first**. Each visit is kept as a separate entry: if you went A → B → A, both visits to A appear.

Select an earlier entry to navigate back to it. This **adds another visit** at the top of Footprints; it does not erase the later part of your trail. The list follows the latest visit when opened, but if you are reading older entries, incoming visits do not pull you away from them.

Use **Up/Down** to move through the entries, **Home** for the newest, and **End** for the oldest. Escape or clicking outside closes the panel. For long sessions, the panel renders a scrolling window of up to 40 rows at a time; **the trail itself is not limited to 40 visits**.

## Keep or restart the trail

- **Copy as Markdown** copies the **whole trail**, newest first, as a Markdown bullet list, including repeated visits and entries outside the visible scroll window. Notes, attachments, folders and placeholders become wikilinks, tags retain their full `#tag/path`, and websites become Markdown links. Paste it into a note if you want a lasting record; copying does not automatically save a note.
- **Start here** clears **this Plex's Footprints** except for the current center, so a new phase of exploration starts cleanly. It does not clear the shared Past nodes history, change pins, or reset another Plex's Footprints.

**Try it:** Start at a project, visit two related notes, return to the project and open Footprints. Notice that the project appears twice. Copy the trail into a working note, then choose **Start here** before exploring a different question.

## How is this different from Past nodes and pins?

| | Footprints (breadcrumbs) | Past nodes (bottom history) | Pins |
| --- | --- | --- | --- |
| Purpose | Recall **every accepted visit** in this Plex session, including repeats | Shared back/forward navigation and recent locations | Quick access to chosen landmarks |
| Ownership | **One Plex** | Shared by all Plexes | Shared by all Plexes |
| Saved across restart? | **No** | **Yes** | **Yes** |
| What happens on return? | A new visit is appended | Normal back/forward history behavior | The pin remains a shortcut |

Each native Plex owns its own Footprints. A second Plex has a different trail, even if it begins at the same node. Moving a Plex between windows retains its trail; **closing that Plex or restarting Obsidian clears it**. Duplicate views start with a fresh trail.

Footprints records navigation, **not the structure of your notes**. It is a chronological list, not a visual, branching breadcrumb tree, timeline or metro map. A renamed note's saved visits follow its updated location; a deleted or unavailable target can appear unavailable and cannot be reopened by selecting it.

For persistent navigation and gate-to-pin actions, see [[02 Navigate and explore/Past nodes and pins]]. To use the trail while developing an idea, try [[07 Use cases/Rediscover and remember your notes]].

[Implementation and validation: PR #187](https://github.com/zsviczian/kplex/pull/187) · [K-Plex navigation guide](https://github.com/zsviczian/kplex/blob/3df08a15f7002ed60a2452286ee1f8044cb97203/README.md#search-history-and-pins).
