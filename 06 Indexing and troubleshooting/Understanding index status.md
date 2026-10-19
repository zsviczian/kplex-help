---
tags:
- kplex-help/reference
- kplex/indexing
- kplex/troubleshooting
Guide:
- '[[06 Indexing and troubleshooting/Indexing and troubleshooting]]'
Related:
- '[[06 Indexing and troubleshooting/How indexing works]]'
- '[[06 Indexing and troubleshooting/On demand vs Eager]]'
- '[[06 Indexing and troubleshooting/Web link indexing]]'
- '[[06 Indexing and troubleshooting/Troubleshooting checklist]]'
---
The index indicator is a **status explanation**, not an instruction to wait before using K-Plex.

## Three separate things to check

| Question | What the indicator helps you understand |
| --- | --- |
| Is my current Plex usable? | Preparing local graph versus Local graph ready, or a local-count limitation. This is about the selected neighborhood. |
| Is full indexing running? | In Eager mode, wider work can show a genuine ratio of processed Markdown files. |
| Are all web links known? | URL inventory has its own preparation, cache restoration and discovery status. A usable local graph does not imply complete URL results. |

Hover or focus the indicator for details. Click/tap to pin its information bubble; click again, click outside or press Escape to dismiss it.

## Why the count depends on mode

On demand prepares the requested graph rather than every note in the vault. A small locally published set is not a meaningful “x of y vault files indexed” ratio. Eager can show real full-index progress. Hidden/revealed views also update their local readiness display.

Background work may continue after local readiness. Counts marked **≥** are lower bounds while sources are being prepared, not final totals. URL discovery and validation can take longer in a large vault.

## Next release: keep working while the wider index catches up

Merged changes improve reuse of cached knowledge, prioritize the requested or restored center and preserve navigation history while startup data arrives. New notes and drawings can become searchable before the entire background pass finishes. The initial stationary center and later ontology updates can refresh without requiring a trip to another node and back.

Ordinary prose autosaves retain an equivalent graph layout instead of appearing to change relationship roles temporarily. Genuine relationship changes still update the Plex. These improvements do not promise instant full-vault indexing, eliminate every intermittent startup issue or establish a universal performance gain.

## Next release: saved is not the same as refreshed

Ontology settings are edited as a local draft and committed after a pause or leaving the field, rather than triggering the former work on every keystroke. A settings or relationship save can complete while the graph update is still pending.

Read the actual completion message. Use an offered refresh/recovery action instead of repeating a creation or assuming the note was not saved. If a settings change is received from another device, it can update the live appearance; an indexing-strategy change still needs a restart. See [[05 Personalize and workspace/Colors and themes]].

## If something looks stuck

Check local readiness, the actual indexing mode and URL inventory separately. Try a specific Vault Search query to locate a missing note. If the visible result contradicts the status, capture diagnostics before restarting or purging; see [[06 Indexing and troubleshooting/Rebuild purge and diagnostics]] and [[06 Indexing and troubleshooting/Troubleshooting checklist]].

Do not purge just because background URL discovery is unfinished. If the application stops responding during a settings change, include the setting, open panes and sequence of edits in the issue; a startup-readiness message cannot explain every kind of freeze.

Sources for merged improvements: [ontology settings #147](https://github.com/zsviczian/kplex/pull/147), [save completion #179](https://github.com/zsviczian/kplex/pull/179), [autosave continuity #180](https://github.com/zsviczian/kplex/pull/180), [startup #183](https://github.com/zsviczian/kplex/pull/183), [restoration #185](https://github.com/zsviczian/kplex/pull/185), [stationary refresh #186](https://github.com/zsviczian/kplex/pull/186). See [[00 Start Here/Recently added features]] for the source baseline.
