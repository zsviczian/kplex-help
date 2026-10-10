---
tags:
- kplex-help/path
- kplex/discovery
- kplex/dates
- kplex/ontology
Explains:
- '[[03 Build and edit/Date properties and daily notes]]'
- '[[01 Core concepts/Ontology and relationship fields]]'
- '[[07 Use cases/Meeting notes and daily notes]]'
- '[[09 Showcase examples/Example - Date and a daily note]]'
- '[[03 Build and edit/Connection details and evidence]]'
Related:
- '[[10 Discover by topic/03 Model and edit relationships]]'
- '[[10 Discover by topic/05 Organize projects and sequences]]'
---
> **Your goal:** Make a Date property a meaningful relationship to a daily note, without rewriting your date values.

## Follow the trail

1. [[03 Build and edit/Date properties and daily notes|Date properties and daily notes]] — configure a default Date role and understand its limits.
2. [[01 Core concepts/Ontology and relationship fields|Ontology and relationship fields]] — learn how a named field overrides the fallback.
3. [[07 Use cases/Meeting notes and daily notes|Meeting notes and daily notes]] — choose a useful relationship meaning for dates.
4. [[09 Showcase examples/Example - Date and a daily note|Example - Date and a daily note]] — open the included sample note and day.
5. [[03 Build and edit/Connection details and evidence|Connection details and evidence]] — inspect source evidence before editing.

## Try it in the help vault

Center the sample, check its Date field, then open **Settings → K-Plex → Plex behavior → Relationship behavior → Default Date role**. With **Parent** selected, the daily note should provide upward context if Obsidian's Daily Notes target resolves. Try **Friend**, then restore Parent.

> [!important] Configured ontology wins
> If `Date` is already assigned explicitly to a role—even Hidden—the dropdown's fallback does not override it. The sample's extra Parent ontology link to its help section is separate from its Date-derived link.

Continue to [[10 Discover by topic/03 Model and edit relationships|Model and edit relationships]] or [[00 Start Here/Choose a topic|all routes]].
