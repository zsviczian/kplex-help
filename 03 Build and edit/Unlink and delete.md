---
aliases:
  - "Unlink and delete"
tags:
  - "kplex-help/caution"
  - "kplex/relationships"
  - "kplex/delete"
Friend:
  - "[[06 Indexing and troubleshooting/Troubleshooting checklist]]"
Previous:
  - "[[03 Build and edit/Connection details and evidence]]"
Next:
  - "[[03 Build and edit/Excalidraw integration]]"
---
**Unlink connection** removes one unambiguous editable property source directly. When several sources contribute to the same edge, K-Plex opens **Connection details** instead of guessing which source you intended to remove.

Deleting a Markdown-backed node uses Obsidian's normal trash workflow. The graph node can remain as a ghost if references still point to the deleted file, including when that node is currently centered. K-Plex can automatically remove references stored in note properties, but it does **not** rewrite arbitrary Markdown-body links for you.

If body references remain, K-Plex opens **Remaining references** so you can review and remove them at the source. The first delete workflow also explains confirmation behavior; the preference lives under **Plex behavior → Navigation & interaction**.

> [!warning]
> Treat relationship editing and deletion as real vault edits. Keep backups and use test notes when learning the workflows.
