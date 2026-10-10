---
aliases:
- On demand vs Eager
tags:
- kplex-help/reference
- kplex/indexing
- kplex/performance
Friend:
- '[[06 Indexing and troubleshooting/Large vault behavior]]'
Previous:
- '[[06 Indexing and troubleshooting/How indexing works]]'
Next:
- '[[06 Indexing and troubleshooting/Web link indexing]]'
---
In **Settings → K-Plex → Indexing config → Indexing mode**, choose when K-Plex prepares semantic source data.

| | **On demand** | **Eager** |
| --- | --- | --- |
| **First goal** | Prepare notes needed for the Plex you request | Same foreground behavior |
| **Background scope** | Additional semantic work is driven by need | Also prepares the full index in the background |
| **Cache** | Reuses persisted results for subsequent navigation | Reuses persisted results too |
| **Relationships** | Same ontology and precedence | Same ontology and precedence |

Neither policy makes every web URL appear immediately. **Web link indexing is an independent background process** in both modes.

Changing Indexing mode requires an **Obsidian restart**. The **Background indexing speed** setting instead controls how much time Obsidian gets between background tasks; it applies immediately. **Responsive (recommended)** favors UI responsiveness, while **Faster** may finish indexing sooner at greater foreground cost.

The supplied help vault uses **On demand**. Use [[06 Indexing and troubleshooting/Large vault behavior|Large vault behavior]] to understand partial gate counts and [[06 Indexing and troubleshooting/Web link indexing|Web link indexing]] for URL progress.

**Status terminology:** On-demand readiness is about your selected neighborhood, not a count of how many of the vault's files have been fully indexed. Eager progress can display a true full-vault ratio. See [[06 Indexing and troubleshooting/Understanding index status|Understanding index status]].
