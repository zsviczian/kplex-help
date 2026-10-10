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
A visible K-Plex connection can be supported by more than one source. Depending on the node types and your settings, evidence can include frontmatter properties, inline properties, Markdown links, unresolved links, dates, URLs, folder hierarchy, tag hierarchy and other supported sources.

An **explicit ontology** tells K-Plex the intended role. An **inferred** relationship is resolved when K-Plex can see a connection but no explicit ontology gives it a stronger meaning. The same visible edge can have multiple pieces of evidence behind it.

This distinction matters when editing. K-Plex does not create a separate database of relationship notes: the Markdown files remain the source of truth. Use [[03 Build and edit/Connection details and evidence|Connection details and evidence]] to see why a relationship exists before changing it.

> [!tip]
> When a relationship surprises you, inspect the evidence first. The graph is a projection of your sources; understanding the source is usually more useful than forcing the display.

## Scalar Date evidence

A recognized Date property linked to an existing Daily Note is tracked as Date-source evidence, not as a conventional `[[wikilink]]`. K-Plex can use its default Date role or a field-specific ontology assignment, preserving normal configured-field precedence. Learn more in [[03 Build and edit/Date properties and daily notes|Date properties and daily notes]].

## Why gate counts may differ from connector paths

Gate badges count **semantic relationship endpoints**, not the number of drawing attachments or connector lines used to lay out the scene. Filtering, presentation sides and partial source loading should not multiply a relation simply because it can be drawn through several positions. A note that has one Challenger should count as one such semantic connection, not several copies of that edge.

[Correction: PR #112](https://github.com/zsviczian/kplex/pull/112).
