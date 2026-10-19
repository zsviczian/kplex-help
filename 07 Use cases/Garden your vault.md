---
aliases:
- Garden your vault with K-Plex
- Make your vault better one note at a time
- Improve neglected notes without reorganizing everything
Note type: Use case
tags:
- kplex-help/example
- kplex/use-cases
Parent:
- '[[07 Use cases/Use cases]]'
Explains:
- '[[03 Build and edit/Drag drop and reclassify]]'
- '[[05 Personalize and workspace/Note-tab synchronization]]'
- '[[04 Filter and focus/Graph Lenses]]'
- '[[05 Personalize and workspace/Node styles from help tags]]'
Friend:
- '[[03 Build and edit/Connection details and evidence]]'
- '[[07 Use cases/Build a Map of Content]]'
---

# Garden your vault — one note at a time

**The situation:** Your Obsidian vault keeps growing. Some notes are useful but hard to rediscover, others have vague labels or outdated statuses, and some promising ideas are still seedlings. Cleaning up everything at once feels overwhelming, so the maintenance never happens.

**The outcome:** Make a few notes easier to find, understand and reuse every time you explore. Over time, the vault becomes more meaningful without a large reorganization project.

> [!tip] Gardening is not a cleanup marathon
> You can improve a single note in seconds: give it a useful tag, mark its maturity, update a project status, or connect it to a related idea. Do a little whenever you encounter something worth tending.

## Example: make unfinished thinking visible

Imagine you have notes about books, sketches and workshop ideas. Some contain only a rough observation; others are mature insights you can use in a presentation. Add a simple personal property such as `maturity: 1` through `maturity: 5` to describe how developed a note feels. K-Plex doesn't assign these scores for you—you choose the meaning of each value.

Keep the Obsidian **File properties** pane open beside K-Plex. As you move from note to note in the Plex, the unpinned, ungrouped Properties pane follows the central file, letting you adjust its metadata without losing the surrounding graph. If the center is a folder or tag rather than a file, the pane clears. A pinned or grouped Properties pane intentionally does not follow.

Turn on an appropriate [[04 Filter and focus/Graph Lenses|Graph Lens]] with **Style matching** rules to show the maturity values visually: for example, bright styling for seedlings and quieter styling for mature notes. Navigate, update a value, and inspect the changing visual pattern. A Lens operates on the current Plex neighborhood; it is not an automatic quality audit of the entire vault.

## Two simple gardening workflows

### 1. Tag as you explore

Pin a frequently used tag in K-Plex, then explore your notes. When you find a note that belongs to the category, use the supported tag-and-note drag-and-drop or connector action to assign its tag. You can also change or remove editable YAML tag membership when a classification no longer fits. This avoids having to open each note and type metadata by hand.

Where K-Plex offers the choice, apply a tag either as an **ordinary Tag** or as a **Note Type**:

- **Ordinary Tag:** adds useful membership and retrieval context. A note can have several tags.
- **Note Type:** also sets the configured note-style property, giving the note a recognizable semantic appearance. A note has one Note Type; choosing another explicitly replaces that type, while other tags can remain.

Both are useful. Use ordinary tags for multiple overlapping topics, and Note Types for categories you want to recognize at a glance. Tags and Note Types are properties of the underlying notes, not temporary colors drawn only in the graph. See [[03 Build and edit/Drag drop and reclassify]] and [[05 Personalize and workspace/Node styles from help tags]].

### 2. Improve properties while keeping context

Put K-Plex beside Obsidian's built-in **File properties** pane and navigate through a project or topic. Set or refine properties such as `maturity`, `status`, `reviewed`, or `needs-follow-up` as you go.

Pair these properties with saved [[04 Filter and focus/Graph Lenses|Graph Lenses]]: one may highlight early-stage notes, another active projects, and another items worth revisiting. Switch Lenses to view the same neighborhood from a different perspective. For a project, a status-based Lens can make ongoing and finished work look different without moving notes to new folders.

For a broader candidate list, use Obsidian **Bases** or Search to find items matching a property, then bring those notes into K-Plex to inspect their relationships. Bases can also provide a table for batch metadata review; K-Plex adds *why a note matters in context*.

## Beyond tagging

Sometimes the best improvement is not another property. Add a missing source link, connect an idea to its project, clarify a title, or inspect an unexpected edge in [[03 Build and edit/Connection details and evidence|Connection details]] before changing it. Keep the edit small, then continue exploring.

## Why it matters

A vault doesn't become useful merely because it holds more notes. Gardening makes knowledge progressively more **findable, recognizable and connected**. Visual feedback makes small improvements visible and can help you decide where to spend the next few minutes.

**Done when:** You have refined a handful of notes—perhaps tags, Note Types, maturity values or relationships—and can immediately see the result in K-Plex. No perfectly groomed vault is required.

## Explore further

- [[07 Use cases/Never start a project with a blank page|Reuse your better-connected notes in a new project]].
- [[07 Use cases/Build a Map of Content|Give a growing subject an entry point]].
- [[05 Personalize and workspace/Note-tab synchronization|Understand how the Properties pane follows the Plex]].
