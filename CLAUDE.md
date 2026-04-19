# dolt-db-skills

This repo is used to develop and run skills for working with the BusMgmtBenchmarks Dolt database — a financial data project tracking retail company financials from SEC 10-K filings and Yahoo Finance.

## Skills

Skills are defined in `.skillshare/skills/` and synced to Claude Code (and other AI tools) via the `skillshare` CLI.

### Available Skills

- `/analyze-financials TICKER YEAR` — Fetches financials from SEC, Yahoo Finance, and the Dolt DB, compares them side by side, detects anomalies, and produces reconciled DB-ready values. Saves a report to `reports/`.
- `/insert-financials TICKER YEAR` — Generates a `REPLACE INTO` SQL file from the reconciled values produced by `/analyze-financials`. Writes to `extract/2026/inserts/`. Does NOT write to the database directly.

Always run `/analyze-financials` before `/insert-financials` in the same session.

## MCP Server

The Dolt MCP server is configured in `configs/mcp-servers.conf`:

```
dolt=https://bus-mgmt-databases.mcp.mathplosion.com/mcp-dolt-database/sse
```

The target database is `calvinw/BusMgmtBenchmarks/main`.

## Setup (on new container)

```bash
setup-env.sh && install-mcps.sh   # runs automatically on container creation
setup-skills.sh                    # installs skillshare CLI (run once manually)
sync-skills.sh                     # syncs .skillshare/skills/ to all AI tools
```

If skills are missing after container creation, run `setup-skills.sh` then `sync-skills.sh`, then restart Claude Code.

## Skill Development

To add or edit a skill, modify the `SKILL.md` file in `.skillshare/skills/<skill-name>/`, then run:

```bash
sync-skills.sh
```

Then restart Claude Code for the changes to take effect.
