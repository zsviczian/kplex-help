---
aliases:
  - "Opening this vault"
tags:
  - "kplex-help/reference"
  - "kplex/getting-started"
Guide:
  - "[[00 Start Here/K-Plex Help]]"
---
This is an **end-user guide and live showcase** for K-Plex in Obsidian. The notes use K-Plex relationships, searchable tags, topic-based discovery paths, screenshots and images.

## Open this vault

1. Extract the archive and open its **K-Plex Help** folder as an Obsidian vault.
2. Install or enable the **K-Plex** community plugin if you have not already. The archive contains help files and configuration, **not executable K-Plex plugin code**.
3. Your preconfigured settings are in `.obsidian/plugins/k-plex/data.json`.
4. Run **Open K-Plex**, use **Alt/Option+/** (current new-install default) to focus Search Vault, and search for **K-Plex Help**.
5. Open [[00 Start Here/Choose a topic|Choose a topic]] to choose a task-led route, or [[00 Start Here/First 5 minutes|First 5 minutes]] for the quickest introduction.

## What you can explore

You can browse the same information through ordinary folders, Markdown wikilinks and a K-Plex graph: Parent/Child hierarchy, related Friends, Challengers, Previous/Next sequences, node styling by tag, URLs, images, Graph Lenses and other features.

The 10 discovery paths reuse the existing reference notes rather than copying their text. If this is your first session, open [[00 Start Here/K-Plex Help|K-Plex Help]] as your home base.

## Newly covered workflows

Open [[00 Start Here/Recently added features|Recently added features]] for the local command palette, keyboard navigation, configurable action shortcuts, fullscreen/Zen, Date relationships and indexing status. The [[00 Start Here/Choose a topic|topic chooser]] now offers 13 curated routes.

## October 10 help update

This update documents the October 9–10 merged K-Plex improvements and refreshes the Help ontology links and topic journeys. The `.obsidian/plugins/k-plex/data.json` settings set:

- `renderSiblings: false`
- `crossLinkOpacity: 50`
- `baseNodeStyle.maxLabelLength: 100`
- All existing numeric `strokeWidth` values reduced by 1, with a minimum of 0.5.

**Important:** The current K-Plex implementation initializes `Show cross-links` as a **view-local React Quick Filter switch**, not a `data.json` setting. To hide them, open **Filters and lenses → Show cross-links** in K-Plex. The vault cannot persist this switch across view mounting without a plugin change.

The official Sketch Your Mind book cover is displayed via the official GitHub-hosted image URL. It requires online access; other existing help assets remain packaged in the ZIP.

This is an end-user help vault, not a K-Plex plugin release or a plugin code change.
