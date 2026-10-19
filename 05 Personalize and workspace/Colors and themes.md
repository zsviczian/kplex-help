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
**Next release:** These appearance controls are merged into K-Plex main but are not included in released 0.1.3. See [[00 Start Here/Recently added features]] for the review baseline.

## Follow Obsidian or keep your own appearance

A fresh installation uses Obsidian's live theme colors. Upgrading preserves the existing appearance as the selected **User theme** rather than silently replacing custom colors. It also provides **Default base + my semantic colors** and **Default theme**.

Open **Settings → K-Plex → Visual styling**. Select a theme from **Theme** to apply it. **Manage themes** uses a searchable manager like the node/link style managers; opening a row does not activate it. Create an independent copy of the current theme or start from defaults.

Default theme cannot be renamed, deleted or reset. Its first genuine saved appearance change creates **Custom theme**. Opening or cancelling an editor does not create a theme.

Named themes store base and semantic appearance. Ontology, navigation, indexing strategy and lens rules remain shared; switching a theme does not create a separate knowledge structure or restore a deleted lens.

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

**Colors → Directional background tint** adds four Compass sectors behind the graph. It is off by default. Choose colors and an intensity, then Save. The sectors are orientation cues, not exact membership boundaries or drop targets; they do not change relationships.

Custom node and link editors also provide paired previews and sliders with inheritance reset. Note Type tag links have a separate style and inherit twice the ordinary tag-link width by default.

## Settings arriving from another device

**Next release:** Valid external settings received by Obsidian are applied to the running plugin without replaying another device's navigation or saving the same settings straight back. A conflicting open editor may ask you to reopen and reapply its draft. Unrelated local edits preserve accepted incoming changes.

This does not replace Obsidian Sync or guarantee conflict-free simultaneous offline edits. Indexing-strategy changes still require a restart. Keep a settings backup before upgrading or downgrading; older releases cannot interpret all newer theme references.

Sources: [appearance guide at the reviewed commit](https://github.com/zsviczian/kplex/blob/10760685552fdbafe089a58fc8d80d318853ff31/docs/APPEARANCE.md), [themes #158](https://github.com/zsviczian/kplex/pull/158), [live settings #182](https://github.com/zsviczian/kplex/pull/182).
