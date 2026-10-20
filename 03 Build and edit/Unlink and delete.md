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
# Unlink and delete

Disconnect two ideas, or remove a note entirely. Choose the action that changes only what you intend: a relationship source or the file itself.

![[Assets/Screenshot - Connection Details Context Menu.png]]

*Open a connection's context menu to inspect its details before choosing an edit.*

Deleting a Markdown-backed node uses Obsidian's normal trash workflow. The graph node can remain as a ghost if references still point to the deleted file, including when that node is currently centered. K-Plex can automatically remove references stored in note properties, but it does **not** rewrite arbitrary Markdown-body links for you.

If body references remain, K-Plex opens **Remaining references** so you can review and remove them at the source. The first delete workflow also explains confirmation behavior; the preference lives under **Plex behavior → Navigation & interaction**.

> [!warning]
> Treat relationship editing and deletion as real vault edits. Keep backups and use test notes when learning the workflows.
