---
tags:
- kplex-help/how-to
- kplex/ontology
- kplex/relationships
Guide:
- '[[03 Build and edit/Build and edit]]'
Related:
- '[[01 Core concepts/Ontology and relationship fields]]'
- '[[03 Build and edit/Create a relationship]]'
- '[[05 Personalize and workspace/Actions and shortcuts]]'
---
K-Plex can suggest configured ontology fields while you edit a Markdown note, so adding a Parent, Child, Friend or other relationship takes less typing.

1. Open **Settings → K-Plex → Ontology → Editor suggester** and enable the ontology suggester.
2. Check or customize the triggers for **Parent, Child, Friend (left), Challenger (right), Previous, Next**, and the **all-ontology** trigger.
3. In a Markdown editor, type the configured trigger and choose a field from the suggestions. Insert your reference using the normal note-link syntax or property editing method.
4. When editing an existing property, use K-Plex's **ontology field assignment commands** to categorize the property without creating a second field name manually.

A trigger is a shortcut to a **field name**, not a new relationship type. The configured field still decides the link's spatial meaning; see [[01 Core concepts/Ontology and relationship fields|Ontology and relationship fields]].

The suggester now uses **bounded literal matching** rather than repeatedly applying a backtracking pattern to an arbitrarily long editor line. This addresses a reported long-paste freeze without changing the configured triggers or suggestion insertion. If you can still reproduce a freeze, report the exact K-Plex version and steps through [GitHub issues](https://github.com/zsviczian/kplex/issues).

> [!tip] When editing properties
> Obsidian's own property editor also works; K-Plex reads the resulting field. For a Date-type field, consult [[03 Build and edit/Date properties and daily notes|Date properties and daily notes]] because Date values are not standard wikilink lists.
