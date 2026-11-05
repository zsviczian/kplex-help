---
aliases:
- kplexAPI
- K-Plex API
- Scripting and AI assistants
tags:
- kplex-help/section
- kplex/automation
Guide:
- '[[Build and edit]]'
Child:
- '[[K-Plex API examples]]'
- '[[Use K-Plex through Obsidian CLI]]'
Friend:
- '[[Manage and clean up ontology]]'
- '[[Export and share a canvas]]'
- '[[Bring a connected outline into your writing]]'
Related:
- '[[skill]]'
- https://github.com/zsviczian/kplex/blob/main/docs/PUBLIC_API.md
---
# Automation and scripting

Give a local script or assistant the context your map already contains. K-Plex's public API can explain your ontology, find indexed notes, inspect why two notes connect, and describe one open canvas without copying all of your note bodies.

## Choose your starting point

- **Write JavaScript inside Obsidian:** [[K-Plex API examples|try the API examples]]. The exact entry point is `window.kplexApi.v1` — capital A, lowercase pi.
- **Work from a terminal:** [[Use K-Plex through Obsidian CLI|call the same API through Obsidian CLI]].
- **Point Codex, Claude or another local assistant at the interface:** give it the [[skill|skill.md file]], or copy that file into your tool's skill setup under its required filename. The skill explains vault selection, read results and deliberate canvas actions.

## What you can ask for

Read configured relationship fields and their descriptions, search the currently indexed vocabulary, inspect a note's neighbors and the evidence behind a connection, or obtain the context of a particular canvas. Scripts can navigate an existing canvas, choose its view or Facets preset, and obtain a committed Mind Map as Markdown. GraphQL is available for combining read queries.

Portable preset and lens packages can also be listed, exported, validated and imported through a review-and-confirm workflow. The [complete API reference](https://github.com/zsviczian/kplex/blob/main/docs/PUBLIC_API.md) covers that advanced workflow and the full method list.

## Know what the result covers

The indexed graph and a displayed canvas are different views of your knowledge. Graph queries are independent of a canvas's filters. Canvas context describes constructed occurrences, including filter and viewport information; it is not the text of the underlying notes.

Every operation reports success or a named error. Reads also report coverage and truncation. A partial empty result cannot prove that a note has no relationships. Graph reads do not start indexing or wait for it to finish. Optional ontology usage lookup reads stored metadata, while explicit occurrence inspection reads the selected saved note; neither silently starts a full indexing pass.

The API runs locally inside Obsidian and opens no network service. Connecting an assistant is your choice; the assistant's own provider and data-sharing behavior still apply. K-Plex supplies no note or relationship editing methods through this API. Use Obsidian's normal file/property tools for changes you intend to make.

## Plan a consistent ontology

Local tools can discover which documents use a field, inspect exact occurrences in selected saved notes, and prepare reviewed assignments, descriptions and inverse pairs. Ontology completion also shares K-Plex's configured suggestions with other inputs. Start with [[K-Plex API examples|the examples]] and the [[Use K-Plex through Obsidian CLI|CLI guide]]. Configuration review and note-text migration remain separate actions; an analysis request authorizes neither automatically.
