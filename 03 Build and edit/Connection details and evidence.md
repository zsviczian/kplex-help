---
aliases:
- Connection details and evidence
tags:
- kplex-help/reference
- kplex/relationships
- kplex/evidence
Friend:
- '[[01 Core concepts/Relationship sources and inference]]'
- '[[04 Filter and focus/Graph Lenses]]'
Previous:
- '[[03 Build and edit/Drag drop and reclassify]]'
Next:
- '[[03 Build and edit/Unlink and delete]]'
Related:
- "[[03 Build and edit/Remove one relationship source]]"
---
Right-click a connector and choose **Connection details…** when you want to know **why this edge exists**.

![[Screenshot - Connection Details Context Menu.png|291]]

The explanation view shows the resolved relationship, active ontology, and the source evidence supporting it. Repeated evidence pointing to the same physical source location is deduplicated, and **Go to source** can navigate to the exact Markdown occurrence.

![[Screenshot - Connection Details.png]]

For an inferred relationship, **Specify ontology…** adds the first explicit ontology. For a relationship that already has ontology, **Add ontology…** adds another explicit property without deleting existing sources.

This is especially important when one edge is supported by several links or fields. A graph edge is a resolved view; evidence tells you what you would actually be editing.

**Date edges:** Connection details can identify a `Date` source. Its scalar date value is not a list of physical wikilinks that K-Plex can directly relink or unlink; edit the native Date property in the original note. See [[03 Build and edit/Date properties and daily notes|Date properties and daily notes]].

## Remove only the source you mean to change

From **Connection details…**, an eligible frontmatter relationship source can now be **removed individually with confirmation**. This does not mean all evidence for the visible edge will be deleted. The action revalidates the source before writing, so an edited or replaced property occurrence is not removed based on a stale snapshot.

Use [[03 Build and edit/Remove one relationship source|Remove one relationship source]] for a practical walkthrough. Inferred-only evidence remains different from an editable frontmatter declaration.

[Change: PR #108](https://github.com/zsviczian/kplex/pull/108).
