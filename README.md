# Tomo agent skills

The skill for building and fixing a business's WhatsApp and Instagram customer journey on [Tomo](https://tomoapp.co.il) with an AI coding agent (Claude Code, Codex, Cursor and others), through Tomo's builder MCP server.

## Install

```bash
npx skills add Value-Solutions-Global/tomo-skills
```

Update later with `npx skills update`. Tomo's `status` tool names the current version, and the skill tells your agent when its copy is older.

Then connect the MCP server, if your agent has not yet:

```bash
claude mcp add --transport http --scope user tomo https://api.tomoapp.co.il/mcp
```

## Where it comes from

This repo is a copy. The skill is written next to Tomo's MCP server, checked against its tools on every change, and served at https://api.tomoapp.co.il/.well-known/agent-skills/tomo/SKILL.md; a GitHub Action here copies it every hour. Changes made here are overwritten.

## Help

Something wrong with Tomo or with installing: https://tomoapp.co.il/support. Once connected, your agent can open a ticket itself with the `support` tool.
