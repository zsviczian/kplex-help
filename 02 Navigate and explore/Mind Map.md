---
tags:
- "kplex-help/how-to"
- "kplex/canvas"
Guide:
- "[[Canvas views]]"
Related:
- "[[Screenshot - Mind Map workshop.png]]"
- "[[Example - Workshop plan]]"
- "[[Compass]]"
- "[[Facets]]"
Friend:
- "[[Expand a note into sections]]"
---
# Develop a hierarchy with Mind Map

Keep an outline in view while exploring its branches. Mind Map keeps its root while you unfold branches or move keyboard selection. Center a note when you want to start the map from that idea.

## Try the workshop hierarchy

1. Center [[Example - Workshop plan|the workshop plan]], then choose **Mind Map** in **Views and lenses**.
2. Unfold the materials branch to reveal its source notes. Use **Expand one generation** to reveal another layer, or fold an individual branch.
3. Use the arrow keys to select and reveal a source note. The plan remains the map root; moving keyboard selection does not change the centered note.
4. Click a note or press **Enter** to center it and make it the map root. **Use as map root** and **Use current note as map root** also offer explicit root changes.

With the default shortcuts, **Alt/Option+Enter** folds or unfolds the selected branch; its chevron does the same without centering the note. **Ctrl/Cmd+Enter** opens the selected note in a new native tab. Your saved shortcuts may override these defaults.

![[Screenshot - Mind Map workshop.png]]

*Desktop layout example: the workshop plan stays at the root while the materials branch unfolds. The visible Incomplete metadata labels and attachment placeholders are preparation states; this image illustrates arrangement and branch controls.*

## Shape an outline without losing its context

The child tree can grow left, right or in a balanced arrangement. Parents stay above the root; peer context stays separate from the child tree. Parent areas grow upward to fit their branches; their height setting establishes a minimum. Pan and zoom the canvas to reach longer branches. Change spacing, density, initial generations and display limits in **Settings → K-Plex → Canvas behavior → Views → Mind Map**.

Repeated and circular relationships can appear as references rather than expanding forever. A branch may still be preparing, have incomplete metadata, or reach a display limit. Those states do not mean the underlying note has no children.

## Write where the idea belongs

Open a Markdown node in its place in the map and use Obsidian's editor. There is one node editor at a time. With the central note open in the editor, click another Markdown note to center it: K-Plex saves the previous note and opens the new center in the same reading or editing mode, preserving the editor's dimensions. You can keep navigating while the next editor loads. A failed save keeps the current editor available.

Close an editor before folding away the branch that contains it. Switching views saves and closes it. Folding a branch and expanding a note's Markdown sections are different actions.

## Use your outline elsewhere

Choose **Export → Canvas to MindMap Markdown** in the canvas context menu to copy or save the constructed map or a selected branch. The outline keeps links and supported cross-links; folds and filters still limit its scope. Choose **Canvas to image** for a PNG instead. See [[Export and share a canvas|Export and share a canvas]] for preview choices and limitations.

## Use the view that suits the task

Return to [[Compass|Compass]] when you want the selected note's immediate neighborhood. Try [[Facets|Facets]] when the useful question is which category each connected note belongs to.
