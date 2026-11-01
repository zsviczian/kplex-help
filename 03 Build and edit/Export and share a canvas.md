---
aliases:
- Export PNG
- Export MindMap Markdown
- Copy a map outline
tags:
- kplex-help/how-to
- kplex/export
Guide:
- '[[03 Build and edit/Build and edit]]'
Friend:
- '[[02 Navigate and explore/Mind Map]]'
- '[[02 Navigate and explore/Footprints and breadcrumbs]]'
- '[[12 Automation/Automation and scripting]]'
- '[[07 Use cases/Bring a connected outline into your writing]]'
---
# Export and share a canvas

Turn the map you have built into something you can use elsewhere: a PNG for a presentation, a linked Markdown outline for writing, or a record of the route you explored.

## Choose the result you need

Right-click empty canvas space, or long-press it on touch, and open **Export**. The menu works in Compass, Mind Map and Facets.

| Choose | You receive |
| --- | --- |
| **Canvas to image** | A preview you can copy or save as PNG |
| **Canvas to MindMap Markdown** | A linked outline you can copy or save as Markdown |
| **Breadcrumbs to Markdown** | The current canvas's Footprints copied as Markdown, newest first, with repeated visits |

Image export also has a toolbar button. Image and Markdown export are available through the Command Palette. Export captures your current map; it does not expand branches or change notes.

## Share a picture

1. Center [[09 Showcase examples/Example - Workshop plan|the workshop plan]] and arrange the map as you want to share it.
2. Choose **Export → Canvas to image**.
3. Select **Whole canvas** to include content beyond the camera view, or **Current viewport** for your current framing.
4. Choose **Image scale** (1×, 2× or 3×) and, if useful, **Transparent background**. Check the preview and any warnings.
5. Select **Copy PNG** or **Save PNG**. Finish choosing the destination in the system save or share dialog.

Whole canvas keeps the current clipping and scroll position inside each relationship area. Rows hidden inside those areas are not unrolled. Unfold or scroll to the material you need before opening export. Transparent output removes the canvas background and Compass tint while keeping nodes, connectors and Facets region styling.

Very large images may use a lower resolution. Some embedded websites, media, unavailable images or fonts cannot be captured; the dialog reports these limitations. Copy and Save availability depends on your device. Successful Copy closes the dialog; a system save/share handoff still needs you to finish the destination choice.

## Take a linked outline into your writing

1. Build the workshop outline in Mind Map, unfolding the branches you want to include. Compass and Facets can also become outlines with cross-links.
2. Select a branch if you want only that part, then choose **Export → Canvas to MindMap Markdown**.
3. Choose **Whole map** or **Selected branch**, when available.
4. Set **Ontology labels** to **Do not include**, **Visible ontology only** (the default), or **All ontology, including hidden**.
5. Review the exact Markdown preview and warnings, then **Copy Markdown** or **Save Markdown**.

The outline keeps the constructed map's order, note links, repeated occurrences and supported cross-links. Offscreen constructed rows remain eligible, including rows outside the camera or a scrolling area's visible portion. Current filters and folds still limit the content. This is an outline of the map, not a copy of every note's text or a whole-vault export.

Additional active ontology labels become cross-links without duplicating a branch. Including hidden labels does not bring back filtered nodes or expand folds. Some structural nodes, unusual link targets or syntax-sensitive labels need conversion or omission; review the warnings before relying on an exact round trip.

Paste the result into a Markdown note, or use Excalidraw's **MindMap Builder** to make a drawing from it. Exporting does not alter the source relationships, and editing the exported outline does not automatically edit them back in K-Plex.

## Keep a record of your exploration

Choose **Export → Breadcrumbs to Markdown** after exploring. It copies this canvas's visit trail, including returns to the same note, rather than a deduplicated reading list. See [[02 Navigate and explore/Footprints and breadcrumbs|Footprints and breadcrumbs]].
