---
tags:
- "kplex-help/how-to"
- "kplex/canvas"
Guide:
- "[[04 Filter and focus/Facets]]"
Related:
- "[[09 Showcase examples/Example - Read by topic]]"
- "[[09 Showcase examples/Example - Workbench questions]]"
- "[[04 Filter and focus/Graph Lenses]]"
---
# Choose layouts and read classification

Arrange categories so comparisons or next steps are easy to see. Then use the status areas to tell a genuine data gap from a note that needs attention.

## Choose an arrangement

| Layout | Useful for |
| --- | --- |
| **Circular** | Comparing several perspectives around one idea without a first-to-last direction |
| **Concentric** | Showing layers of context around the focus |
| **Horizontal** | Reading a sequence across the canvas |
| **Vertical** | Reading stages down the canvas or placing the focus beside a sequence |
| **Quadrants** | Comparing exactly four categories, such as two choices on two axes |

Choose the layout in the preset editor. Horizontal and vertical layouts let you choose where the focus sits and reverse the category placement. Quadrants need four categories; other category counts use a fallback arrangement.

Set category width and height defaults in the preset, or resize an area on the canvas. Wider areas can fit cards in more columns; taller areas show more rows. Overflow stays inside an area so the focus remains accessible. Canvas resize choices and preset defaults serve different purposes: a preset establishes the starting dimensions, while a particular canvas can retain its own area sizes.

For a linear workflow, guides can use arrows, plain lines or no visible line, with optional captions and per-step overrides. They explain the order of categories; only note connectors represent actual note relationships.

## Understand the four sources

**Property** reads the named Markdown field. **Note type** reads the configured Note type value. **Tags** checks the note's actual tags in their displayed form, including the leading `#`. All three compare against the exact values configured for each category.

**Category rule** combines conditions through the same visual condition editor and Code syntax used by Graph Lenses. For example, `note.learningMode == "read" and note.sessionSize == "short"` places a short reading guide in one quadrant. `note` refers to the candidate; `this` can refer to the focused note. Rules using relationship evidence need a real relationship context; the focus does not have a made-up relationship to itself.

## Read status before making a decision

- **Unassigned:** no configured category matches. A missing property can be a legitimate reason.
- **Conflicting:** more than one category matches. A note with two relevant tags is a useful example, not necessarily an error.
- **Checking:** required local metadata is being prepared.
- **Cannot classify:** the needed metadata, value structure, rule or relationship context is unavailable.

You can combine these into **Diagnostics** or keep separate areas, choose the dock position and hide empty status areas. Combined diagnostics keeps a badge on each note so the reason stays visible. Missing information is not evidence that a rule is false.

Compare [[09 Showcase examples/Example - Read by topic|the tag example]] with [[09 Showcase examples/Example - Workbench questions|the rule example]] to see why both classification and uncertainty matter.
