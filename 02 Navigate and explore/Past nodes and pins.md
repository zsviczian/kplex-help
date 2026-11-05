---
aliases:
- Past nodes and pins
tags:
- kplex-help/how-to
- kplex/navigation
Friend:
- '[[K-Plex Help]]'
- '[[Footprints and breadcrumbs]]'
Previous:
- '[[Vault Search vs Find in this Plex]]'
Next:
- '[[Editor node and web pages]]'
---
# Past nodes and pins

Return to where you were, or keep a project within easy reach. Past nodes remembers recent navigation; pins keep the landmarks you choose.

![[Screenshot - Pins.png]]

*Pins keep chosen landmarks above the graph.*

![[Screenshot - Past nodes.png]]

*Past nodes keeps recent destinations below the graph, with icons for the target type.*

Pins are useful for anchors such as a project home, a research question, a dashboard note, or this help home. History is useful for retracing exploration.

Past nodes and pins use your node styles, including note-type and tag colors, borders, icons and prefixes. They keep compact list sizes; the current destination has a separate accent outline.

To scroll Past nodes with a mouse, hold the primary button and drag left or right. A short click still opens the chosen note. Touch swiping, trackpad scrolling and keyboard activation remain available.

In Mind Map, selecting a history entry or pin starts the map at that note as its new root. The full History and pins pickers do the same, within the canvas that opened them.

You can also create relationships from these surfaces. Drag a relationship gate onto a history entry or pinned note to connect using that gate's relationship type. Dragging a node body onto a history entry or pin lets you choose the relationship type.

This help vault starts with a few useful pins, including [[K-Plex Help|K-Plex Help]] and [[Relationship roles|Relationship roles]].

**Keyboard routes:** **Backspace** goes back and **Shift+Backspace** goes forward when no type-to-select phrase is active. **Alt/Option+B** opens pins, **Alt/Option+H** opens the full history picker, and **Alt/Option+P** toggles the current selection/center pin. These defaults can be changed in [[Actions and shortcuts|Actions and shortcuts]].

## Want every visit in just this canvas?

[[Footprints and breadcrumbs|Footprints (session breadcrumbs)]] records the complete visit sequence of **one canvas**, newest first, including repeated visits. Use the footprints icon next to Find in canvas, rather than the shared Past nodes bar at the bottom. Footprints is **not persisted**: it survives moving that canvas between windows, but clears when the canvas closes or Obsidian restarts.

Selecting an earlier Footprints visit appends another visit. **Start here** resets only that canvas's trail, while **Copy as Markdown** exports the whole list for pasting into a note. Neither action clears Past nodes or pins. For a practical exercise, try [[Rediscover and remember your notes]].

## Put pins in your preferred order

Drag a pin by its reorder handle and follow the insertion marker, then release to save its position. Its context menu also offers **Move left** and **Move right**. Reordering is shared across your canvases; it does not change History. Cancelling the drag leaves the order unchanged.

## Pin today, this week or this month

1. Open **Settings → K-Plex → Canvas behavior → Pins**.
2. Enable **Show this pin** for **Today**, **This week** or **This month**.
3. For Today, leave **Use Daily Notes settings** on to use Obsidian's configured folder, date format and template. Turn it off to supply a custom Folder and Date format; these fields appear only while using custom settings.
4. Configure the weekly and monthly folders/formats to match your notes. Check **Current destination** before leaving settings.

The destinations follow this device's local date and update as the day, week or month changes. They point to notes, not to a fixed date saved when you enabled the pin. Weekly dates use the chosen start of the week. Use `GGGG-[W]WW` for an ISO week-year/week, or the matching locale format `gggg-[W]ww`; week-years can differ from calendar years near New Year.

If the destination does not exist, activating the pin asks **Create periodic note?**. Review the path and **After saving** destination, then create it or cancel. The opening choice is remembered separately from ordinary creation and linking. Notes are never created merely because the date changes.

Today with Daily Notes settings enabled uses core Daily Notes creation and its configured template. Custom daily, weekly and monthly pins use their configured paths; they do not automatically inherit a separate periodic-notes plugin's template settings. Applicable Templater creation automation still runs. See [[Date properties and daily notes|Date properties and daily notes]] for relationships based on dates in other notes.
