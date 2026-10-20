---
aliases:
- Glossary
- K-Plex terms
tags:
- kplex-help/reference
- kplex/getting-started
- kplex/concepts
Related:
- '[[01 Core concepts/Relationship roles]]'
- '[[06 Indexing and troubleshooting/How indexing works]]'
- '[[00 Start Here/Choose a topic]]'
- '[[02 Navigate and explore/Keyboard shortcuts reference]]'
- '[[03 Build and edit/Date properties and daily notes]]'
- '[[05 Personalize and workspace/Fullscreen and Zen mode]]'
---
# Glossary

Seen an unfamiliar word in K-Plex? Use this reference to understand the label and find the guide that shows it in action.

| Term | Meaning |
| --- | --- |
| **Plex** | The relationship map centered on one current note or node. |
| **Center** | The item whose immediate relationships organize the view. |
| **Neighbor** | A visible item connected to the center. |
| **Gate** | A directional group of relationships, including a count and expansion controls. |
| **Ontology** | The mapping from property names to roles such as Parent, Friend and Challenger. |
| **Evidence** | A source occurrence (property, link, body field and so on) that supports a visible connection. |
| **Inferred connection** | A relationship K-Plex can derive without an explicit ontology field. |
| **Placeholder / ghost** | An unresolved link to a note that does not yet exist as a file. |
| **Past nodes / pins** | Past nodes records where you went; pins keep chosen shortcuts available. |
| **Graph Lens** | A reusable filter or style rule for the *visible* Plex. |
| **On demand / Eager** | Two ways to prepare relationships: as you explore, or across the vault in the background. |
| **URL inventory** | Web links K-Plex has discovered; it can remain incomplete while local graph navigation works. |
| **Sidecar** | A normal Obsidian document pane positioned beside the graph. |
| **Graph focus** | Keyboard ownership for K-Plex graph navigation, separate from a search field or editor. |
| **Type to select** | Temporary, case-insensitive phrase matching of **visible** node labels on the focused graph. |
| **K-Plex command palette** | A searchable list of actions available to the current Plex, distinct from Obsidian's palette. |
| **Action Manager** | Shared action catalog behind commands, menus, buttons, local shortcuts and the K-Plex palette. |
| **Graph-local shortcut** | A key binding interpreted only while the relevant K-Plex surface has focus. |
| **Published command** | A K-Plex action exposed to Obsidian's Command Palette, separately from local shortcut assignment. |
| **Physical vs logical key** | A shortcut matched by key position versus the character the keyboard produces. |
| **Shortcut conflict** | Two bindings competing for the same local context; ambiguous K-Plex keys execute neither action. |
| **Fullscreen** | Session-only desktop mode that covers the Obsidian workspace without invoking system fullscreen. |
| **Zen mode** | Session-only mode hiding K-Plex's toolbar, pins and history while retaining graph controls. |
| **Default Date role** | Fallback Parent/Friend/Child/Challenger/Previous/Next role for an unconfigured native Date property linked to a Daily Note. |
| **Explicit field ontology** | A role assigned to a named property. It overrides fallback Date roles, even when the field is Hidden. |
| **Local graph ready** | The requested Plex is prepared; this does not promise a complete URL inventory or full-vault background pass. |

Continue with [[01 Core concepts/The spatial relationship model|The spatial relationship model]] for the positions, [[01 Core concepts/Relationship sources and inference|Relationship sources and inference]] for where connections come from, or [[00 Start Here/Choose a topic|Choose a topic]] for a task-led route.

## Feature-specific explanations

[[02 Navigate and explore/Keyboard shortcuts reference|Keyboard shortcuts reference]] · [[05 Personalize and workspace/Fullscreen and Zen mode|Fullscreen and Zen mode]] · [[03 Build and edit/Date properties and daily notes|Date properties and daily notes]] · [[06 Indexing and troubleshooting/Understanding index status|Index status]]

## New terms in the latest updates

| Term | Meaning |
| --- | --- |
| **Single-source removal** | Confirmed removal of one eligible frontmatter relationship occurrence, without automatically removing other evidence on the same edge. |
| **Gate count** | How many related notes belong to that gate; several sources can support one connection. |
| **Drawing/Markdown representation** | An Excalidraw file's selected display mode; passive same-file Sidecar/tab follow preserves the deliberate choice. |
| **Quick Filter cross-links toggle** | Show or hide extra connections in this Plex. This choice is not saved across a restart. |
| **Label-length limit** | Maximum characters in a regular node label, separate from density. This help vault sets it to 100. |
| **Cache inactivity recovery** | Retirement of startup restore work that stops making progress; not a total time limit on healthy indexing. |

Explore [[03 Build and edit/Remove one relationship source|Single-source removal]], [[05 Personalize and workspace/Visibility and connector styling|cross-links]], and [[03 Build and edit/Excalidraw integration|representation switching]] in more detail.
