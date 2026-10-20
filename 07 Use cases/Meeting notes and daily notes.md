---
Note type: Use case
aliases:
- Reconstruct what happened and why
- Explore your knowledge through dates and daily notes
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
- '[[07 Use cases/Projects and decisions]]'
---
# Meeting notes and daily notes

Trying to remember what was decided, when it happened and which project it belonged to? Connect meetings to both their project and their day.

![[Assets/Screenshot - Date connections.png]]

*The Date example connects to its daily note as well as its broader topic. These are separate reasons for the two relationships.*

**Outcome:** You can recover the context of a meeting or decision by following either the project it belongs to or the day it happened.

**Setup:** Configure the relevant Date properties and Daily Notes.

## Try it: reconstruct last week's project decisions

Keep a separate note for a meeting that produced useful decisions. Give it a native **Date** property, connect it to its project, and link the resulting decisions or actions. Use your configured daily-note naming and location, with an existing daily note for the date you are testing.

Start from the project and navigate to the meeting to revisit its rationale. Then follow its date relationship to see the day's other connected work. Reverse the journey from the daily note when you remember when something happened but not the project or filename.

Write the conclusion back into the project or decision note: what changed, why it changed and what still needs follow-up. The graph helps you recover the context; the notes retain the explanation.

**Done when:** You can answer “What did we decide, why, and when?” without searching through every daily note.

## A date is context, not necessarily a Parent

With **Default Date role = Parent**, the daily note provides calendar context above the meeting. Agenda items can remain Children and related decisions Friends. Another workflow may benefit from a lateral Date role instead.

Set the default for your general case, then map individual Date property names such as `Meeting Date` or `Reviewed on` under **Settings → K-Plex → Ontology → Manage ontology** when their meaning differs. An explicit Hidden mapping can prevent an unrelated date from becoming a graph edge.

For a deliberate journal chain, connect entries with Previous/Next. Do not assume that every date is a sequence or that K-Plex sorts your project into a timeline automatically.

Try [[09 Showcase examples/Example - Date and a daily note]], then read [[03 Build and edit/Date properties and daily notes]] for the exact conditions and limits. The example is intentionally static; your own vault uses its own daily-note configuration.

> [!warning] Avoid accidental chronology
> Dates describe when something happened. Previous and Next describe an explicit order. A date-scoped automatic Wander retrospective is not part of this workflow.
