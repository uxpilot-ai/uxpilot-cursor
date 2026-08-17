# UX Pilot for Cursor

Public Cursor Marketplace plugin. It connects Cursor to UX Pilot over MCP.

MCP URL:

```text
https://mcp-server-485825078314.us-central1.run.app/mcp/ui
```

This repository has no OAuth client secrets.

## Layout

Follows the official [Cursor plugin template](https://github.com/cursor/plugin-template) (one plugin in a multi-plugin marketplace manifest).

- Marketplace: `.cursor-plugin/marketplace.json`
- Plugin: `plugins/uxpilot/`
- MCP config: `plugins/uxpilot/mcp.json`

Validate:

```bash
node scripts/validate-template.mjs
```

Local load: copy or symlink `plugins/uxpilot` to `~/.cursor/plugins/local/uxpilot`, then reload Cursor.

Submit this GitHub URL at [cursor.com/marketplace/publish](https://cursor.com/marketplace/publish) after the repo is public.

## License

MIT
