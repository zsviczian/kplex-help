---
tags:
  - kplex-help/release-notes
Guide:
  - "[[11 Release notes/Release notes]]"
Previous:
  - "[[Release 0.3.0]]"
Explains:
  - "[[03 Build and edit/Manage and clean up ontology]]"
  - "[[03 Build and edit/Connection details and evidence]]"
  - "[[02 Navigate and explore/Explore folders]]"
  - "[[02 Navigate and explore/Mind Map]]"
  - "[[02 Navigate and explore/Editor node and web pages]]"
  - "[[06 Indexing and troubleshooting/Understanding index status]]"
Related:
  - https://github.com/zsviczian/kplex/pull/228
  - https://github.com/zsviczian/kplex/pull/230
  - https://github.com/zsviczian/kplex/pull/234
  - https://github.com/zsviczian/kplex-help
Note type: ReleaseNotes
---
Create the relationship fields you need without leaving the connection you are working on. This update also keeps folder browsing and visible relationships more responsive during indexing, and lets you continue editing as you move through a Mind Map.

## Define a relationship without a detour

When configuring **Pair with**, type a new property name and choose **Create … as paired field**. Save to define both sides together, with the partner assigned the reciprocal role. You no longer need to add the property to a note first just to make it available for pairing.

The **Note property** selector in **Add connection ontology** also offers **Create ontology…**. Define the new field, optionally give it a partner, then return to the connection with that field selected. Creating the definition saves your vocabulary; confirming the connection applies the property to the note. Existing relationship properties and Markdown-body links are preserved.

See [[03 Build and edit/Manage and clean up ontology|managing relationship fields]] and [[03 Build and edit/Connection details and evidence|adding ontology to a connection]].

## Keep exploring while the index catches up

Ordinary note edits and file moves are less likely to restart broad index verification. While wider recovery continues, visible notes can use available metadata to reflect the current ontology, rather than waiting for the whole vault to finish. Missing information can still leave a neighborhood incomplete.

Folder browsing follows Obsidian's current file and folder structure. Adding or moving a file into a folder no longer temporarily clears its existing contents from the canvas while note indexing catches up. Folder counts and sibling lists stay consistent when browsing the same area in two Plexes.

The startup indicator also clears when verification finishes, fixing a case where **Verifying cached notes** could remain at 99% after the work had completed.

See [[02 Navigate and explore/Explore folders|exploring and organizing folders]] and [[06 Indexing and troubleshooting/Understanding index status|understanding index status]].

## Keep writing as you move through a Mind Map

With the central Markdown note open in a node editor, click another Markdown note to bring it to the center. K-Plex saves the previous note and opens the new center in the same reading or editing mode, preserving the editor's dimensions. You can continue to another note even while the next editor is still loading.

If saving fails, the current editor stays available so you can recover your work. Clicking a note centers it; the branch chevron folds or unfolds it. A notice about folding away an open editor now describes that action rather than appearing when you simply navigate to a new center.

See [[02 Navigate and explore/Mind Map|Mind Map]] and [[02 Navigate and explore/Editor node and web pages|reading and writing inside the canvas]].

## Learn more

Explore the [K-Plex Help vault](https://github.com/zsviczian/kplex-help) for guides, screenshots and working examples.

Changes: [ontology creation](https://github.com/zsviczian/kplex/pull/228), [indexing and folder recovery](https://github.com/zsviczian/kplex/pull/230), and [index status and Mind Map editing](https://github.com/zsviczian/kplex/pull/234).
