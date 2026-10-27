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
# Understanding index status

Know whether to keep working or wait for more context. Read the status for the current graph separately from wider indexing and web-link discovery.

![[Assets/Screenshot - Index status.png]]

*The status details explain the current preparation phase. This capture shows the real update in progress while the help notes were being edited.*

## Read the status for your task

The indicator near **K-Plex** explains what is happening. Open its details when you need more context.

| Status or cue | What it means for you |
| --- | --- |
| **Waiting for K-Plex to open** | Preparation is deferred until a canvas is opened. |
| **Preparing local graph** | The selected note's neighborhood is still being prepared. |
| **Local graph ready** | You can work with this neighborhood even if wider discovery continues. |
| **≥** beside a gate count | This is a lower bound; more related notes may arrive. |
| **Local graph counts unavailable** | A complete local count is not available; it does not mean every part of K-Plex has failed. |
| Web-link discovery still running | Some website results may appear later. |

An **Eager** index can show whole-vault progress. **On demand** describes the requested neighborhood instead; it is not a promise that every note in the vault is already prepared. Choose the behavior for your devices in [[06 Indexing and troubleshooting/On demand vs Eager]].

## Keep working while context arrives

Try navigating to the particular note you need. Filename and path search can work while richer relationships are still loading. A new file can be saved and discoverable before every connection has refreshed.

Read completion messages carefully. If an edit is saved but its graph refresh is pending, use the offered recovery action rather than creating a duplicate note or repeatedly saving the same change.

## If the visible result stays wrong

Clear filters and inspect the affected connection's [[03 Build and edit/Connection details and evidence|details]]. If needed, [[06 Indexing and troubleshooting/Rebuild purge and diagnostics|capture diagnostics]] before restarting, rebuilding or purging. Mention what you were trying to do and which status you saw.

An unfinished website inventory alone is not a reason to purge the cache. Use the [[06 Indexing and troubleshooting/Troubleshooting checklist|troubleshooting checklist]] to choose a smaller first step.
