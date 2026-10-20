---
tags:
  - kplex-help/release-notes
  - kplex/unreleased
Guide:
  - "[[11 Release notes/Release notes]]"
Explains:
  - "[[01 Core concepts/Ontology and relationship fields]]"
  - "[[03 Build and edit/Manage and clean up ontology]]"
  - "[[06 Indexing and troubleshooting/On demand vs Eager]]"
  - "[[04 Filter and focus/Expand a note into sections]]"
  - "[[05 Personalize and workspace/Colors and themes]]"
  - "[[05 Personalize and workspace/Layout density and typography]]"
  - "[[02 Navigate and explore/Footprints and breadcrumbs]]"
  - "[[07 Use cases/Garden your vault]]"
Previous:
  - "[[11 Release notes/K-Plex 0.1.3]]"
---
# K-Plex 0.2.0 — Your knowledge, your workspace

K-Plex is becoming more than a way to navigate connected notes. Organize knowledge directly from the graph, keep different tasks in separate Plex views, retrace an exploration, and make the workspace fit your preferred appearance.

### Organize your vault while exploring

Bring notes from Obsidian into K-Plex and drag them between views or into a Markdown draft. Move supported notes or folders to folder destinations, assign tags, and create new notes or placeholders in a chosen location. The graph becomes a place to **do the organizing**, not merely inspect its result.

