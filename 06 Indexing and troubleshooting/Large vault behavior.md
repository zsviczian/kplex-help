---
aliases:
  - "Large vault behavior"
tags:
  - "kplex-help/concept"
  - "kplex/indexing"
  - "kplex/performance"
Friend:
  - "[[06 Indexing and troubleshooting/On demand vs Eager]]"
  - "[[06 Indexing and troubleshooting/Troubleshooting checklist]]"
Previous:
  - "[[06 Indexing and troubleshooting/Web link indexing]]"
Next:
  - "[[06 Indexing and troubleshooting/Rebuild purge and diagnostics]]"
---
K-Plex is designed so a large vault does not have to become fully indexed before you can act locally.

Filename/path search and Obsidian-known relationships can appear while indexing continues. A note that belongs to a large tag or folder does not require all of its siblings to load before the note opens. A **≥** gate count means relationships prepared so far are shown, with more potentially arriving as the neighborhood loads.

When every K-Plex surface is hidden, automatic indexing pauses and pending changes are coalesced. Showing K-Plex again catches up. Background publications preserve camera and scroll position instead of repeatedly recentering the graph.

If one note exceeds the supported relationship-loading bound, K-Plex can report that its local graph counts are unavailable without implying that the entire index has failed.

## More reliable cache restoration

Recent releases reduce overhead during **large URL-cache restoration**, **search publication for many distinct URLs**, and repeated cached-source reads. They also stop abandoned or stuck startup restore operations from keeping the old cache work alive indefinitely. A **90-second inactivity policy** applies to certain restore stages; it is **not a 90-second total time limit** on a healthy, progressing vault.

These are responsiveness and recovery improvements rather than a new setting, an increase in indexed content, or a change to ontology semantics. A very large vault may still need time to acquire URL inventory and relationship evidence.

[Changes: PR #95](https://github.com/zsviczian/kplex/pull/95) · [#102](https://github.com/zsviczian/kplex/pull/102) · [#104](https://github.com/zsviczian/kplex/pull/104) · [#105](https://github.com/zsviczian/kplex/pull/105).
