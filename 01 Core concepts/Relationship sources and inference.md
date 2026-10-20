---
aliases:
- Relationship sources and inference
tags:
- kplex-help/concept
- kplex/relationships
- kplex/evidence
Friend:
- '[[03 Build and edit/Connection details and evidence]]'
Previous:
- '[[01 Core concepts/Ontology and relationship fields]]'
Next:
- '[[01 Core concepts/Node types]]'
---
# Relationship sources and inference

Wondering why two notes are connected, or why a line remains after an edit? Inspect the sources behind the relationship before deciding what to change.

![[Assets/Screenshot - Reading relationships.png]]

*The research example keeps a question and its surrounding context together. Open a neighbor to explore it.*

## Look behind the line

A connection may come from a note property, an inline field, a body link, a tag, a folder, a date or a website reference. Several sources can support the same line.

An **explicit relationship** uses a property assigned to a role such as Parent or Friend. An **inferred relationship** is a connection K-Plex can see without that explicit meaning. Your [[01 Core concepts/Ontology and relationship fields|ontology settings]] tell K-Plex how to interpret property names.

For example, a note might point to the same project from its Parent property and from a paragraph in the body. Removing the property leaves the body reference. The connection can remain, although its meaning or appearance may change.

## Inspect before changing

Right-click a connector, or long-press on touch, and open **Connection details…**. Follow the source to understand why the relationship exists. Then [[03 Build and edit/Remove one relationship source|remove one editable source]] or edit the note itself.

A Date relationship is different from a wikilink list: change its value in Obsidian's Date property editor. See [[03 Build and edit/Date properties and daily notes]].

Gate badges count related endpoints, not how many source occurrences or line segments support them. Counts can be incomplete while the current neighborhood is still loading; [[06 Indexing and troubleshooting/Understanding index status|check the status]] if a number surprises you.
