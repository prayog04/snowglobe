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

## Week ending 2026-08-07

### Stats
| Metric | Value |
|--------|-------|
| Starting portfolio (Mon 8/3 AM) | **NOT LOGGED** — no market-open snapshot exists; see outage note below |
| Last verified snapshot pre-outage | $1,009,303.99 (2026-07-24 pre-market, RESEARCH-LOG) |
| Ending portfolio (2026-08-07 live) | $1,006,649.91 |
| Change since 7/24 (~10 trading days, not a clean week) | -$2,654.08 (-0.26%) |
| Phase P&L (since inception 7/13) | +$6,649.91 (+0.66%) |
| S&P 500 week (Aug 3-7) | +3.6% — best week since mid-April, record close Fri |
| Bot vs S&P 500 (this week) | Not computable — no Monday baseline for the bot |
| Trades this week | 0 (W:0 / L:0 / open:0 new) — 0/3 weekly allowance used |
| Win rate | N/A — zero closed trades since inception |
| Best trade | N/A (no closed trades) |
| Worst trade | N/A (no closed trades) |
| Profit factor | N/A (no closed trades) |

### Closed Trades
| Ticker | Entry | Exit | P&L | Notes |
| — | — | — | — | No closed trades since inception (2026-07-13) |

### Open Positions at Week End
| Ticker | Entry | Close | Unrealized | Stop |
|---|---|---|---|---|
| XOM | 800sh @ $144.77 | $153.08 | +$6,649.92 (+5.74%) | $143.16 GTC trailing 10% (hwm $159.07) |

### What Worked
- The GTC trailing stop is a real broker-side order — it kept working and kept the position protected through a 10-trading-day period with zero bot activity.
- No unauthorized or erroneous trades occurred during the outage — Alpaca order history shows exactly the two orders ever placed (7/15 buy, 7/15 trailing stop), nothing else.
- XOM thesis held up on its own — position still profitable (+5.74% unrealized) and phase P&L is still positive (+0.66%) despite total neglect for two weeks.

### What Didn't Work
- **CRITICAL: total scheduling outage.** No pre-market, market-open, midday, daily-summary, or weekly-review run produced any commit to `memory/` between 2026-07-24 and 2026-08-06 (confirmed via git log) — 10 straight trading days with zero research, zero monitoring, zero logging, zero ability to enforce the -7% manual cut-loss or trail-tightening rules if they'd been needed.
- This is not a new issue — it's an escalation. 7/20 and 7/24 entries already flagged shorter logging gaps (7/14-7/19, then 7/23) as "scheduled-workflow reliability" problems. Nothing was fixed between then and now; the gap simply got longer.
- Account sat at ~12% deployed (vs. 75-85% target) through the entire outage and missed nearly all of this week's 3.6% S&P 500 rally — cash sat idle while the market ran, with no bot present to act on it either way.
- The weekly-review process itself is not immune to the failure it's supposed to catch — this review only exists because a run finally fired today; nothing caught the gap while it was open.

### Key Lessons
- Broker-side GTC stops are the only safety net that survives a harness outage — that's exactly why Rule 4 (real GTC order, not a mental stop) matters, and it's the only reason this outage didn't cost real risk-management coverage.
- A flagged reliability gap that isn't fixed will recur and grow — this is the third consecutive review cycle to note a missing-runs problem, each one worse than the last.
- "Patience > activity" is a trading discipline, not an excuse for the scheduling layer to go quiet — those are two different failure modes and this week's grade reflects the latter, not the former.

### Adjustments for Next Week
- **Top priority, non-trading:** confirm the pre-market/market-open/midday/daily-summary schedule triggers are actually configured and firing (check `routines/` and whatever cron/scheduler drives this account) before trusting any future review's data.
- Once daily runs are confirmed live, re-underwrite XOM with current data (price has pulled back from the $159 hwm to $153) before deciding whether to hold, trim, or let the stop manage it.
- Resume normal cadence toward the 75-85% deployment target — the account has effectively been a single-position book for over three weeks now.
- Next Friday's review should explicitly confirm all five scheduled runs fired this week before computing any performance numbers.

### Overall Grade: D — capital preservation held (thanks to the GTC stop and a thesis that happened to stay intact), but this was a full operational outage, not a trading week. Grade reflects the process failure, not the P&L.
