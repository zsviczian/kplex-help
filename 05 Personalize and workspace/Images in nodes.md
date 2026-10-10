---
aliases:
  - "Images in nodes"
tags:
  - "kplex-help/reference"
  - "kplex/styling"
  - "kplex/images"
Friend:
  - "[[01 Core concepts/Node types]]"
Previous:
  - "[[05 Personalize and workspace/Node styles from help tags]]"
Next:
  - "[[05 Personalize and workspace/Sidecar]]"
---
A note can reference a small image through a property or Dataview-style inline field. By default:

```markdown
thumbnail:: [[image.jpg]]
node-image:: [[image.jpg]]
```

- `thumbnail` shows a small image before the label.
- `node-image` replaces the visible label with a compact image while preserving the node footprint and accessible identity.

Image attachments can also appear as their own nodes and can render as **file name**, **thumbnail + file name**, or **image only**.

The property names are configurable. Image-only presentation fields are treated as presentation metadata rather than automatically creating duplicate inferred child relationships.
