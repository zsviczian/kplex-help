---
tags:
- "kplex-help/how-to"
- "kplex/canvas"
Guide:
- "[[04 Filter and focus/Facets]]"
Friend:
- "[[04 Filter and focus/Graph Lenses]]"
Related:
- "[[04 Filter and focus/Define a Facets workflow]]"
---
# Reuse a preset or lens in another vault

Keep a useful workflow when you move between vaults, or share it with someone who uses different notes. Export its definition and review what will be imported.

## Share only what is useful

1. Select **Export preset** beside a workflow in **Manage presets**. A Graph Lens editor can export a lens on its own.
2. Select any companion lenses explicitly, then choose **Copy JSON** or **Download JSON**. Only referenced palette colors accompany the definition.
3. Review the exported data before sending it. Names, field values, rules and help may contain terms specific to your vault.
4. In the destination vault, import the JSON and review the preview. Choose whether to create a new entry or replace an existing one, which companion lenses to include, and whether to keep existing palette values or use the imported ones.
5. Select the imported preset or lens and adapt its fields and values to the destination notes.

A preset can include its own Markdown help, category colors, layout, sizing and workflow guides. A standalone Graph Lens can be shared without a Facets preset. Sharing a definition does not send the notes it describes, nor does importing one enable it on every canvas.

## Ask for help authoring a preset

An export can include authoring context that explains the supported data format. If you choose to give that text to an AI service, review it yourself and remove private terms first. K-Plex does not silently send your notes to a service. Generated JSON still needs the normal import preview and validation.

Use [[04 Filter and focus/Define a Facets workflow|the workflow guide]] to decide what the definition should accomplish before sharing it.
