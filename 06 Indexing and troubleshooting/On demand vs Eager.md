---
aliases:
- On demand vs Eager
- Device-specific indexing
- Prepare the index before opening K-Plex
tags:
- kplex-help/reference
- kplex/indexing
- kplex/performance
Guide:
- '[[06 Indexing and troubleshooting/Indexing and troubleshooting]]'
Related:
- '[[06 Indexing and troubleshooting/Large vault behavior]]'
Previous:
- '[[06 Indexing and troubleshooting/How indexing works]]'
Next:
- '[[06 Indexing and troubleshooting/Web link indexing]]'
---
# Choose when K-Plex prepares its index

There are two choices: **when preparation starts** and **how much it prepares**. Open **Settings → K-Plex → Indexing config** to set each independently for Desktop, Tablet and Phone.

## Start at launch or first use

**Prepare index before opening K-Plex** allows preparation at plugin startup, including loading saved index data. Turn it off to wait until a Plex opens. A restored Plex counts as open, even in an inactive tab or sidebar. Saved history and pins alone do not start preparation; an explicit rebuild does.

| Device | Default preparation | Default strategy |
| --- | --- | --- |
| Desktop | At plugin startup | Eager |
| Tablet | At first Plex opening | On demand |
| Phone | At first Plex opening | On demand |

Missing device preferences receive these defaults on upgrade. Your saved device choices are preserved. The older single indexing-mode choice does not override the new defaults for all devices.

Deferring preparation avoids starting that pipeline in a session where you never open K-Plex. The first opening may take longer. Once admitted, closing and reopening a Plex reuses the same session rather than starting everything over.

![[Assets/Screenshot - Device indexing.png]]

*The running demo shows the default startup switches and strategies for all three device types.*

## Choose the strategy

| | **On demand** | **Eager** |
| --- | --- | --- |
| First goal | Prepare the notes needed for the requested Plex | The same useful foreground graph |
| Wider work | Additional semantic work follows demand | Also prepares the full index in the background |
| Saved results | Reused when valid | Reused when valid |
| Relationship meaning | The same ontology and precedence | The same ontology and precedence |

Both the startup choice and strategy apply after **restarting Obsidian or reloading K-Plex**. Changing them does not stop, clear or restart the current index. These are device preferences, not K-Plex theme settings.

**Background indexing speed** is different: it applies immediately. **Responsive (recommended)** gives Obsidian more time between background tasks; **Faster** can finish work sooner at greater foreground cost.

Web links retain their own background discovery after preparation starts. Local readiness does not mean every URL is already known. See [[06 Indexing and troubleshooting/Web link indexing]].

While waiting for first use, diagnostics can report **Waiting for K-Plex to open**. Once open, On-demand readiness describes the selected neighborhood; Eager can show genuine full-index progress. See [[06 Indexing and troubleshooting/Understanding index status]].

The defaults postpone work; they do not guarantee a smaller fully built graph, instant first opening or a measured CPU/memory improvement.
