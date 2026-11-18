---
name: boardwalk
description: Look up US planned construction projects and building permits through the Boardwalk MCP. Use when the user asks about filings, permits, alerts, lists, or exports.
---

# Boardwalk

Boardwalk records what a public filing stated. A blank field was not in the filing. Say what is known. Do not invent a project, a permit number, or a contact.

Sign-in is the user's own Boardwalk account. If a tool says an active trial or plan is needed, relay that sentence. Do not invent an API key.

## How to search

- Planned work (rezones, plats, site plans, approvals) uses the project tools. Building work already permitted (roofs, pools, new homes, who pulled the permit) uses the permit tools. When either could answer, count both.
- Call `count_projects` or `count_permits` before fetching rows. Counts are free. Keep a chat page around 25 rows, and never more than 50. If the count is over 250 and they want to review it in chat, tell them the number and tighten the filters or work in batches. If they asked for a CSV, CRM, or email, use the export tool instead of pasting rows.
- `q` on the count and search tools is the map search box (name, developer, words from the filing). Use `ai_search_projects` only when they need a passage from the minutes.
- A saved alert or list is `list_alerts` / `list_user_lists`, then the match or list tool. Do not search the whole database for a name they already saved. Permit alerts use `palr_` ids. Project alerts use `alr_` ids.
- Do not call `run_alert` unless they asked to run it now. Confirm `create_enrichment` before starting it. Confirm `delete_alert` before deleting it.
- `describe_data` lists questions this corpus cannot answer. If the question is on that list, say so and stop.

The full instructions, including credit rules, are at https://boardwalkai.com/skills/cursor.md.