Learn more:: [[03 Build and edit/Drag drop and reclassify]] · [[03 Build and edit/Create notes and placeholders]]. [Implementation: PR #177](https://github.com/zsviczian/kplex/pull/177).

### Keep two lines of thought open

Work with multiple independent Plex views and their own document synchronization and Sidecar associations. For example, keep your project or article centered in one Plex while following references in another. Fold the Plex tab group when you want more room for the document.

Learn more:: [[05 Personalize and workspace/Note-tab synchronization]] · [[05 Personalize and workspace/Sidecar]]. [PR #187](https://github.com/zsviczian/kplex/pull/187) · [PR #173](https://github.com/zsviczian/kplex/pull/173).

### Garden notes without leaving the graph

Obsidian's built-in **File properties** pane now follows the note at the center of an active Plex when the pane is unpinned and ungrouped. Browse related notes, update properties such as status or maturity, and use Graph Lenses to see those classifications reflected in the graph. It turns reviewing and improving notes into a fluid activity rather than repeatedly opening files and finding their metadata.

Alongside tag and Note Type assignment through drag-and-drop, this gives you two complementary ways to garden your knowledge: **classify notes quickly** and **refine their metadata while exploring**.

Learn more:: [[05 Personalize and workspace/Note-tab synchronization]] · [[03 Build and edit/Drag drop and reclassify]] · [[04 Filter and focus/Graph Lenses]] · [[07 Use cases/Garden your vault|Garden your vault — one note at a time]]. [File properties: PR #171](https://github.com/zsviczian/kplex/pull/171) · [native tag actions: PR #177](https://github.com/zsviczian/kplex/pull/177).

### Retrace your visit trail with Footprints

Each Plex now records its own **complete session visit trail**, including repeated visits. Revisit earlier stops, start a fresh trail, or copy it as Markdown. Footprints is **not persisted**, unlike the shared saved Past nodes history and pins. A branching visual map of the journey is not included.

Learn more:: [[02 Navigate and explore/Footprints and breadcrumbs]]. [PR #187](https://github.com/zsviczian/kplex/pull/187).

### Make K-Plex look and feel like your Obsidian workspace

Use native Obsidian theme colors, named appearances and paired light/dark colors. Reset basic colors independently from the semantic styles of your nodes and relationships. Adjust the layout and reduce visual noise with more deliberate hover behavior, including Alt/Option previews of crosslinks that are normally hidden.

Learn more:: [[05 Personalize and workspace/Colors and themes]] · [[05 Personalize and workspace/Visibility and connector styling]] · [[05 Personalize and workspace/Layout density and typography]]. [PR #158](https://github.com/zsviczian/kplex/pull/158) · [PR #181](https://github.com/zsviczian/kplex/pull/181).

### Describe a connection from either end

Pair ordinary ontology fields such as **Guide / Explains**, **Parent / Child**, or **Previous / Next**. K-Plex can use the opposite caption when you view the connection from the other end, without requiring you to write the relationship into both notes. The help vault now uses these three pairs, so you can explore real examples rather than a special demonstration format.

Learn more:: [[01 Core concepts/Ontology and relationship fields]]. [PR #190](https://github.com/zsviczian/kplex/pull/190).

### Find and clean up relationship properties

**Manage ontology** brings assigned and unassigned fields into one searchable list. Open a field and select **Show documents** to see where it is used, filter the results, open a document in K-Plex or a new Obsidian tab, or copy the list as Markdown.

After correcting a misspelled field in your notes, use **Refresh counts** to remove zero-use entries from **Unassigned**. Deliberately configured fields remain even when unused. This helps you tidy the vocabulary without losing intentional assignments.

Learn more:: [[03 Build and edit/Manage and clean up ontology]] · [[07 Use cases/Garden your vault]]. [PR #194](https://github.com/zsviczian/kplex/pull/194).

![[Assets/Screenshot - Ontology documents.png]]

*Find the notes behind a field before changing your ontology.*

### Choose when each device starts indexing

Desktop, tablet and phone now have independent startup and strategy settings under **Settings → K-Plex → Indexing config**.

| Device | Default start | Default strategy |
| --- | --- | --- |
| Desktop | When the plugin starts | Eager |
| Tablet | When a Plex first opens | On demand |
| Phone | When a Plex first opens | On demand |

Changes apply after restarting Obsidian or reloading K-Plex. A restored Plex counts as open. Waiting until first use postpones preparation, including saved index loading; it can make the first opening take longer. It is not a promise of faster full-vault indexing.

Learn more:: [[06 Indexing and troubleshooting/On demand vs Eager]]. [PR #195](https://github.com/zsviczian/kplex/pull/195).

### Explore long notes with a more readable outline

Expanding a note into sections now keeps ordinary links under their headings. Section clusters respond more usefully to density settings, show the note's available gate counts, and preview the relevant heading with Ctrl/Cmd-hover—even if you press the modifier after moving the pointer onto the node. Ctrl/Cmd-wheel still zooms when the pointer is over a scrollable region.

Text rendering is clearer after zooming and scrolling, with more room for large glyphs. One-sided layout puts Friends and Challengers in **one shared list** on the left while preserving their different relationship meanings.

Learn more:: [[04 Filter and focus/Expand a note into sections]] · [[05 Personalize and workspace/Layout density and typography]]. [#162](https://github.com/zsviczian/kplex/pull/162) · [#149](https://github.com/zsviczian/kplex/pull/149) · [#189](https://github.com/zsviczian/kplex/pull/189).

## Under the hood: fewer interruptions

Settings updates arriving through Obsidian Sync can apply to the running plugin without immediately writing the same settings back. Navigation, indexing and graph presentation behave more consistently during startup, late ontology processing and normal Markdown autosaves. Diagnostics now capture more useful session activity when reporting a problem.

Learn more:: [[06 Indexing and troubleshooting/Understanding index status]] · [[06 Indexing and troubleshooting/Rebuild purge and diagnostics]]. Sources: [#182](https://github.com/zsviczian/kplex/pull/182), [#180](https://github.com/zsviczian/kplex/pull/180), [#183](https://github.com/zsviczian/kplex/pull/183), [#186](https://github.com/zsviczian/kplex/pull/186), [#174](https://github.com/zsviczian/kplex/pull/174).

Visible ontology edits can update a stationary Plex while unrelated startup indexing continues. This corrects a confirmed case where a new relationship stayed inferred until navigating away and back; it does not claim to resolve every possible startup or application-freeze issue.

## Try the changes in this vault

Start with [[01 Core concepts/Ontology and relationship fields]], inspect the live pairs in [[03 Build and edit/Manage and clean up ontology]], then follow the **Explains** links from this release to the guides. For an everyday workflow, try [[07 Use cases/Garden your vault]].
