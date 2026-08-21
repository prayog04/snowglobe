# Weekly Review

Friday reviews appended here.
Template for each entry:

## Week ending YYYY-MM-DD

### Stats
| Metric | Value |
|--------|-------|
| Starting portfolio | $X |
| Ending portfolio | $X |
| Week return | ±$X (±X%) |
| S&P 500 week | ±X% |
| Bot vs S&P | ±X% |
| Trades | N (W:X / L:Y / open:Z) |
| Win rate | X% |
| Best trade | SYM +X% |
| Worst trade | SYM -X% |
| Profit factor | X.XX |

### Closed Trades
| Ticker | Entry | Exit | P&L | Notes |

### Open Positions at Week End
| Ticker | Entry | Close | Unrealized | Stop |

### What Worked
- ...

### What Didn't Work
- ...

### Key Lessons
- ...

### Adjustments for Next Week
- ...

### Overall Grade: X

## Week ending 2026-07-13

### Stats
| Metric | Value |
|--------|-------|
| Starting portfolio | $1,000,000.00 |
| Ending portfolio | $1,000,000.00 |
| Week return | $0 (0.00%) |
| S&P 500 week | +0.4% (week ending Jul 10) |
| Bot vs S&P | -0.4% |
| Trades | 0 (W:0 / L:0 / open:0) |
| Win rate | N/A |
| Best trade | N/A |
| Worst trade | N/A |
| Profit factor | N/A |

### Closed Trades
| Ticker | Entry | Exit | P&L | Notes |
| — | — | — | — | No trades — account created today, no trading history exists |

### Open Positions at Week End
| Ticker | Entry | Close | Unrealized | Stop |
| — | — | — | — | None |

### What Worked
- N/A — Alpaca account was created today (2026-07-13); zero trading days have elapsed

### What Didn't Work
- N/A — no trades taken yet, nothing to evaluate

### Key Lessons
- This "week" is not a real trading week: account inception (`created_at`) is 2026-07-13, same as today's run date
- Weekly review triggered before any pre-market/market-open runs populated TRADE-LOG.md or RESEARCH-LOG.md
- Flagging rather than fabricating a review — no fictional trades, P&L, or grade generated

### Adjustments for Next Week
- Confirm daily workflows (pre-market, market-open, midday, daily-summary) have run at least once before next Friday's review
- Re-run weekly review once real trading history exists

### Overall Grade: N/A (no data)

## Week ending 2026-08-21

**Scheduling gap flagged**: No pre-market/market-open/midday/daily-summary/weekly-review
entries exist between 2026-07-24 and today — a ~4-week gap (5 missed Fridays including this
review's own cadence). Figures below compare the last verified log state (2026-07-24) to
today's live Alpaca state; this is NOT a single trading week, and any activity inside the gap
that wasn't logged (see below) may be incomplete.

### Stats
| Metric | Value |
|--------|-------|
| Starting portfolio (last verified, 2026-07-24) | $1,009,303.99 |
| Ending portfolio (2026-08-21, live) | $1,016,271.99 |
| Period return (~4 weeks) | +$6,968.00 (+0.69%) |
| S&P 500 week (ending 8/21) | -1.4% (CNBC); FRED weekly series shows -1.9% |
| Bot vs S&P (this week only, directional) | Outperformed — position held through an index down-week |
| Trades | 0 new (still 1 open: XOM) |
| Win rate | N/A — no closed trades |
| Best trade | N/A |
| Worst trade | N/A |
| Profit factor | N/A |

### Closed Trades
| Ticker | Entry | Exit | P&L | Notes |
|---|---|---|---|---|
| — | — | — | — | No closed trades this period |

### Open Positions at Week End
| Ticker | Entry | Close | Unrealized | Stop |
|---|---|---|---|---|
| XOM | 800sh @ $144.77 | $165.11 | +$16,272.00 (+14.05%) | 7% GTC trailing (stop $156.8352, hwm $168.64) |

### What Worked
- XOM thesis kept paying off unattended — unrealized gain grew from +8.6% (7/24) to +14.05% (8/21) with zero manual intervention needed
- The 10%→7% trail-tighten rule (triggered near +15%) did fire on the account — stop is correctly positioned per strategy, protecting most of the gain
- Account survived a down week for the S&P (-1.4 to -1.9%) without giving back capital

### What Didn't Work
- **Critical: scheduled workflows did not run for ~4 weeks** (last commit/log entry 2026-07-24; today is 2026-08-21) — no pre-market research, no market-open/midday checks, no EOD snapshots, and this weekly review itself skipped ~5 Fridays (7/31, 8/7, 8/14, plus the original 7/17 gap)
- **Untracked live action found**: Alpaca order history shows the XOM trailing stop was canceled and replaced (10%→7%, new hwm $168.64) on 2026-08-19, with no corresponding RESEARCH-LOG/TRADE-LOG entry and no git commit anywhere in this repo (checked all branches) — the account was modified outside any logged/committed session
- Deployment still stuck at ~13% vs. the 75-85% target — now an extended, unmonitored stretch on top of the 6 sessions already flagged pre-gap
- Zero new trades taken in ~4 weeks despite a 3-trades/week allowance — no research was being generated to identify candidates
- No visibility into whether other decisions (skipped trades, missed catalysts) happened correctly during the blackout — the log simply isn't there

### Key Lessons
- A sound thesis on one position can carry P&L through an outage, but that is luck, not process — the bot was not actually managing risk or sourcing new ideas for a month
- An unlogged live stop change is a bigger red flag than a bad trade: it means the account can be touched with zero audit trail, which breaks the "never move a stop down / always log it" discipline this system depends on
- This is an infrastructure/scheduling problem, not a strategy problem — no rule in TRADING-STRATEGY.md needs to change based on what little data exists

### Adjustments for Next Week
- Operator should verify why the scheduled routines (pre-market, market-open, midday, daily-summary, weekly-review) stopped firing after 2026-07-24 — this needs to be fixed outside this repo (scheduler/cron config), not in memory files
- Once routines resume, do not backfill fabricated daily entries for the gap — log going forward and reference this review for the blackout period
- Re-evaluate the 75-85% deployment target given it's now been unmet for well over a month with no forcing function
- Confirm no other live orders/positions were changed during the gap beyond the one stop adjustment found here

### Overall Grade: C — position held up and the stop rule fired correctly, but the bot was effectively unsupervised for a month with one unlogged live order change; a scheduling failure of this length would have been much costlier with a less cooperative market
