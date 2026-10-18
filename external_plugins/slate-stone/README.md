# Slate Stone for Grok Build

Read-only access to the Slate Stone Financial catalog of Excel financial models through the hosted MCP server at `https://mcp.slatestonefinancial.com/mcp` (Streamable HTTP).

## Requirements
An active Slate Stone All-Access subscription (see https://slatestonefinancial.com/pricing/). The subscription includes a personal API key; after subscribing, request it on https://slatestonefinancial.com/contact/ using the email on your subscription. Set it as the `SLATE_STONE_API_KEY` environment variable; the plugin sends it as `Authorization: Bearer <key>`. Keys are read-only and revocable.

Without a key, only `get_pricing` works (it explains how to subscribe); every other tool returns a "subscription required" message.

## Tools (all read-only)
`search_models`, `get_model`, `list_categories`, `get_pricing`, `search`, `fetch`.

## Network endpoints and credentials
- Calls only `https://mcp.slatestonefinancial.com/mcp`.
- Needs only the user's own Slate Stone API key from `SLATE_STONE_API_KEY`. No hooks, no commands, no shell, no file access, no telemetry.

## License
Plugin configuration: MIT. Slate Stone content and models: proprietary, under the terms at https://slatestonefinancial.com/terms/. Educational use only, not financial advice.
