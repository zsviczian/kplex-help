---
tags:
- "kplex-help/how-to"
- "kplex/canvas"
Guide:
- "[[04 Filter and focus/Facets]]"
Friend:
- "[[04 Filter and focus/Facets layouts and classification]]"
- "[[04 Filter and focus/Share presets and lenses]]"
Related:
- "[[09 Showcase examples/Example - Workshop board]]"
---
# Define a Facets workflow

Turn a distinction you already make into a reusable view. Begin with a small set of connected notes and categories that help you decide what to do.

## Make a preset

1. Open **Settings → K-Plex → Canvas behavior → Views → Facets → Manage presets**, or use the selected preset's settings control on the canvas.
2. Create a preset, or **Duplicate** a nearby example and give it a name that describes its purpose.
3. Keep three to seven categories. Name them, set their order and colors, and choose the **Classification source**.
4. Enter matching values for a property, tags or note types. For **Category rule**, use the condition editor to define what makes each category match.
5. Choose a layout and **Save**. Select the preset on a Facets canvas centered on your example note.

For a property such as `Workshop stage`, the help example recognizes `Collect`, `Shape` and `Share`. Matching trims spaces and preserves case. For a Tags source, enter values in their displayed form, including the leading `#`, such as `#kplex/navigation`. Normal YAML tags may omit that prefix. Several recognized aliases can lead to one category; the visible category label can change without rewriting note values.

## Separate looking from changing notes

Changing a preset, its colors or its layout changes the view. It does not rewrite note properties.

For a **Property** source, an explicit **Assignment value** can make a category a destination for a property assignment. Drop a supported note into that category, or use the available assignment action, then review and confirm the property preview. This writes the selected property, rather than changing the note's ontology relationship to the center. Leave Assignment value empty for a read-only category.

Tags, note types and category rules classify notes here; they are not writable category-drop targets. Edit their data in the normal note or use the dedicated tag and note-type actions. A workflow arrow between areas is a visual guide, not a relationship between every pair of notes.

## Keep the preset useful

Write short help explaining the question, expected note data and any limits. The help can travel with the preset. **Cancel** keeps the installed version; **Save** applies the edited preset to canvases using it. Selecting a preset is local to a canvas, while editing its definition is shared.

Delete unused presets through **Manage presets**. Choose a replacement so existing and closed canvases have a useful destination; deleting the preset leaves notes unchanged.

Try [[09 Showcase examples/Example - Workshop board|the workshop board]] before adapting the pattern to your own project.
