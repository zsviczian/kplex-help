---
aliases:
  - "Unlink and delete"
tags:
  - "kplex-help/caution"
  - "kplex/relationships"
  - "kplex/delete"
Friend:
  - "[[Troubleshooting checklist]]"
Previous:
  - "[[Connection details and evidence]]"
Next:
  - "[[Excalidraw integration]]"
---
# Unlink and delete

Disconnect two ideas, or remove a note entirely. Choose the action that changes only what you intend: a relationship source or the file itself.

![[Screenshot - Connection Details Context Menu.png]]

*Open a connection's context menu to inspect its details before choosing an edit.*

Deleting a Markdown-backed node uses Obsidian's normal trash workflow. The graph node can remain as a ghost if references still point to the deleted file, including when that node is currently centered. K-Plex can automatically remove references stored in note properties, but it does **not** rewrite arbitrary Markdown-body links for you.

If body references remain, K-Plex opens **Remaining references** so you can review and remove them at the source. The first delete workflow also explains confirmation behavior; the preference lives under **Canvas behavior → Navigation & interaction**.

> [!warning]
> Treat relationship editing and deletion as real vault edits. Keep backups and use test notes when learning the workflows.

## Unlink from either end

**Unlink connection** looks for the editable declaration in the note that owns it. If Note B has a property linking to Note A, centering Note A still lets you remove that property contribution from B. Inspect the source note and field before confirming; other evidence may keep the visible connection alive.

**Delete placeholder…** also works when only Markdown-body links remain. It opens **Remaining references**, explains why the placeholder is still present, and lets you open the referring notes to edit their links manually. It does not silently rewrite prose.
