---
name: there-lists
description: Use the There Lists MCP tools to read and update the user's There Lists shopping lists.
---
# There Lists

Tools: `list_lists`, `get_list`, `add_items`, `check_item`, `uncheck_item`, `list_stores`, `tidy`, `confirm_action`.

- Call `list_lists` first; never guess list or item IDs.
- Use `get_list` before checking/unchecking so you act on the right item.
- `tidy` and other changes that remove or reorganize items may return a pending action; show the user what will change and only call `confirm_action` after they agree.
- If a tool returns `plus_required`, tell the user Grok access needs There Plus (one-time purchase in the iOS app, Settings > Grok Bot; Restore Purchases is there too).
