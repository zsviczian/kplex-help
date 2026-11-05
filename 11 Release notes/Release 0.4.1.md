---
aliases:
- K-Plex 0.4.1 release notes
tags:
- kplex-help/release-notes
Note type: ReleaseNotes
Guide:
- '[[11 Release notes/Releases 0.4]]'
Previous:
- '[[11 Release notes/Release 0.4.0]]'
Next:
- '[[11 Release notes/Release 0.4.2]]'
Explains:
- '[[06 Indexing and troubleshooting/How indexing works]]'
- '[[03 Build and edit/Unlink and delete]]'
- '[[06 Indexing and troubleshooting/Understanding index status]]'
Related:
- https://github.com/zsviczian/kplex/releases/tag/0.4.1
---
# K-Plex 0.4.1 — Keep exploring as notes change

Move between notes with less repeated preparation. This update improves Eager indexing and makes it easier to remove unwanted references from either end of a connection.

Published November 2, 2026. This is a reader-facing summary of the [published release](https://github.com/zsviczian/kplex/releases/tag/0.4.1).

## Keep the graph current while you work

Once an Eager index is ready, ordinary note changes update the affected relationships without requiring each next center to prepare the whole graph again. Navigation and edits on the canvas take priority over unrelated background work. Saved index data is reused on later starts, with clearer progress while preparation continues.

See [[06 Indexing and troubleshooting/How indexing works|How indexing works]] and [[06 Indexing and troubleshooting/Understanding index status|Understanding index status]].

## Remove references from either endpoint

**Unlink connection** can offer the editable property in the note that actually owns it, even when the other note is centered. When a placeholder is still referenced in Markdown text, **Delete placeholder…** opens an explanation and offers the source notes for manual editing instead of silently doing nothing.

See [[03 Build and edit/Unlink and delete|Unlink and delete]].
