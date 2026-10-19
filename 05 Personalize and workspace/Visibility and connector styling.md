---
aliases:
- Visibility and connector styling
tags:
- kplex-help/reference
- kplex/styling
- kplex/nodes
Friend:
- '[[01 Core concepts/Node types]]'
- '[[04 Filter and focus/Graph Lenses]]'
- '[[05 Personalize and workspace/Colors and themes]]'
Previous:
- '[[05 Personalize and workspace/Note-tab synchronization]]'
---
K-Plex can show or hide categories such as attachments, folders, tags, URLs, unresolved/virtual nodes, inferred relationships and page nodes. Visibility controls determine how much structural context you see at once.

Connector appearance includes color, width, solid/dashed/dotted style, arrowheads, labels and text appearance. Ontology-specific styles can override the base connector. For a temporary perspective rather than persistent styling, use [[04 Filter and focus/Graph Lenses]].

This help configuration gives Challenger/Watch-out connections a stronger visual treatment and uses separate colors for hierarchical, lateral and sequential ontology fields.

## Next release: inspect connections without keeping all cross-links visible

Hold **Alt** on Windows or **Option** on macOS while hovering over a node, gate or connector to highlight its related connections. With **Show cross-links** off, modifier-hover can also temporarily reveal eligible cross-links between displayed nodes:

- Hover a **node** to reveal eligible cross-links touching that node.
- Hover a **gate** to reveal only eligible cross-links attached to that exact gate.

Release the key or leave the target to clear the preview. Losing window focus or navigating also clears it. With cross-links already enabled, matching edges highlight without adding duplicates.

This does not reveal filtered-out nodes, bypass clipping or search for every connection across the vault. It does not change the saved relationship data or turn the normal Cross-links toggle on.

## Next release: separate modifier preferences

Under **Settings → K-Plex → Plex behavior → Navigation & interaction**, hover highlighting and area outlines have separate modifier requirements. They require Alt/Option by default when no existing choice is saved. Turn off the hover requirement for the short delayed hover behavior instead; Alt/Option can still request the temporary cross-link preview.

Gate tooltips also require the modifier by default. Explicit **Area settings** remains available for editing relationship areas without relying on hover outlines. Existing saved preferences are preserved.

## This help vault's display choices

The supplied configuration uses **Siblings off**, **cross-link opacity 50%**, and **100-character regular node labels**. Its saved node, relationship and Graph Lens stroke widths were reduced by one point, with a 0.5-point minimum.

To hide cross-links, open **Filters and lenses** in the active Plex and turn off **Show cross-links**. In the reviewed baseline this toggle starts on in each view and is not persisted in `data.json`. A distributed settings file therefore cannot pre-disable it. Opacity affects how visible those lines are when shown, not whether they are enabled.

Use [[04 Filter and focus/Quick Filter]] to simplify the neighborhood further, or [[05 Personalize and workspace/Colors and themes]] to adapt the appearance without removing relationships.

Sources for next-release interaction: [#170](https://github.com/zsviczian/kplex/pull/170), [#171](https://github.com/zsviczian/kplex/pull/171), [#177](https://github.com/zsviczian/kplex/pull/177), [cross-link preview #181](https://github.com/zsviczian/kplex/pull/181). [Reviewed graph implementation](https://github.com/zsviczian/kplex/blob/10760685552fdbafe089a58fc8d80d318853ff31/src/ui/PlexGraph.tsx).
