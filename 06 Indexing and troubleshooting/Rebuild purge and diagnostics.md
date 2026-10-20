---
aliases:
- Rebuild purge and diagnostics
tags:
- kplex-help/how-to
- kplex/indexing
- kplex/troubleshooting
Friend:
- '[[08 About/Community GitHub and contributing]]'
Previous:
- '[[06 Indexing and troubleshooting/Large vault behavior]]'
Next:
- '[[06 Indexing and troubleshooting/Troubleshooting checklist]]'
---
# Rebuild purge and diagnostics

Is the graph still wrong after checking the affected note? Capture diagnostics first, then choose a recovery step that leaves your notes intact.

![[Assets/Screenshot - Report a problem.png]]

*Report a bug copies diagnostics and opens this review dialog. Nothing is submitted automatically.*

## Capture the problem before resetting anything

**Report a bug** copies a diagnostic report and opens a dialog where you can review it. It is also available from the graph's background context menu in K-Plex. A report complements your description; it does not capture everything that happened on screen or replace a short recording of an intermittent issue.

## more useful passive activity information

Both report routes include a short activity summary from this K-Plex session, plus current work/readiness information. No debug-console setup is needed. Copying the report does not upload it, reset the capture or start a new indexing job.

The activity summary contains fixed categories, counts, durations and public build/mode metadata—not note content, paths, queries or property values. Other support-report sections can disclose environment, theme or plugin metadata, so review the complete text before publishing it.

Reloading K-Plex or restarting the app clears the session activity summary. Capture the report before another restart whenever possible, and mention earlier restarts or build changes in your issue.

Elapsed times can include waits and overlapping work. They are not CPU measurements or proof that the application was continuously idle. A saved note with a pending graph refresh is also different from a failed note save.

## Use maintenance tools in increasing order of disruption

After recording the problem, refresh the current view if graph data looks stale. Use **Rebuild index** when K-Plex needs to re-evaluate derived graph data. Reserve **Indexing config → Purge index cache** for a cache problem that warrants deleting the persistent IndexedDB cache; your notes are unchanged, but restart Obsidian before continuing with K-Plex.

The cache-size display is an approximate logical payload estimate, not necessarily the physical disk allocation. An incomplete URL inventory alone is not a reason to purge. See [[06 Indexing and troubleshooting/Understanding index status]].
