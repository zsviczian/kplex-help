---
aliases:
- Colors and appearance
- Reset colors without losing semantic styles
tags:
- kplex-help/how-to
- kplex/styling
Parent:
- '[[05 Personalize and workspace/Personalize and workspace]]'
Friend:
- '[[05 Personalize and workspace/Node styles from help tags]]'
- '[[05 Personalize and workspace/Visibility and connector styling]]'
- '[[04 Filter and focus/Graph Lenses]]'
---
# Colors and themes

Want the map to fit your Obsidian theme while keeping colors that mean something to you? Choose a named appearance, adjust it and reset only the colors you intend to change.

## Follow Obsidian or keep your own appearance

A fresh installation uses Obsidian's live theme colors. The one-time upgrade saves your previous appearance as **User theme** and selects **Default base + my semantic colors**: native Obsidian base colors with your semantic styles and non-color choices preserved. A notification points you to Visual styling. **Default theme** remains available too.

Fresh installs do not receive an upgrade notification. Later restarts and plugin updates keep your selected theme; the migration is not a recurring color reset. A first-run ExcaliBrain import also receives its preserved User-theme copy.

Open **Settings → K-Plex → Visual styling**. Select a theme from **Theme** to apply it. **Manage themes** uses a searchable manager like the node/link style managers; opening a row does not activate it. Create an independent copy of the current theme or start from defaults.

Default theme cannot be renamed, deleted or reset. Its first genuine saved appearance change creates **Custom theme**. Opening or cancelling an editor does not create a theme.

Named themes store base and semantic appearance. Ontology, navigation, indexing strategy and lens rules remain shared; switching a theme does not create a separate knowledge structure or restore a deleted lens.

![[Assets/Screenshot - Named themes.png]]

*Visual styling in this vault: native base colors with the existing semantic colors retained.*

## Reset the right colors

Use **Reset colors** beside the theme selector and review its Light/Dark preview before confirming.

| Scope | What changes |
| --- | --- |
| Base colors only | Restore native canvas and standard node/link colors while keeping custom semantic styling. This is the default reset scope. |
| Semantic colors only | Clear color overrides in custom rules, semantic assignments, directional tint and lens colors; retain base assignments. |
| All colors | Apply both color resets. |

Resets preserve rule names, matching keys, tag order, icons, fonts, sizes, shapes and other non-color fields. Named palette entries and other saved themes remain. Custom rules can still override standard colors after a base-only reset.

For this help vault, **Default base + my semantic colors** is a useful starting point when adopting native colors while retaining the meaning of its custom help styles.

## Choose what a color follows

**Default** inherits the applicable style or native color. **Fixed color** uses one literal color. **Named color** refers to a saved Light/Dark pair. **Theme color** follows an Obsidian or custom CSS variable, such as `--interactive-accent`.

Zero opacity means transparent, not Default. A variable or named-color choice remains a reference; it is not saved as a sampled RGB value. In a nested picker, **Use color** updates the draft; select **Save** in the containing editor to keep it.

Under **Colors → Named colors**, create and manage Light/Dark pairs. Renaming keeps references. Deleting a used color asks for a replacement. Suggested opposite-mode colors are a starting point, not a guarantee of readable contrast.

## Add a subtle directional cue

![[Assets/Screenshot - Directional tint.png]]

*The directional-tint editor compares Light and Dark colors and keeps Save and Cancel visible.*

**Colors → Directional background tint** adds four Compass sectors behind the graph. It is off by default. Choose colors and an intensity, then Save. The sectors are orientation cues, not exact membership boundaries or drop targets; they do not change relationships.

Custom node and link editors also provide paired previews and sliders with inheritance reset. Note Type tag links have a separate style and inherit twice the ordinary tag-link width by default.

## Settings arriving from another device

Valid external settings received by Obsidian are applied to the running plugin without replaying another device's navigation or saving the same settings straight back. A conflicting open editor may ask you to reopen and reapply its draft. Unrelated local edits preserve accepted incoming changes.

This does not replace Obsidian Sync or guarantee conflict-free simultaneous offline edits. Indexing-strategy changes still require a restart. Keep a settings backup before upgrading or downgrading; older releases cannot interpret all newer theme references.
