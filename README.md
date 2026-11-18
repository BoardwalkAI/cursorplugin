# Boardwalk for Cursor

Boardwalk reads public city and county records and returns two datasets: planned projects (what is proposed, where, by whom, and what was decided) and building permits.

The plugin is free. Signing in uses a Boardwalk account, and deliveries past the free trial follow that account's plan. [Privacy](https://boardwalkai.com/privacy) and [terms](https://boardwalkai.com/terms).

## Install

Install **Boardwalk** from the Cursor Marketplace, then enable it under Customize → MCPs. Cursor asks you to sign in with a Boardwalk account. There is no API key in this plugin.

A reviewer can create an account at [boardwalkai.com](https://boardwalkai.com). The free trial can search and export a small number of records. Server URL, for a manual install: `https://mcp.boardwalkai.com/mcp`.

## What the agent should do

Count before pulling records. Counts are free. A page of projects or permits spends the account's export allowance, so keep chat pages small and send a CSV export when someone wants the whole set. Planned projects and building permits are different tools. Say what the filing says, and leave a field blank when the filing did not state it.

The longer agent instructions are at [boardwalkai.com/skills/cursor.md](https://boardwalkai.com/skills/cursor.md).
