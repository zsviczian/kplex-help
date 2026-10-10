---
aliases:
  - "Visibility and connector styling"
tags:
  - "kplex-help/reference"
  - "kplex/styling"
  - "kplex/nodes"
Friend:
  - "[[01 Core concepts/Node types]]"
  - "[[04 Filter and focus/Graph Lenses]]"
Previous:
  - "[[05 Personalize and workspace/Note-tab synchronization]]"
---
K-Plex can show or hide categories such as attachments, folders, tags, URLs, unresolved/virtual nodes, inferred relationships and page nodes. Use visibility controls to decide how much structural context you want at once.

Connector appearance is also configurable: color, width, solid/dashed/dotted style, arrowheads, label visibility and text appearance. Ontology-specific link styles can override the base connector style.

This help `data.json` gives Challenger/Watch-out connections a stronger visual treatment and uses separate colors for hierarchical, lateral and sequential ontology fields. That makes the documentation ontology visible even before you read a connector label.

For temporary context-specific styling instead of persistent styles, use [[04 Filter and focus/Graph Lenses|Graph Lenses]].

## This help vault's display choices

The supplied help configuration uses **Siblings off**, **cross-link opacity 50%**, and **100-character regular node labels**. Its saved node, relationship and Graph Lens stroke widths have each been reduced by one point, with a 0.5-point minimum so thin lines remain visible.

**Turn cross-links off separately:** open **Filters and lenses** in the active Plex and turn off **Show cross-links**. This hides additional lines between peripheral nodes without deleting relationships. K-Plex currently initializes that toggle as *on* in each view and does **not** persist it in the plugin's `data.json`; therefore it cannot be pre-disabled by distributing a help-vault settings file. Opacity 50% controls how visible those extra connectors would be **if shown**, not whether they exist.

For a simpler screen, combine that toggle with the vault's already-disabled Siblings setting and, if needed, a [[04 Filter and focus/Quick Filter|Quick Filter]].
