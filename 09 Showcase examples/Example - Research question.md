---
aliases:
  - "Example - Research question"
tags:
  - "kplex-help/example"
  - "kplex/use-cases"
  - "kplex/research"
Parent:
  - "[[07 Use cases/Research and learning]]"
Related:
  - "[[01 Core concepts/The spatial relationship model]]"
---
This is a deliberately small demonstration node rather than a full help article. Its frontmatter contains:

```yaml
Parent: [[07 Use cases/Research and learning]]
Related: [[01 Core concepts/The spatial relationship model]]
```

Make this note the center in K-Plex. **Research and learning** should appear above it because the relationship is declared from this child note with the literal `Parent` ontology field. The spatial-model note appears to the left through the custom `Related` → Friend ontology.

This pattern is useful when the most natural place to store hierarchy is on the child rather than on the parent hub.
