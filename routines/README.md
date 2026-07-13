# Cloud Routine Prompts

These five files are the production path. Paste each one **verbatim** into
its corresponding Claude Code cloud routine (Routines → New Routine). Do not
paraphrase — the env-var check block and the commit-and-push step are
load-bearing.

| File | Cron (America/Chicago) | Purpose |
|---|---|---|
| `pre-market.md` | `0 6 * * 1-5` | Research catalysts, write today's trade ideas |
| `market-open.md` | `30 8 * * 1-5` | Execute planned trades, set trailing stops |
| `midday.md` | `0 12 * * 1-5` | Cut losers, tighten stops on winners |
| `daily-summary.md` | `0 15 * * 1-5` | Snapshot portfolio, send chat recap |
| `weekly-review.md` | `0 16 * * 5` | Weekly stats, grade, strategy updates |

Each routine needs these environment variables set in its routine config
(not a `.env` file), and "Allow unrestricted branch pushes" enabled — see
the main setup guide, Part 7.
