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
# Ontology autocomplete

Add meaningful relationships while writing, without remembering every property name. Use ontology suggestions to insert a configured field and keep typing.

![[Assets/Screenshot - Ontology suggestions.png]]

*The editor-suggester Settings page shows the triggers for each direction and for all ontology fields.*

## Add a field while writing

1. Open **Settings → K-Plex → Ontology → Editor suggester** and enable suggestions.
2. Check the triggers for Parent, Child, Friend, Challenger, Previous, Next and all ontology fields. Use your configured values rather than copying another vault's shortcuts.
3. In a Markdown editor, type a trigger and part of a field name. Select a suggestion, then add a note link with Obsidian's usual `[[link]]` syntax.

The suggestion inserts a property name. Its configured role decides where the linked note appears in K-Plex. You can also use Obsidian's normal Properties editor.

## When the right word is missing

Use [[03 Build and edit/Manage and clean up ontology|Manage ontology]] to assign a field or pair its opposite meaning. If suggestions do not appear, check that the feature is enabled and the trigger matches your saved setting.

For dates, use [[03 Build and edit/Date properties and daily notes|Date properties and daily notes]]: a Date value is different from a note-link list.
