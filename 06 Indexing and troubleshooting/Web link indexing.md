---
aliases:
  - "Web link indexing"
tags:
  - "kplex-help/reference"
  - "kplex/indexing"
  - "kplex/web"
Friend:
  - "[[02 Navigate and explore/Editor node and web pages]]"
  - "[[08 About/Community GitHub and contributing]]"
Previous:
  - "[[06 Indexing and troubleshooting/On demand vs Eager]]"
Next:
  - "[[06 Indexing and troubleshooting/Large vault behavior]]"
---
Web-link discovery runs **independently in the background**. Local note relationships can be usable before K-Plex has found every URL in the vault.

- **Cached URLs first:** a compatible cache can restore existing results quickly.
- **Incremental updates:** changed notes are rescanned rather than every note on every navigation.
- **Current URL gains referrers:** an open web-link node can update as more referring notes are discovered.

In **Settings → K-Plex → Indexing config**, the status may read **Preparing web link index**, **Loading cached web links — … notes loaded**, **Discovering web links — … / … notes**, or **Web link discovery incomplete**. The last state need not prevent ordinary local graph navigation.

## Try it here

Center [[08 About/Community GitHub and contributing|Community, GitHub and contributing]]. Its web addresses are ontology values, so they can appear as URL nodes. If some URLs are absent at first, check discovery progress before rebuilding the index.

Learn how links open in [[02 Navigate and explore/Editor node and web pages|Editor node and web pages]], or choose [[10 Discover by topic/09 Work with web sources|Work with web sources]]. Opening a website sends normal browser requests to that external site.

## Dense URL updates and startup resilience

Opening a high-degree website node or restoring a cache with many URLs should be more responsive: K-Plex now avoids repeated work while reconstructing shared URL references and preparing search entries. URL source updates are processed with bounded work rather than forcing all derived links onto the same immediate UI turn.

Healthy background work continues as long as progress is being made. A stalled or superseded cache restore can be retired without reviving outdated results.

[Changes: PR #95](https://github.com/zsviczian/kplex/pull/95) · [#102](https://github.com/zsviczian/kplex/pull/102) · [#104](https://github.com/zsviczian/kplex/pull/104) · [#105](https://github.com/zsviczian/kplex/pull/105).
