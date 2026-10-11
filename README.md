# Stagewright plugins

The [Stagewright](https://stagewright.ai) plugin for coding agents: set Stagewright up from your repo (no account needed), write and fix narrated product walkthroughs that double as end-to-end checks, gather the product context that makes them right from the tools your team already uses, run recurring routines, and triage walkthrough results on pull requests.

## Claude Code

```
/plugin marketplace add stagewright-ai/plugins
/plugin install stagewright@stagewright
```

Then, in your repository: `/stagewright:init`.

## Codex

```
codex plugin marketplace add stagewright-ai/plugins
```

Then install **Stagewright** from `/plugins`, and ask Codex to "set up Stagewright in this repo from what it already has".

## Cursor and other agents

```sh
npx skills add stagewright-ai/plugins          # the skills
npx stagewright@latest skills add              # or: copy them in with the CLI
```

and add the MCP server (stdio): `npx -y stagewright@latest mcp`. Or connect any MCP client to `https://api.stagewright.ai/mcp`.

Everything the plugin includes, and what each command does: [plugins/stagewright](plugins/stagewright/README.md).

This repository is published from Stagewright's main repository whenever the plugin changes, so changes are made there. Issues are welcome here; questions to support@stagewright.ai.
