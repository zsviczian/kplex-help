---
aliases:
- How to use this help vault
tags:
- kplex-help/reference
- kplex/getting-started
- kplex/ontology
Guide:
- '[[00 Start Here/Get started]]'
Friend:
- '[[05 Personalize and workspace/Node styles from help tags]]'
Next:
- '[[01 Core concepts/Core concepts]]'
Related:
- "[[09 Showcase examples/Facets demonstrations]]"
---
# How to use this help vault

Try K-Plex while learning it. These notes are both a readable guide and a live graph: follow a topic in Markdown or make it the center of the canvas.

## Three ways to browse

1. **By goal:** [[00 Start Here/Choose a topic|Choose a topic]] offers thirteen curated paths, from first steps through graph filtering, research, keyboard workflows, date relationships and troubleshooting.
2. **By feature:** use the folders and section hubs on the help home for reference-style reading.
3. **By relationship:** center a note in K-Plex; follow Parents up, Children down, Friends to the left, Challengers to the right, and Previous/Next through ordered steps.

## The help ontology

| Field in notes | K-Plex role | How it is used |
| --- | --- | --- |
| `Parent`, `Guide` | Parent ↑ | broader category or guide; paired with Child and Explains |
| `Child`, `Explains` | Child ↓ | subtopic, step or topic explained |
| `Friend`, `Related` | Friend ← | useful neighboring subject |
| `Challenger`, `Watch out` | Challenger → | caveat, counterpoint or limit |
| `Previous` | Previous ← | preceding sequential step; paired with Next |
| `Next` | Next → | following sequential step |

A *property name* is not the same thing as a *role*. K-Plex maps several property names to the same direction. Try [[01 Core concepts/Ontology and relationship fields|Ontology and relationship fields]] to see the difference.

## Try the configured pairs

The vault uses **Guide/Explains**, **Parent/Child**, and **Previous/Next**. Center [[00 Start Here/K-Plex Help]], follow a guide connection, then come back: the caption describes the connection from the endpoint you are viewing. No duplicated note property is required.

Inspect the configuration in [[03 Build and edit/Manage and clean up ontology]]. Keep the ordinary field names in note frontmatter; the slash syntax is a Settings convention only. **Learn more** remains an additional Child field used in the release notes.

## Tags and appearance

Each note has a help-style tag such as `#kplex-help/concept`, `#kplex-help/how-to`, `#kplex-help/path`, or `#kplex-help/caution`, plus one or more topic tags. The bundled node styling makes the type of help visible in the canvas; [[05 Personalize and workspace/Node styles from help tags|Node styles from help tags]] explains the scheme.

## Folders, images and URLs

Folders keep help familiar in the Obsidian file explorer. The images in `Assets/` are attached from Markdown, and URL nodes introduce GitHub, community and reference sites. Folder and tag nodes are optional visibility settings; this vault does not require them to be displayed to navigate the ontology.

> [!tip] A route is not a duplicate manual
> Discovery paths have **Explains** relationships to existing reference notes. Their reading order is written as numbered steps so it does not conflict with each reference note's own **Previous/Next** relationships.

## This vault demonstrates recent features

The [[00 Start Here/Recently added features|recent features hub]] links to the Action Manager, graphical keyboard navigation, fullscreen/Zen and Date-property role settings. There is also a **real date example** at [[09 Showcase examples/Example - Date and a daily note|Example - Date and a daily note]]. For practice, use [[10 Discover by topic/11 Work without the mouse|keyboard path]], [[10 Discover by topic/12 Connect dates and daily notes|dates path]] or [[10 Discover by topic/13 Present and concentrate|focus path]].

## Build a view around your own question

The default **Compass** view teaches the relationship vocabulary used throughout the help. **Mind Map** follows a hierarchy from a stable root. **Facets** lets you define categories for the direct neighbors of a note.

Open [[09 Showcase examples/Facets demonstrations|the four Facets demonstrations]] to see property, tag, note-type and category-rule sources with different arrangements. Each preset has a useful starting note and its own help. Treat them as examples for a workflow you define, rather than a system you must adopt.
