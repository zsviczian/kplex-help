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
# Web link indexing

Looking for a website you know you linked from a note? Web links may still be appearing while the rest of your graph is ready to use.

![[Assets/Screenshot - Index status.png]]

*The status details explain the current preparation phase. This capture shows the real update in progress while the help notes were being edited.*

- **Cached URLs first:** a compatible cache can restore existing results quickly.
- **Incremental updates:** changed notes are rescanned rather than every note on every navigation.
- **Current URL gains referrers:** an open web-link node can update as more referring notes are discovered.

In **Settings → K-Plex → Indexing config**, the status may read **Preparing web link index**, **Loading cached web links — … notes loaded**, **Discovering web links — … / … notes**, or **Web link discovery incomplete**. The last state need not prevent ordinary local graph navigation.

## Try it here

Center [[08 About/Community GitHub and contributing|Community, GitHub and contributing]]. Its web addresses are ontology values, so they can appear as URL nodes. If some URLs are absent at first, check discovery progress before rebuilding the index.

Learn how links open in [[02 Navigate and explore/Editor node and web pages|Editor node and web pages]], or choose [[10 Discover by topic/09 Work with web sources|Work with web sources]]. Opening a website sends normal browser requests to that external site.

## If a known website is still missing

Open the note that contains the link and check its address. If web-link discovery has finished but the result remains wrong, [[06 Indexing and troubleshooting/Rebuild purge and diagnostics|capture diagnostics]] before rebuilding.
