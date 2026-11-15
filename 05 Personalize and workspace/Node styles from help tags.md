---
aliases:
  - "Node styles from help tags"
tags:
  - "kplex-help/reference"
  - "kplex/styling"
  - "kplex/tags"
Friend:
  - "[[How to use this help vault]]"
Previous:
  - "[[Layout density and typography]]"
Next:
  - "[[Images in nodes]]"
---
# Node styles from help tags

Tell a task, concept or caution apart before opening it. Use note types or tags to give those kinds of notes a consistent visual identity.

![[Screenshot - Shared note type style.png]]

*Desktop: the shared #Guide style includes Node details for optional document properties. Add fields deliberately; the editor does not populate existing notes automatically.*

| Style tag | Meaning in the help |
| --- | --- |
| `#kplex-help/home` | Main entrance |
| `#kplex-help/section` | Reference section hub |
| `#kplex-help/path` | Curated, task-based discovery route |
| `#kplex-help/concept` | Explanation of a concept |
| `#kplex-help/how-to` | Step-by-step action |
| `#kplex-help/reference` | Detailed reference |
| `#kplex-help/caution` | Important boundary or risk |
| `#kplex-help/example` | Use case or demonstration |
| `#kplex-help/about` | About the project and its community |

Topic tags (such as `#kplex/indexing` or `#kplex/navigation`) add a second way to browse and filter notes. A topic tag is not the same as the visual style tag.

K-Plex uses one shared style per tag, displayed with its # prefix. The configured **Node style property** (default: `Note type`) selects the tag style that has priority for that note. Existing note-type and tag styles migrate into the shared definitions; the same tag can still classify other notes normally.

**Try it:** Visit [[Choose a topic|Choose a topic]] and compare the look of a path, section, concept and how-to note. Then inspect **Settings → K-Plex → Visual styling → Node styling → Node styles**.

## Give a note a type and useful details

Use a Markdown node's **Set note type** action to choose a valid tag/type. K-Plex updates the configured document property and matching YAML tag together. Review whether to keep the old type as an ordinary tag when replacing it; Clear removes the selected type deliberately.

In the shared style editor, define up to **16 ordered document properties** to show below the name. Enable the useful rows and inspect the preview for your selected note. Property text has its own global font size. These definitions describe what to display; they do not silently add data to existing notes.

**Add missing properties** previews a single eligible note's absent fields before writing them. **Review note types** finds invalid types, missing matching tags and missing configured properties for explicit review. Existing values, including empty, false or null values, are kept. A Markdown node can also open Obsidian's native **File properties** sidebar.
