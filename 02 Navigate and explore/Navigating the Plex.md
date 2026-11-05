---
aliases:
- Navigating the canvas
- Navigating the Plex
tags:
- kplex-help/how-to
- kplex/navigation
Friend:
- '[[01 Core concepts/The spatial relationship model]]'
Next:
- '[[02 Navigate and explore/Vault Search vs Find in this Plex]]'
---
# Navigating the canvas

Follow an idea without losing its context. Make a note the center, explore a connected note and use history to return.

![[Assets/Screenshot - Reading relationships.png]]

*The research example keeps a question and its surrounding context together. Open a neighbor to explore it.*

- **Single-click / tap** a node to make it the center.
- **Double-click** a file-backed node to open it in Obsidian.
- Double-click a URL to open it in the browser.
- Double-click an unresolved link to create the missing Markdown note.
- Drag empty graph space to pan; use the wheel or pinch to zoom.
- Right-click or long-press for context menus.
- Click empty graph space to clear temporary highlights.
- Use **Fit graph** to bring the visible canvas back into view.

> [!practice]
> Center [[00 Start Here/K-Plex Help|K-Plex Help]], then click this note, [[02 Navigate and explore/Vault Search vs Find in this Plex|Vault Search vs Find in this canvas]], and back. Watch how shared nodes move rather than being redrawn as unrelated points.

## Open a file in K-Plex from Obsidian

Right-click an existing file in Obsidian's file explorer, its tab or a resolved file link, then open the **K-Plex** submenu. Use long-press where the device provides that context menu.

| Destination | Desktop | Tablet | Phone |
| --- | --- | --- | --- |
| **Open** | Yes | Yes | — |
| **Open in new tab** | Yes | Yes | — |
| **Open to the right** | Yes | Yes | — |
| **Open in side panel** | Yes | Yes | Yes |
| **Open in new window** | Yes | — | — |

The chosen file becomes the center. This works for existing notes, attachments and drawings. Unresolved links in supported editor/reading context menus open their placeholder without creating a file. In Obsidian Files, folders offer **Open in K-Plex** and can also be dragged onto the canvas center. Ordinary K-Plex tabs show the centered file's basename with the K-Plex icon. A second tab or split can keep its own center while you continue in the first.

To find a node's file, use its **Open** submenu. **Open in file navigation** reveals it in Obsidian when the Files core plugin is enabled. Desktop also offers **Open in Finder** on macOS, **Open in Explorer** on Windows, or **Show in system explorer** on Linux. These reveal the file without changing the map's center.

## Use scrolling to pan with a trackpad

Enable **Settings → K-Plex → Plex behavior → Navigation & interaction → Trackpad navigation**. Ordinary scrolling then pans the canvas in both directions. Pinch, or hold Control on Windows or Command on macOS while scrolling, to zoom around the pointer.

The setting is off by default: ordinary scrolling normally zooms. Native editors and lists retain their own scrolling behavior in either mode. Touch panning and pinching remain available independently of this preference.

## Prefer the keyboard?

[[02 Navigate and explore/Keyboard navigation|Keyboard navigation]] covers graph focus, selecting nodes with arrows and switching areas; [[02 Navigate and explore/Type to select visible nodes|Type to select visible nodes]] jumps to displayed labels. The [[02 Navigate and explore/K-Plex command palette|K-Plex command palette]] makes graph actions searchable. For an uncluttered workspace, use [[05 Personalize and workspace/Fullscreen and Zen mode|Fullscreen and Zen mode]].

## Interpreting relationship counts

The small number beside a directional gate is a relationship count, not the number of line segments drawn. Gate badges count related notes, even when several sources support the same connection. Partial counts can still be marked while source data is loading.

For each connector's underlying sources, open [[03 Build and edit/Connection details and evidence|Connection details and evidence]].

## Open links using the right handler

K-Plex recognizes `obsidian://` links as searchable URL nodes. Opening one delegates to Obsidian's URI handling, so a link can open its intended note or action rather than a web preview. Review unfamiliar URI actions before opening them.

For ordinary web links, a Markdown label in frontmatter supplies a readable node title and remains available after a cached start. **Copy link** respects Obsidian's configured link format and path preferences when you paste into a note. Opening a section uses the section's own source file and heading.

## Preview before navigating

K-Plex's **Page Preview** preference applies across normal tabs, sidebars and popout windows. Use Obsidian's usual preview interaction to inspect a supported target without committing to a new center.
