---
aliases:
- Connection details and evidence
tags:
- kplex-help/reference
- kplex/relationships
- kplex/evidence
Friend:
- '[[Relationship sources and inference]]'
- '[[Graph Lenses]]'
Previous:
- '[[Drag drop and reclassify]]'
Next:
- '[[Unlink and delete]]'
Related:
- "[[Remove one relationship source]]"
learningMode: "read"
sessionSize: "short"
---
# Connection details and evidence

Does a connection look surprising? Open Connection details to see which note, property or link supports it before making an edit.

![[Screenshot - Connection Details Context Menu.png|291]]

The explanation view shows the resolved relationship, active ontology, and the source evidence supporting it. Repeated evidence pointing to the same physical source location is deduplicated, and **Go to source** can navigate to the exact Markdown occurrence.

![[Screenshot - Connection Details.png]]

Use the ontology action to add an explicit document property. For a connection that already has ontology, this adds another declaration rather than editing the existing one. Choose the owning note and field, review the resulting statement, then save. To change a configured field's meaning or description, use its pencil/**Edit** action. To edit an authored occurrence in Markdown, use **Go to source**.

This is especially important when one edge is supported by several links or fields. A graph edge is a resolved view; evidence tells you what you would actually be editing.

**Date edges:** Connection details can identify a `Date` source. Its scalar date value is not a list of physical wikilinks that K-Plex can directly relink or unlink; edit the native Date property in the original note. See [[Date properties and daily notes|Date properties and daily notes]].

## Remove only the source you mean to change

From **Connection details…**, an eligible frontmatter relationship source can now be **removed individually with confirmation**. This does not mean all evidence for the visible edge will be deleted. The action revalidates the source before writing, so an edited or replaced property occurrence is not removed based on a stale snapshot.

Use [[Remove one relationship source|Remove one relationship source]] for a practical walkthrough. Inferred-only evidence remains different from an editable frontmatter declaration.

## Move a property to the other note

An eligible property source offers **Flip owner** alongside Edit and Go to source. This moves just that selected field-to-target declaration to the other Markdown note, using its inverse field. It is useful when the same connection should be written from the other endpoint.

The confirmation shows **Current relationship** and **After saving** together. Review both, then **Save relationship** or **Cancel**. You do not need to flip it a second time inside the confirmation. Other properties and Markdown-body links stay in place; the new declaration is saved before the old one is removed. Both owners must be real Markdown notes. If the source changed while the dialog was open, inspect it again before retrying.
