---
aliases:
- Manage ontology
- Find documents using a relationship field
- Clean up misspelled ontology
tags:
- kplex-help/how-to
- kplex/ontology
- kplex/relationships
Guide:
- '[[03 Build and edit/Build and edit]]'
Related:
- '[[01 Core concepts/Ontology and relationship fields]]'
- '[[03 Build and edit/Connection details and evidence]]'
- '[[07 Use cases/Garden your vault]]'
Friend:
- '[[07 Use cases/Garden your vault]]'
Watch out:
- '[[03 Build and edit/Remove one relationship source]]'
---
# Manage and clean up ontology

Found a misspelled relationship property, or want to understand where a field is used? Manage ontology helps you find its notes and choose a clear, consistent meaning.

## Find a field

1. Open **Settings → K-Plex → Ontology → Manage ontology**.
2. Search for part of a property name or its paired name. Use the role filter to narrow the list; **Unassigned** is useful when cleaning up unfamiliar fields.
3. Open a row to assign a role, configure **Pair with**, or inspect the existing assignment. Paired fields appear together.

In this vault, search for **Guide**. Its partner **Explains** describes the same hierarchy from the opposite endpoint. See [[01 Core concepts/Ontology and relationship fields]] before changing the direction of an existing pair.

![[Assets/Screenshot - Ontology pairs.png]]

*Search for Guide to see its paired Explains assignment without changing either note property.*

## Define a field when you need it

In **Pair with**, type the missing partner's property name and choose **Create … as paired field**. Save to define both fields together; the partner receives the reciprocal role. You do not need to add the new property to a note first.

When adding or specifying ontology for a connection, choose **Create ontology…** in its **Note property** selector. Define the field and optional partner, then return to the connection with the saved field selected. Confirm the connection to apply it to the note. Creating a definition alone does not change note properties.

## See the documents behind it

Open the field, then select **Show documents**. The list uses information already available to K-Plex; opening it does not start an extra whole-vault indexing pass.

- Type a keyword to filter document names and paths.
- Open an item in K-Plex to explore its context, or use its separate action to open it in a new Obsidian tab.
- Copy the list as Markdown when you want a cleanup checklist or a record of the affected notes.
- Use **Refresh** after editing a note. A list can be incomplete while indexing continues; zero results are not a substitute for reviewing incomplete coverage.

![[Assets/Screenshot - Ontology documents.png]]

*Documents using Explains, filtered to Use cases. The separate row actions open a canvas or an Obsidian tab; the top button copies the filtered list.*

## Remove stale discoveries

After correcting the field in the actual notes, return to **Manage ontology** and select **Refresh counts**. An **Unassigned** field with zero matching documents disappears from the list. An assigned field remains available at zero uses because its configuration may be intentional.

The manager does not rename note properties for you. Removing an assignment changes K-Plex's interpretation; it does not remove that property or its links from Markdown. Inspect [[03 Build and edit/Connection details and evidence]] before removing a relationship source.

**Try it:** search for **Explains**, open **Show documents**, and filter for **Use cases**. Open one result in K-Plex, then compare it with the note's frontmatter in Obsidian.

## Related help

- [[01 Core concepts/Ontology and relationship fields]] — roles, pairs and ordinary note properties.
- [[03 Build and edit/Remove one relationship source]] — remove one authored contribution safely.
- [[07 Use cases/Garden your vault]] — make cleanup part of normal exploration.
