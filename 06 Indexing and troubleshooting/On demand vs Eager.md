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
- '[[Indexing and troubleshooting]]'
Related:
- '[[Screenshot - Background indexing effort.png]]'
- '[[Large vault behavior]]'
Previous:
- '[[How indexing works]]'
Next:
- '[[Web link indexing]]'
Friend:
- '[[Mobile and touch]]'
Watch out:
- '[[Understanding index status]]'
---
# On demand vs Eager

Want K-Plex ready sooner on your desktop, but to wait until needed on your phone? Set when preparation starts and how much it prepares separately for each device.

## Start at launch or first use

**Prepare index before opening K-Plex** allows preparation at plugin startup, including loading saved index data. Turn it off to wait until a canvas opens. A restored canvas counts as open, even in an inactive tab or sidebar. Saved history and pins alone do not start preparation; an explicit rebuild does.

| Device | Default preparation | Default strategy |
| --- | --- | --- |
| Desktop | At plugin startup | Eager |
| Tablet | At first canvas opening | On demand |
| Phone | At first canvas opening | On demand |

Missing device preferences receive these defaults on upgrade. Your saved device choices are preserved. The older single indexing-mode choice does not override the new defaults for all devices.

Deferring preparation avoids starting that pipeline in a session where you never open K-Plex. The first opening may take longer. Once admitted, closing and reopening a canvas reuses the same session rather than starting everything over.

![[Screenshot - Device indexing.png]]

*The running demo shows the default startup switches and strategies for all three device types.*

## Choose the strategy

| | **On demand** | **Eager** |
| --- | --- | --- |
| First goal | Prepare the notes needed for the requested canvas | The same useful foreground graph |
| Wider work | More relationships are prepared as you explore | Also prepares the full index in the background |
| Saved results | Reused when valid | Reused when valid |
| Relationship meaning | The same ontology and precedence | The same ontology and precedence |

Both the startup choice and strategy apply after **restarting Obsidian or reloading K-Plex**. Changing them does not stop, clear or restart the current index. These are device preferences, not K-Plex theme settings.

**Background indexing speed** is different: it applies immediately. **Responsive (recommended)** gives Obsidian more time between background tasks; **Faster** can finish work sooner at greater foreground cost.

## Choose what happens when K-Plex loses focus

In **Indexing config → When K-Plex is inactive**, set **Background effort** independently of startup and strategy. This applies when another tab or pane is active, or when you use another application—even if K-Plex remains visible beside your editor.

| Background effort | What happens |
| --- | --- |
| **0 — Paused** | Pending changes wait for K-Plex focus. |
| **1–99** | Indexing continues with reduced effort. The default is **10**. |
| **100 — Same as foreground** | Indexing uses the selected foreground speed. |

![[Screenshot - Background indexing effort.png]]

*Desktop: Background effort is set to the default 10. Moving it to 0 pauses automatic work while K-Plex is inactive.*

Changes apply immediately in both indexing strategies. K-Plex's brand mark dims when it is inactive. Select its canvas again to let it catch up. Choose **Paused** if ongoing preparation makes writing or drawing less smooth; allow more effort if you prefer indexing to progress while you work elsewhere.

Initial index preparation finishes uninterrupted. New complete-cache saves wait for K-Plex focus; a save that has already started finishes after you switch away. Pausing background indexing does not clear saved progress or change your notes.

Web links retain their own background discovery after preparation starts. Local readiness does not mean every URL is already known. See [[Web link indexing]].

While waiting for first use, diagnostics can report **Waiting for K-Plex to open**. Once open, On-demand readiness describes the selected neighborhood; Eager can show genuine full-index progress. See [[Understanding index status]].

Choose the defaults that fit when you use K-Plex. You can change them later without changing your notes.
