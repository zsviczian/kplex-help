---
aliases:
- K-Plex CLI
- Codex and Claude access
tags:
- kplex-help/how-to
- kplex/automation
Guide:
- '[[12 Automation/Automation and scripting]]'
Friend:
- '[[12 Automation/K-Plex API examples]]'
Related:
- '[[skill]]'
- https://help.obsidian.md/cli
- https://github.com/zsviczian/kplex/blob/main/docs/CLI.md
---
# Use K-Plex through Obsidian CLI

Let a terminal script or local assistant inspect your map without a separate server. Obsidian CLI runs JavaScript inside the open application, where it can call the same `window.kplexApi.v1` interface as an Obsidian script.

## Give an assistant the skill

Point Codex, Claude or another local assistant to [[skill.md]] available at https://github.com/zsviczian/kplex-help/blob/main/skill.md.

For example:

> Read the K-Plex skill at `https://github.com/zsviczian/kplex-help/blob/main/skill.md`. In vault `<my-vault>`, find my workshop plan and explain its direct Child relationships. Report any incomplete coverage. Do not change my notes.

The file is also available [directly on GitHub](https://raw.githubusercontent.com/zsviczian/kplex-help/main/skill.md). If your tool installs skills by folder, copy it into a `kplex-obsidian-cli` folder as `SKILL.md` using that tool's installation convention.

CLI eval has the privileges of your Obsidian session. Run local code you trust. The skill guides access; it does not grant an assistant permission to edit notes, import settings, install plugins or send content elsewhere.

## Connect to the intended vault

1. In desktop Obsidian, enable **Settings → General → Command line interface** and follow the registration prompt. See [Obsidian's CLI setup](https://help.obsidian.md/cli) if the command is unavailable.
2. Keep the intended vault open with K-Plex enabled.
3. Address it explicitly with `vault=...` as the first parameter, and verify its path before reading or changing content.

These terminal examples use POSIX shell quoting. Replace `YOUR_VAULT` with your open vault's name or ID:

```sh
obsidian vault=YOUR_VAULT vault info=path
obsidian vault=YOUR_VAULT eval 'code=JSON.stringify(window.kplexApi.v1.capabilities())'
obsidian vault=YOUR_VAULT eval 'code=JSON.stringify(window.kplexApi.v1.ontologyGuide({format:"markdown"}))'
obsidian vault=YOUR_VAULT eval 'code=JSON.stringify(window.kplexApi.v1.search({query:"Workshop",limit:10}))'
obsidian vault=YOUR_VAULT eval 'code=JSON.stringify(window.kplexApi.v1.canvases())'
```

K-Plex supplies no separate `obsidian kplex:*` command family. Use `eval` and the public API. Do not rely on whichever vault or canvas happens to have focus.

## Use a canvas ID from the result

Choose an `id` returned by `canvases()`, then read its context:

```sh
obsidian vault=YOUR_VAULT eval 'code=JSON.stringify(window.kplexApi.v1.context({canvasId:"RETURNED_CANVAS_ID"}))'
```

For a settled Mind Map, return Markdown and its warnings without saving a file:

```sh
obsidian vault=YOUR_VAULT eval 'code=JSON.stringify(window.kplexApi.v1.exportMarkdown({canvasId:"RETURNED_CANVAS_ID"}))'
```

Check `ok` before using `value`, then inspect coverage, truncation and export warnings. See [[12 Automation/K-Plex API examples|the examples]] for neighbors, evidence, GraphQL and navigation with readback. Canvas context does not include note bodies; use ordinary Obsidian reading commands when you deliberately need their content.

## Run from Windows or a script

On Windows, use **Obsidian.com** to capture output. A usual installation path is `C:\Program Files\Obsidian\Obsidian.com`. In PowerShell, a short read without embedded JavaScript string quotes is:

```powershell
& 'C:\Program Files\Obsidian\Obsidian.com' 'vault=YOUR_VAULT' eval 'code=JSON.stringify(window.kplexApi.v1.status())'
```

For scripts with quoted values, pass an argument array rather than building a shell command. Save the following as a local `.mjs` file, replace the vault name, and run it with Node:

```js
import {spawnSync} from 'node:child_process';

const executable = process.env.KPLEX_OBSIDIAN_CLI ??
  (process.platform === 'win32'
    ? 'C:\\Program Files\\Obsidian\\Obsidian.com'
    : 'obsidian');
const vault = 'YOUR_VAULT';
const code = 'JSON.stringify(window.kplexApi.v1.search({query:"Workshop",limit:10}))';
const response = spawnSync(executable,
  [`vault=${vault}`, 'eval', `code=${code}`],
  {encoding: 'utf8', timeout: 30_000, maxBuffer: 4 * 1024 * 1024});
if (response.error || response.status !== 0 || /^Error:/m.test(response.stdout ?? '')) {
  throw response.error ?? new Error(response.stderr || response.stdout || 'CLI failed');
}
const result = JSON.parse(response.stdout.trim().replace(/^=>\s*/, ''));
console.log(JSON.stringify(result, null, 2));
if (!result.ok) process.exitCode = 1;
```

Keep evals short and on one line. An `Error:` response can accompany a zero process exit code. A timeout after an action does not prove nothing happened: reacquire the API and read the affected state before retrying.

## Inspect ontology usage for a cleanup proposal

After capability discovery, CLI eval can await `ontologyDocuments` to find stored usage candidates, then await `inspectOntologyOccurrences` for exact fields in a selected saved note. These are different from passive graph queries: usage reads stored metadata, and occurrence inspection reads the selected source file.

```sh
obsidian vault=YOUR_VAULT eval 'code=(async()=>JSON.stringify(await window.kplexApi.v1.ontologyDocuments({field:"Explains",limit:20})))()'
```

Keep coverage, continuation and unsupported flags with your analysis. Requesting an audit does not authorize text migration or configuration changes. See [[12 Automation/K-Plex API examples|the examples]] for source inspection and reviewed configuration, and give an assistant the updated [[skill|CLI skill]].
