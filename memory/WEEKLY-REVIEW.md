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

## Week ending 2026-07-17

### Stats
| Metric | Value |
|--------|-------|
| Starting portfolio | $1,000,000.00 |
| Ending portfolio | $1,002,536.47 |
| Week return | +$2,536.47 (+0.25%) |
| S&P 500 week | -0.5% (7,575.39 → 7,533.77) |
| Bot vs S&P | +0.75% |
| Trades | 1 (W:0 / L:0 / open:1) |
| Win rate | N/A — no closed trades |
| Best trade | N/A closed — XOM open +2.19% |
| Worst trade | N/A |
| Profit factor | N/A |

### Closed Trades
| Ticker | Entry | Exit | P&L | Notes |
| — | — | — | — | No closed trades this week |

### Open Positions at Week End
| Ticker | Entry | Close | Unrealized | Stop |
| XOM | $144.77 (800 sh, 7/15) | $147.94 | +$2,536.48 (+2.19%) | 10% trailing GTC, stop $135.00 (hwm $150) |

### What Worked
- XOM entry matched the Iran/Strait-of-Hormuz oil catalyst + Energy-sector-momentum thesis flagged in 7/13 pre-market research; position is profitable (+2.19% unrealized)
- Real 10% GTC trailing stop is live on XOM per rule 4 (stop $135, hwm $150)
- Trade frequency respected — 1 new position, well under the 3-trades/week cap

### What Didn't Work
- **Data integrity failure**: no commits to memory/TRADE-LOG.md or memory/RESEARCH-LOG.md since 2026-07-13, despite Alpaca showing a live XOM buy filled 2026-07-15. The XOM entry, its research rationale, and 4 days of market activity (7/14–7/17) have zero audit trail in memory — this review had to be reconstructed entirely from live `alpaca.sh account/positions/orders` output, not memory files
- Unknown whether pre-market/market-open/midday/daily-summary workflows ran at all on 7/14, 7/16, 7/17 — DAILY-SUMMARY.md's only entry is 7/13 (egress-blocked fallback)
- Massively under-deployed: 1 of 5-6 target positions, ~12% capital deployed vs the 75-85% target — the account sat mostly in cash all week
- Last week's review already flagged "confirm daily workflows have run" as an action item — it was not confirmed, and the underlying gap got worse instead of better

### Key Lessons
- Live order fills on Alpaca do NOT imply memory got written — every scheduled run must actually commit+push, or the trade becomes invisible to future reviews and to the strategy's own rules (sector-exit-after-2-losses, 3-trades/week cap, etc. all depend on TRADE-LOG.md being accurate)
- A silent gap in RESEARCH-LOG/TRADE-LOG entries is itself a signal and should trigger investigation, not just a note-and-move-on
- Weekly review must reconcile live Alpaca state against memory files, not trust memory files alone — this week that reconciliation caught a real, undocumented $115.8k position

### Adjustments for Next Week
- Root-cause why 7/14, 7/16, 7/17 workflow runs didn't produce memory commits (cron misfire vs. commit-step failure vs. runs not happening) before trusting any future daily log
- Backfill the missing 7/15 XOM entry into TRADE-LOG.md and RESEARCH-LOG.md so history going forward is accurate
- Source 2-4 more candidates to move toward the 5-6 position / 75-85% deployed targets
- Add a lightweight reconciliation check (live positions vs. TRADE-LOG.md) to the start of each daily workflow to catch drift immediately instead of a week later

### Overall Grade: C — the one trade made was sound and properly risk-managed, but the week's process reliability (memory logging) failed badly and needs to be fixed before results can be trusted
