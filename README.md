# Claude-MCP

MCP server configurations for use with Claude Code.

## UpPromote MCP

Registered in `.mcp.json` as `uppromote-mcp` (HTTP transport, `https://mcp.uppromote.com/mcp`).

The auth token is read from the `UPPROMOTE_MCP_TOKEN` environment variable rather than
being committed to this repo. Before using this server, set it in your shell or local
environment:

```sh
export UPPROMOTE_MCP_TOKEN="mcp_..."
```

Claude Code expands `${UPPROMOTE_MCP_TOKEN}` in `.mcp.json` at startup, so the real token
never needs to be checked into source control.
