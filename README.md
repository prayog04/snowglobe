# Trading Bot

An autonomous, cloud-scheduled swing-trading agent built on Claude Code.
It places (currently paper) trades on Alpaca, writes its own daily
research, executes a disciplined strategy with hard rules, and notifies
you via ClickUp. It is stateless between runs — all memory lives in this
repo, committed to `main`.

## Layout

- `CLAUDE.md` — agent rulebook, auto-loaded every session.
- `scripts/` — the only way the agent touches the outside world:
  - `alpaca.sh` — trading (account, positions, orders)
  - `perplexity.sh` — market research
  - `clickup.sh` — chat notifications
- `.claude/commands/` — local slash commands (`/portfolio`, `/trade`,
  `/pre-market`, `/market-open`, `/midday`, `/daily-summary`,
  `/weekly-review`). Use these for manual/local runs against `.env`.
- `routines/` — the five cloud routine prompts (the production path).
  Paste these verbatim into Claude Code cloud routines on a cron schedule.
- `memory/` — the agent's persistent state, committed to `main`:
  `TRADING-STRATEGY.md`, `TRADE-LOG.md`, `RESEARCH-LOG.md`,
  `WEEKLY-REVIEW.md`, `PROJECT-CONTEXT.md`.

## Local setup

1. `cp env.template .env` and fill in your credentials. `.env` is
   gitignored — never commit it.
2. Open this repo in Claude Code.
3. Run `/portfolio` to smoke-test the Alpaca connection.

## Cloud setup

See `routines/README.md` and the setup guide, Part 7, for creating the
five scheduled cloud routines (GitHub App install, env vars, cron
schedules).

## Trading mode

This repo is currently configured for **paper trading**
(`ALPACA_ENDPOINT=https://paper-api.alpaca.markets/v2` in `env.template`).
Switch to the live endpoint only after you've watched it run correctly
for a while.
