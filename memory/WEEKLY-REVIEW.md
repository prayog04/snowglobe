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

## Week ending 2026-08-28

**Note: this entry covers a 34-day gap, not one week.** No scheduled workflow (pre-market/market-open/midday/daily-summary/weekly-review) ran between 2026-07-25 and 2026-08-27 — confirmed via `git log`: zero commits to `memory/` in that span. "Starting portfolio" below is the last confirmed pre-gap figure (2026-07-24), not last Monday's.

### Stats
| Metric | Value |
|--------|-------|
| Starting portfolio | $1,009,303.99 (last confirmed, 2026-07-24) |
| Ending portfolio | $1,009,629.23 |
| Week return | +$325.24 (+0.03%) over 34 days (not 1 week) |
| S&P 500, same period (Jul 24→Aug 27 close) | +4.36% |
| S&P 500, standard week ending 8/28 alone | +0.7% |
| Bot vs S&P (full period) | -4.33% |
| Trades | 1 (W:1 / L:0 / open:0) |
| Win rate | 100% (1/1 closed) |
| Best trade | XOM +8.32% |
| Worst trade | XOM +8.32% (only trade) |
| Profit factor | N/A (no losing trades) |

### Closed Trades
| Ticker | Entry | Exit | P&L | Notes |
|---|---|---|---|---|
| XOM | $144.77 (7/15) | $156.81 (8/27) | +$9,632.00 (+8.32%) | Stopped out by its own GTC trailing stop (tightened 10%→7% around +15%, hwm $168.64) with zero oversight during the gap — see TRADE-LOG.md 8/27 backfill |

### Open Positions at Week End
| Ticker | Entry | Close | Unrealized | Stop |
|---|---|---|---|---|
| — | — | — | — | None — 100% cash, 0 positions |

### What Worked
- The GTC trailing stop functioned exactly as designed and protected a real gain on XOM even through a total 34-day oversight blackout — no bot or human touched the account and the position still closed as a winner
- The "tighten to 7% at +15%" rule engaged correctly (hwm $168.64 ≈ +16.5% from entry, consistent with the trigger)
- The only trade taken this period was a net winner; zero losing trades

### What Didn't Work
- **Critical:** zero scheduled workflow runs for 34 straight days (7/25-8/27) — no research, no logging, no live oversight of a ~$1M account
- Capital sat ~88-100% in cash the entire gap while the S&P rallied +4.36% — nearly all of that upside was forgone with no active decision behind it
- XOM ran to an unrealized peak of ~+16.5% (hwm $168.64) before giving back to +8.32% at the stop — no research entry ever existed to evaluate taking profit early, because nothing ran
- The 3-trades/week allowance sat completely unused for 5 straight weeks; no new candidates were ever sourced during the gap

### Key Lessons
- A real GTC stop order is a genuine safety net — it kept the book from ever going red even with the scheduler fully down
- This outage was invisible until this review manually cross-checked `git log` and live Alpaca order history — no one was alerted in real time
- Workflow health has no independent signal today; only a completed run produces evidence it happened, so a stalled scheduler fails silently

### Adjustments for Next Week
- Root-cause why pre-market/market-open/midday/daily-summary stopped firing after 2026-07-24 (check the cloud schedule config and `.claude/commands/`/`routines/` wiring) before resuming normal cadence
- Add a heartbeat/alert if an expected scheduled run doesn't fire in its window, so a multi-week silent outage can't recur
- Once runs are confirmed working again, resume normal research cadence — deployment (0% now) and the trades/week allowance have both sat unused for over a month
- Re-verify Alpaca order history at the next session start in case any other fill was missed by this backfill

### Overall Grade: D — the one trade taken was a winner, but a 34-day zero-oversight scheduling outage on a live-monitored $1M account is a process failure, not a performance one
