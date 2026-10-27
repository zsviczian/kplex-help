---
tags:
- "kplex-help/release-notes"
Guide:
- "[[11 Release notes/Release notes]]"
Explains:
- "[[06 Indexing and troubleshooting/How indexing works]]"
- "[[06 Indexing and troubleshooting/Large vault behavior]]"
- "[[06 Indexing and troubleshooting/On demand vs Eager]]"
Related:
- "https://github.com/zsviczian/kplex/releases/tag/0.2.3"
- "https://github.com/zsviczian/kplex/pull/201"
- "https://github.com/zsviczian/kplex/pull/203"
- "https://github.com/zsviczian/kplex/pull/204"
- "https://github.com/zsviczian/kplex/pull/205"
- "https://github.com/zsviczian/kplex/pull/207"
- "https://github.com/zsviczian/kplex/pull/206"
- "https://github.com/zsviczian/kplex/compare/0.2.2...0.2.3"
---
# K-Plex 0.2.3 — Less waiting, more exploring

Get to work with existing notes while K-Plex prepares their connections. This update reduces repeated indexing work and improves startup and editing responsiveness.

Published **2026-10-24**. The original GitHub release text is reproduced below.

## Original published notes

## Major indexing and performance improvements

This release brings significant improvements to indexing performance, especially for larger Obsidian vaults.

- **Faster startup:** K-Plex now avoids unnecessarily reindexing thousands of unchanged notes when Obsidian starts. In our large-vault testing, background indexing time dropped from over 30 minutes to around 7 minutes.
- **Lower CPU usage:** Reduced redundant parsing, database operations, and dependency processing make indexing considerably more efficient.
- **Faster updates:** Creating, editing, and deleting notes requires less database work, particularly when relationships remain unchanged.
- **More reliable indexing:** Improved coordination between background tasks prevents unnecessary rebuilds and helps indexing recover automatically when source data becomes available.
- **Better responsiveness:** Background work is more efficient while preserving access to navigation and editing during indexing.

Actual improvements depend on vault size, cache state, and indexing activity. Further performance optimization is ongoing.

---

## What's Changed
* Reduce startup indexing work and correct bounded source validation by @zsviczian in https://github.com/zsviczian/kplex/pull/201
* Record Mac real-vault indexing results and guarded study tooling by @zsviczian in https://github.com/zsviczian/kplex/pull/203
* Reuse authenticated dependency counts during source replacement by @zsviczian in https://github.com/zsviczian/kplex/pull/204
* Share protected metadata reads during cached-source validation by @zsviczian in https://github.com/zsviczian/kplex/pull/205
* Batch bounded dependency-count repair by @zsviczian in https://github.com/zsviczian/kplex/pull/207
* Resume startup after source recovery and avoid redundant startup work by @zsviczian in https://github.com/zsviczian/kplex/pull/206


**Full Changelog**: https://github.com/zsviczian/kplex/compare/0.2.2...0.2.3
