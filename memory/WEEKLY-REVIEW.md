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

## Week ending 2026-09-11

### Stats
| Metric | Value |
|--------|-------|
| Starting portfolio | ~$1,006,189.24 (est., see note) |
| Ending portfolio | $1,012,709.24 |
| Week return | +$6,520.00 (+0.65%, est.) |
| S&P 500 week | -0.8% (holiday-shortened, Mon 9/7 closed for Labor Day) |
| Bot vs S&P | +1.45pp |
| Trades | 0 (W:0 / L:0 / open:1) |
| Win rate | N/A — no trades closed this week |
| Best trade | N/A this week (all-time: XOM +8.32%, closed 8/27) |
| Worst trade | N/A — no losing trades on record |
| Profit factor | N/A (1 all-time winner, $9,632.00; 0 losers) |

**Note on "Starting portfolio":** No Monday/Tuesday EOD snapshot exists in TRADE-LOG.md for this week (or for the prior ~7 weeks — see Data Gap below). Estimated by reconstructing week-start portfolio value from live cash ($846,719.24, unchanged all week per order history) plus 1,000 XOM shares at last Friday's (9/4) close of $159.47, sourced via Perplexity since the wrapper scripts expose no historical-bars endpoint. This is a reconstruction, not a logged fact — flagging rather than presenting it as precise.

### Closed Trades
| Ticker | Entry | Exit | P&L | Notes |
| — | — | — | — | No trades closed this week (Sep 8-11) |
| XOM (backfilled, not this week) | $144.77 (7/15) | $156.81 (8/27) | +$9,632.00 (+8.32%) | 7% trailing GTC stop fired at hwm $168.64. Never logged in TRADE-LOG.md — reconstructed from Alpaca closed-order history during this review. First closed trade in account history. |

### Open Positions at Week End
| Ticker | Entry | Close | Unrealized | Stop |
| XOM | 1,000 sh @ $162.91 (opened 9/1) | $165.99 | +$3,080.02 (+1.89%) | $150.63 GTC trailing 10% (hwm $167.37) |

### What Worked
- Trailing-stop mechanics fired exactly as designed: the original XOM position auto-tightened to a 7% trail near the +15% threshold and exited profitably (+8.32%, +$9,632.00) on 8/27 with no manual intervention needed
- Capital was redeployed same-session: XOM re-entered 1,000 sh @ $162.91 on 9/1, the day the stop filled — no extended idle-cash gap after the exit
- This week's est. return (+0.65%) beat the S&P 500's holiday-shortened week (-0.8%) by ~1.45pp
- Current stop (10% trail, $150.63) sits a healthy distance below market with room before the next tighten threshold

### What Didn't Work
- Severe logging gap: TRADE-LOG.md and RESEARCH-LOG.md have zero entries between 2026-07-24 and today (2026-09-11) — ~7 weeks, over 30 trading days — despite two real fills occurring in that window (8/27 stop-sell, 9/1 re-buy) that were never recorded
- No weekly review ran on any of the ~8 intervening Fridays; this is only the second WEEKLY-REVIEW.md entry in the account's 9-week life
- Deployment is ~16.4% of equity (1 of 5-6 target positions, $165,990 of $1,012,709) — still far under the 75-85% target, the same pattern flagged repeatedly pre-gap (6+ sessions in July) and apparently unresolved since
- This week's starting equity had to be reconstructed via an external price lookup rather than read from a system snapshot — an audit-trail gap, not just a cosmetic one

### Key Lessons
- Silent scheduling/logging failures are as costly as bad trades: 7 weeks of undocumented activity means the actual decisions behind the 8/27 exit and 9/1 re-entry can't be reviewed or learned from
- The trailing-stop rule engine is trustworthy on its own, but memory-file discipline around it (logging the fill, logging the reentry) failed independently of the trade logic
- Under-deployment has now persisted across both the pre-gap period (flagged repeatedly in July) and the post-gap period — the "wait for a dated catalyst" bar may be filtering out too much, or sourcing isn't happening at all during the gap

### Adjustments for Next Week
- Confirm pre-market/market-open/midday/daily-summary routines are actually running and logging on schedule now (last confirmed research entry before this review was 7/24)
- Explicitly flag any dated gap in TRADE-LOG.md/RESEARCH-LOG.md going forward rather than leaving it silent
- Actively source 1-2 new candidates against the sector-momentum framework — deployment has been stuck near 12-16% for the account's entire life
- New logging-integrity rule added to TRADING-STRATEGY.md (see below) in response to this failing badly across 7+ weeks

### Overall Grade: C — mechanically sound trading (stop discipline, profitable exit/reentry, beat S&P this week) undercut by a major operational failure: 7 weeks of undocumented trading activity and zero weekly reviews since inception.
