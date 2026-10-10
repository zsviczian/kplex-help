---
aliases:
- Ontology and relationship fields
tags:
- kplex-help/concept
- kplex/ontology
- kplex/relationships
Friend:
- '[[03 Build and edit/Create a relationship]]'
Previous:
- '[[01 Core concepts/Relationship roles]]'
Next:
- '[[01 Core concepts/Relationship sources and inference]]'
---
![[Image - Ontology.png]]

**Ontology** maps a property name to a spatial role. A note property named `Related` does not need to be literally called `Friend` to appear on the **left**; K-Plex can classify `Related` as Friend ontology.

## Example from this vault

```yaml
Related:
  - "[[01 Core concepts/Relationship roles]]"
Watch out:
  - "[[01 Core concepts/What K-Plex is not]]"
```

In this help vault, `Related` maps to **Friend** (left) and `Watch out` maps to **Challenger** (right). These are deliberate, editable examples of meaningful property names.

K-Plex supports YAML/frontmatter properties and compatible Dataview-style inline fields **without needing the Dataview plugin**. You can configure Parent, Child, Friend, Challenger, Previous, Next, Hidden and excluded metadata fields in K-Plex's Ontology settings. Property assignment is also available from context menus and the Command Palette.

> [!note] An ontology role is not a guarantee about every link
> Ordinary Markdown links, folders, tags, URLs and other sources can also contribute to the graph. K-Plex resolves them using source evidence and precedence, rather than treating every mention as an explicit ontology relationship.

Continue with [[01 Core concepts/Relationship sources and inference|Relationship sources and inference]] or follow [[10 Discover by topic/03 Model and edit relationships|Model and edit relationships]].

## Date properties are a special case

An Obsidian Date value that resolves to a Daily Note has a configurable **Default Date role** (initially Parent). A configured named field mapping—even **Hidden**—overrides that fallback. Unlike a wikilink property, a Date scalar is edited in Obsidian’s property editor. Read [[03 Build and edit/Date properties and daily notes|Date properties and daily notes]].
