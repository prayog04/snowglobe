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

## Week ending 2026-09-04

### Stats
| Metric | Value |
|--------|-------|
| Starting portfolio | ~$1,009,629.22 (reconstructed — see note) |
| Ending portfolio | $1,006,189.24 |
| Week return | -$3,439.98 (-0.34%) |
| S&P 500 week | +0.5% (week ending Sep 4) |
| Bot vs S&P | -0.84% |
| Phase P&L (since 7/13) | +$6,189.24 (+0.62%) |
| Trades | 1 (W:0 / L:0 / open:1) |
| Win rate | N/A (no closes this week) |
| Best trade | N/A |
| Worst trade | N/A |
| Profit factor | N/A |

**Note on Starting portfolio:** No commit exists for Monday 8/31 open equity — reconstructed as current cash ($846,719.24) + current XOM cost basis ($162,909.98) = $1,009,629.22, which is what equity would have been all-cash after the 8/27 close, carried flat over the weekend into Monday's open (no trades 8/28-8/31 on file).

### Closed Trades
| Ticker | Entry | Exit | P&L | Notes |
| — | — | — | — | No closes this week. (Context, not this week: XOM 800sh entered 7/15 @ $144.77 was stopped out 8/27 @ $156.81 via the 7% tightened trail, +$9,632.00 / +8.32% — correct rule-6 behavior, but undocumented in TRADE-LOG/RESEARCH-LOG; see gap below.) |

### Open Positions at Week End
| Ticker | Entry | Close | Unrealized | Stop |
| XOM | $162.90998 (1000sh, bought 9/1) | $159.47 | -$3,439.98 (-2.11%) | $149.085 GTC trailing 10% (hwm $165.65) |

### What Worked
- Strategy mechanics fired correctly when active: the 10%→7% trail-tighten rule (rule 6) triggered on schedule as XOM crossed +15%, locking in +8.32% instead of round-tripping the gain
- Re-entered XOM 9/1 with a fresh 10% GTC trailing stop placed same-session — risk management on the new position is live and correctly configured
- Trades this week stayed within the 3/week cap (1 used)

### What Didn't Work
- **CRITICAL: zero git commits to this repo from 7/24 to 9/1 (5+ weeks).** Pre-market, market-open, midday, daily-summary, and at least 4 prior Friday weekly-reviews never landed, despite real fills executing on the live paper account in that window (8/19 stop-tighten, 8/27 stop-out, 9/1 re-entry) — the automation's audit trail went completely dark while the account kept trading
- No RESEARCH-LOG or TRADE-LOG entry exists for the 8/27 exit or the 9/1 re-entry — the catalyst/thesis for re-buying XOM at $162.91 (vs. the $156.81 it was just stopped out at) cannot be verified against the Entry Checklist
- This week marked negative (-0.34%) and trailed the S&P 500 (+0.5%) by 84bps
- Deployment is ~16% of equity (1 position) vs. the 75-85% target — consistent with the under-deployment pattern flagged in every prior logged session

### Key Lessons
- Correct trading rules and a dark audit trail are independent failure modes — a stop can fire perfectly while nobody (and no log) is watching
- Per CLAUDE.md, each session is a fresh clone: any scheduled run that fails at the commit/push step leaves zero trace, so a silent failure compounds for weeks before anyone notices — this is exactly what happened
- A re-entry after a stop-out is a new trade and needs its own documented catalyst check, not an assumption that the old thesis still holds

### Adjustments for Next Week
- Investigate why scheduled routines stopped committing after 7/24 and confirm pre-market/market-open/midday/daily-summary are firing and pushing again
- Backfill TRADE-LOG.md and RESEARCH-LOG.md for the 8/19 stop-tighten, 8/27 exit, and 9/1 re-entry from Alpaca order history (next market-open run)
- Add a heartbeat check so a scheduled run completing without a git commit gets flagged, not discovered weeks later
- Re-evaluate the 75-85% deployment target given the account has run under it for essentially every logged session to date

### Overall Grade: F — driven by the 5+ week loss of logging/oversight on a live-trading account, not by the trade mechanics themselves (which behaved correctly)
