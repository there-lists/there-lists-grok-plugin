# There Lists plugin for Grok Build

Connect Grok to [There Lists](https://apps.apple.com/app/id6810781564), the iOS shopping-list app that reminds you when you arrive at a store.

## What you get
- **MCP server** `there-lists` at `https://there-connector.hoonie1107.workers.dev/api/mcp` (Streamable HTTP, OAuth).
- **Skill** `there-lists`: how to use the tools safely (look up IDs first, confirm destructive changes).

| Tool | Purpose |
|---|---|
| `list_lists` | List your shopping lists |
| `get_list` | Read one list's items |
| `add_items` | Add items to a list |
| `check_item` / `uncheck_item` | Mark an item bought / not bought |
| `list_stores` | Show saved stores |
| `tidy` | Propose cleanup of a list (needs confirmation) |
| `confirm_action` | Apply a change the user confirmed |

## Authentication & requirements
Sign in with Apple via OAuth on first connection. No API key; never paste credentials into chat.
Requires **There Plus** ($2.99 one-time in-app purchase). Without it, tools return `plus_required`.

## Network endpoints
Only `there-connector.hoonie1107.workers.dev` (the There Lists connector, a Cloudflare Worker). No hooks, no scripts, no local code execution, no telemetry.

## Privacy & support
- Privacy policy: TODO_PRIVACY_URL
- Support: TODO_SUPPORT_EMAIL

## License
MIT
