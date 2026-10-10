---
tags:
- kplex-help/example
- kplex/use-cases
- kplex/dates
Parent:
- '[[07 Use cases/Meeting notes and daily notes]]'
Friend:
- '[[03 Build and edit/Date properties and daily notes]]'
Date: '2026-10-09'
---
**This note contains a real native Date value in its properties.** Its `Date` value is `2026-10-09` (see the YAML at the top of the file). A companion file named `2026-10-09.md` exists in this vault root.

## Try it

1. Enable Obsidian's **Daily notes** core plugin (already enabled in the supplied vault), use the default `YYYY-MM-DD` format and the vault root as the Daily Notes location, and ensure this note's `Date` field has the native **Date** property type.
2. Center this note in K-Plex. With **Default Date role = Parent**, the note for **2026-10-09** can appear as a **Parent**. This example also has a separate `Parent` property pointing to **Meeting notes and daily notes**—the two have different evidence sources.
3. Choose another **Default Date role** under **Settings → K-Plex → Plex behavior → Relationship behavior**. K-Plex should reinterpret just the unconfigured scalar Date link without rewriting the date.
4. Explicitly map the `Date` field in **Ontology → Relationship fields** (for instance, as **Challenger**) and observe that the explicit mapping takes priority. Restore the default when finished if this is a shared help vault.

> [!important] What if the date node doesn't appear?
> Obsidian must recognize the field as Date and resolve its Daily Notes target under the active format/folder. If your Obsidian Daily Notes configuration differs, the sample is still a useful written example; inspect its Date property and refer to the [[03 Build and edit/Date properties and daily notes|Date properties and daily notes]] guide.

Use **Connection details** on the Date edge to inspect its Date-property origin. Edit the scalar date in Obsidian rather than trying to remove it as a standard wiki-link.
