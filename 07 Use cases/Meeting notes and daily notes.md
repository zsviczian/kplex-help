---
tags:
- kplex-help/example
- kplex/use-cases
- kplex/dates
Guide:
- '[[07 Use cases/Use cases]]'
Child:
- '[[09 Showcase examples/Example - Date and a daily note]]'
Related:
- '[[03 Build and edit/Date properties and daily notes]]'
- '[[07 Use cases/Sequential workflows]]'
---
A date is useful **context**, but it is not necessarily a Parent in every workflow. K-Plex lets you decide.

**Meeting workflow:** Put a native `Date` property on a meeting note. If **Default Date role = Parent**, its daily note provides the broader calendar context *above* the meeting. Keep agenda items as Children and related decisions as Friends.

**Journal workflow:** If the dated note is a step in a sequence, consider an explicit `Previous`/`Next` relationship between journal entries. You can instead configure a Date field to use Previous/Next, but only when that role genuinely models the relationship you intend.

**Multiple date fields:** Set **Default Date role** for your general case, then explicitly map `Meeting Date`, `Reviewed on`, or other individual Date property names in **Ontology → Relationship fields** if you need a different direction. An explicit **Hidden** mapping can prevent an unrelated date from becoming a graph edge.

Try [[09 Showcase examples/Example - Date and a daily note|Example - Date and a daily note]], then open [[03 Build and edit/Date properties and daily notes|Date properties and daily notes]] to see the exact conditions and limits. The example is intentionally static; your personal daily notes use your own file naming and location.

> [!warning] Avoid accidental chronology
> Dates describe **when** something happened. `Previous` and `Next` usually describe an **explicit order**. Do not treat all Date properties as sequence edges without checking whether that is the meaning you want.
