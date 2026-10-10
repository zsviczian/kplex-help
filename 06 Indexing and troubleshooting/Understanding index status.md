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
| Is my **current Plex** usable? | **Preparing local graph** versus **Local graph ready**, or a specific local-count limitation. This is about the selected neighborhood. |
| Is **full indexing** running? | In **Eager** mode, indexing/updating progress may show **x of y Markdown files** processed while wider work proceeds. |
| Are all **web links** known? | The URL inventory has its own background preparation, cache restoration and discovery status. A usable local graph does not guarantee complete URL results. |

Hover or focus the status indicator for details. You can click/tap to pin its information bubble, then click again, click outside or press Escape to dismiss it.

## Why the count depends on mode

In **On demand** mode, K-Plex prepares the requested graph rather than every note in the vault. A small count of locally published notes is **not** meaningful as “x of y vault files indexed”; the newer status display deliberately avoids that misleading ratio. In **Eager** mode a genuine full-index progress ratio can be shown. The indicator also catches up after a hidden/revealed view so it does not continue claiming “Preparing local graph” once the selected graph is actually ready.

Background work may continue after local readiness. Counts marked **≥** are lower bounds while sources are still being prepared, not the exact final count. When a URL points to many source notes, URL updates are scheduled cooperatively to help keep interactions responsive.

## If something looks stuck

1. Check whether **Local graph ready** is reported, regardless of background work.
2. Check the current **Indexing mode** and **Web link** inventory separately in K-Plex settings.
3. Try a specific Search Vault query or navigate to the missing note, which can request targeted work.
4. If status contradicts the visible graph or remains stale after switching away/back, collect diagnostics and see [[06 Indexing and troubleshooting/Troubleshooting checklist|Troubleshooting checklist]].

Do not purge the cache just because a URL inventory is still filling. [[06 Indexing and troubleshooting/Rebuild purge and diagnostics|Rebuild, purge and diagnostics]] describes when more disruptive steps make sense.
