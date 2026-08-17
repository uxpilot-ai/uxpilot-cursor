# UX Pilot for Cursor

Connects [Cursor](https://cursor.com) to [UX Pilot](https://uxpilot.ai) over MCP so Agent can use your UX Pilot workspace tools.

## What this plugin does

It registers a remote MCP server:

`https://mcp-server-485825078314.us-central1.run.app/mcp/ui`

After install, sign in with your UX Pilot account (OAuth). Do not put API keys or OAuth secrets in this repo.

## Install

### Cursor Marketplace

Install **UX Pilot** from Customize when the listing is live.

### Local (development)

1. Copy or symlink this folder to `~/.cursor/plugins/local/uxpilot`
2. Reload the Cursor window (**Developer: Reload Window**)
3. Open **Customize**, connect the UX Pilot MCP server, and complete OAuth

## Widgets

Cursor supports [MCP Apps](https://cursor.com/docs/mcp.md). Generation and confirmation UIs may render in a sandboxed iframe. That is not guaranteed to match ChatGPT. If a widget is missing, listing and edit tools still work through normal tool results. Destructive actions (delete, publish) stay confirmation-gated and must not complete from the model alone.

On some Cursor versions the iframe is inside a collapsed tool-call group; expand it to see the UI.

## MCP path

Use `/mcp/ui` (this plugin). ChatGPT uses `/mcp`. Do not point Cursor at `/mcp`.
