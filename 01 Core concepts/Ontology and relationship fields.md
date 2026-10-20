---
aliases:
- Ontology and relationship fields
tags:
- kplex-help/concept
- kplex/ontology
- kplex/relationships
Friend:
- '[[03 Build and edit/Create a relationship]]'
- '[[03 Build and edit/Manage and clean up ontology]]'
Previous:
- '[[01 Core concepts/Relationship roles]]'
Next:
- '[[01 Core concepts/Relationship sources and inference]]'
---
# Ontology and relationship fields

Want the map to use words that make sense for your work, such as Guide, Example or Risk? Assign your property names to relationship roles so their position explains what they mean.

![[Image - Ontology.png]]

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

![[Assets/Screenshot - Ontology pairs.png]]

*The live manager finds the Guide/Explains pair by either property name.*

## Pairs describe the two ends of one relationship

This help vault is configured with three pairs:

| Pair | From the first field's note | From the other endpoint |
| --- | --- | --- |
| Guide / Explains | Guide points up to the guide | Explains names the guide’s connection to its topic |
| Parent / Child | Parent points up to the broader note | Child names the parent’s connection to its detail |
| Previous / Next | Previous points to the preceding step | Next names the forward connection from that step |

The `/` belongs in **K-Plex Settings**, not in your Markdown property name. Keep using ordinary `Guide`, `Explains`, `Parent`, `Child`, `Previous` or `Next` properties in the notes.

For example, a topic can declare its Guide/Explains relationship once:

```yaml
Guide:
  - "[[00 Start Here/K-Plex Help]]"
```

From the topic you follow **Guide** to the help home. From the help home the inverse connection can be captioned **Explains**. You do not need to add a mirrored property to the other note. The ordinary properties in your notes remain unchanged.

To inspect a real pair, open **Settings → K-Plex → Ontology → Manage ontology**, search for **Guide**, and open the row. **Pair with** shows **Explains**. Alternatively, a role field in Settings can contain `Guide/Explains` once. Prefer the structured editor when learning the syntax; it validates roles and partner choices.

Read [[03 Build and edit/Manage and clean up ontology]] to find documents using either physical field. Changing a displayed inverse caption does not rename properties across your vault.

## Date properties are a special case

An Obsidian Date value that resolves to a Daily Note has a configurable **Default Date role** (initially Parent). A configured named field mapping—even **Hidden**—overrides that fallback. Unlike a wikilink property, a Date scalar is edited in Obsidian’s property editor. Read [[03 Build and edit/Date properties and daily notes|Date properties and daily notes]].
