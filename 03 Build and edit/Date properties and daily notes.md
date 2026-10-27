---
tags:
- kplex-help/how-to
- kplex/ontology
- kplex/dates
Guide:
- '[[03 Build and edit/Build and edit]]'
Related:
- '[[01 Core concepts/Ontology and relationship fields]]'
- '[[01 Core concepts/Relationship sources and inference]]'
- '[[07 Use cases/Meeting notes and daily notes]]'
- '[[03 Build and edit/Connection details and evidence]]'
---
# Date properties and daily notes

Connect a meeting or event to the day it happened. A Date property can link it to your Daily Note without adding a separate wikilink.

![[Assets/Screenshot - Date connections.png]]

*The Date example connects to its daily note as well as its broader topic. These are separate reasons for the two relationships.*

## Choose a default role

1. Enable Obsidian's **Daily notes** core plugin and ensure the target daily note follows your configured date format and folder. Give the source property Obsidian's **Date** property type.
2. Open **Settings → K-Plex → Canvas behavior → Relationship behavior → Default Date role**.
3. Choose **Parent** (default), **Friend**, **Child**, **Challenger**, **Previous**, or **Next**. This is the fallback for Date properties **without** a configured ontology role.
4. Navigate to a note with a recognized Date value and an existing resolvable Daily Note. K-Plex shows the relationship in the chosen direction. **Connection details** retains its Date provenance.

Example (the field's value is a date, **not** a wikilink):

```yaml
---
Date: 2026-10-09
---
```

With **Parent** as the fallback, a meeting note dated `2026-10-09` can show `2026-10-09.md` **above** it. If you prefer the daily note as a **Child**, change the fallback to Child. **Changing the role reinterprets the relationship**, not the underlying Markdown date or the Daily Notes naming rules.

## Override the default for a particular field

Suppose `Meeting Date` should always be a **Friend**, but other Date properties should be **Parent**. In **Settings → K-Plex → Ontology → Relationship fields**, assign `Meeting Date` to Friend. That explicit field definition takes precedence over **Default Date role**. The same principle applies to Parent, Child, Challenger, Previous, Next—and **Hidden**. A field explicitly marked Hidden remains hidden, regardless of the fallback.

K-Plex keeps Date-source evidence distinct from an ordinary linked property. **Do not use the graph's direct wikilink relink/unlink workflow to edit a scalar Date value**; change the Date property in Obsidian’s property editor. A reciprocal body link from the daily note does not automatically replace the configured Date relationship.

> [!important] A Date is not an arbitrary text string
> The automatic relationship depends on Obsidian recognizing the value as a Date with a resolvable Daily Notes target. It does not automatically create missing daily-note files or turn every date-looking text field into a new relationship. It also does not alter your Obsidian Daily Notes formatting.

## See the feature in this vault

Open [[09 Showcase examples/Example - Date and a daily note|Example - Date and a daily note]] and the root daily note `2026-10-09.md`. This help vault enables Obsidian's Daily notes core plugin and uses the default date-name convention; your own vault's Daily Notes settings may be different. Continue with [[07 Use cases/Meeting notes and daily notes|Meeting notes and daily notes]].

For Obsidian's own behavior, see [Properties](https://obsidian.md/help/properties) and [Daily notes](https://obsidian.md/help/plugins/daily-notes).
