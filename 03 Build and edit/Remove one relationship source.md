---
aliases:
- Remove one relationship source
- Remove one evidence source
tags:
- kplex-help/how-to
- kplex/relationships
- kplex/safety
Guide:
- "[[03 Build and edit/Build and edit]]"
Related:
- "[[03 Build and edit/Connection details and evidence]]"
- "[[03 Build and edit/Unlink and delete]]"
- "[[03 Build and edit/Date properties and daily notes]]"
Watch out:
- "[[01 Core concepts/Relationship sources and inference]]"
---
One visible connector may have several independent sources. For example, a note's **Parent** property and a separate body link can both refer to the same target. Removing the *connector* and removing *one source that supports it* are different operations.

## Remove a single frontmatter source

1. Open the context menu on an existing connection and choose **Connection details…**.
2. Inspect the evidence list and identify the **frontmatter property** that should no longer define the relationship.
3. Use that source's remove action and **confirm** the change.
4. Reopen Connection details and review the remaining evidence. The connection may remain visible when another source still supports it.

K-Plex rechecks the selected file and property occurrence before writing, rather than blindly removing something that has changed. This feature is deliberately **scoped to eligible direct frontmatter relationship sources**, not a generic way to delete any inferred or body relationship.

> [!warning] Confirm the source, not just the line
> If several fields or files support the same visual relationship, removing one entry should not silently delete the others. When in doubt, inspect the underlying Markdown frontmatter in Obsidian first. Keep a current vault backup before testing graph edits on important data.

Native scalar **Date properties** are not editable wiki-link lists; change the date value in the source note instead. See [[03 Build and edit/Date properties and daily notes|Date properties and daily notes]].

**Also see:** [[03 Build and edit/Connection details and evidence|Connection details and evidence]] and [[03 Build and edit/Unlink and delete|Unlink and delete]].

[Source: merged PR #108](https://github.com/zsviczian/kplex/pull/108).
