---
aliases:
- Images in nodes
tags:
- kplex-help/reference
- kplex/styling
- kplex/images
Friend:
- '[[01 Core concepts/Node types]]'
- '[[07 Use cases/Develop visual ideas]]'
Previous:
- '[[05 Personalize and workspace/Node styles from help tags]]'
Next:
- '[[05 Personalize and workspace/Sidecar]]'
---
A note can reference a small image through a property or Dataview-style inline field. By default:

```markdown
thumbnail:: [[image.jpg]]
node-image:: [[image.jpg]]
```

`thumbnail` shows a small image before the label. `node-image` replaces the visible label with a compact image while preserving the node footprint and accessible identity.

Image attachments can also appear as their own nodes, displayed as **file name**, **thumbnail + file name**, or **image only**. The property names are configurable. Image-only presentation fields are treated as presentation metadata rather than automatically creating duplicate inferred Child relationships.

## Remote images require permission

**Available in 0.1.3:** Remote node images are disabled by default. Enable **Allow remote node images** in K-Plex settings only when you intend to load them. This can send a request to the image's hosting server. Local images do not need this permission.

A remote image embedded in an ordinary Obsidian note and that same image used as a K-Plex node image are different display paths. A book cover visible in the document is not proof that K-Plex's remote-node-image permission is enabled.

For visual thinking, local images or Excalidraw notes can give ideas a recognizable identity. The workflows here do not assume an interface for choosing a particular Excalidraw focus frame as the graph card. See [[03 Build and edit/Excalidraw integration]] and [[07 Use cases/Develop visual ideas]].

[Source: release 0.1.3](https://github.com/zsviczian/kplex/releases/tag/0.1.3).
