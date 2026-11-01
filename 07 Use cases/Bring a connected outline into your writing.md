---
Note type: Use case
aliases:
- Write from a connected outline
tags:
- kplex-help/example
- kplex/use-cases
Parent:
- '[[07 Use cases/Use cases]]'
Explains:
- '[[03 Build and edit/Export and share a canvas]]'
- '[[12 Automation/Automation and scripting]]'
Friend:
- '[[07 Use cases/Research and learning]]'
- '[[02 Navigate and explore/Mind Map]]'
- '[[09 Showcase examples/Example - Workshop plan]]'
---
# Bring a connected outline into your writing

**The situation:** You have gathered useful notes around a project, but starting a document still means reconstructing the structure you just explored.

**The outcome:** Start writing from a linked outline, keeping your sources close. Share a picture when someone needs the overview rather than the working notes.

## Try it with the workshop plan

Center [[09 Showcase examples/Example - Workshop plan|the workshop plan]], choose Mind Map and unfold the materials you want to use. Keep the branches that belong in your next draft; fold or filter the rest.

![[Assets/Screenshot - Mind Map workshop.png]]

*The workshop map provides a starting structure. Choose the branches you want to carry into a written plan; the screenshot illustrates the map, not the export dialog.*

## Ways to make it happen

### Start the draft from a linked outline

Choose **Export → Canvas to MindMap Markdown** from the canvas context menu. Review **Whole map** or **Selected branch**, choose which ontology labels to include, and copy the preview into a new writing note. Use its links to revisit supporting material as you write. This copies the outline, not every source note's body.

### Share the overview

Choose **Export → Canvas to image**. Use **Current viewport** for a focused illustration or **Whole canvas** for the constructed scene beyond your current framing. Check the preview: scrolling areas keep their clips, and folded branches stay folded. A transparent PNG works well when you want your presentation's background to show through.

### Ask a local assistant to help you prepare

Use [[12 Automation/Automation and scripting|the public API]] to give your assistant the chosen canvas's context and your ontology's meanings. Ask it to inspect a few relevant relationships, acknowledge incomplete coverage and propose an outline. For a Mind Map, it can obtain the Markdown directly through `exportMarkdown()`.

Read the linked notes deliberately when their text is needed, and choose what to share with the assistant. API context describes the map; it does not silently include all note bodies or edit your notes.

**Done when:** You have an outline you can write into, with links back to the notes that support it. Changing that exported outline does not automatically change K-Plex's original relationships.
