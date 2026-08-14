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

## Week ending 2026-08-14

**Data-gap flag:** TRADE-LOG.md and RESEARCH-LOG.md have no entries between 2026-07-24 and this run — a 3-week silent gap (no pre-market/market-open/midday/daily-summary logging). No weekly review was produced for weeks ending 7/17, 7/24, 7/31, or 8/7 either — this is the first review since the 7/13 placeholder. There is no Monday-AM (8/10) equity logged and the wrapper exposes no portfolio-history endpoint, so a true single-week return cannot be computed. Numbers below bracket the full gap (7/24 → 8/14, ~21 days) instead of fabricating a week-1 baseline. Flagging, not guessing.

### Stats
| Metric | Value |
|--------|-------|
| Starting portfolio | $1,009,303.99 (last logged equity, 2026-07-24 pre-market — no Mon 8/10 figure exists) |
| Ending portfolio | $1,012,263.99 |
| Period return (7/24→8/14, ~21 days) | +$2,960.00 (+0.29%) |
| S&P 500, same period | +5.36% (7,411.98 → ~7,808.87) |
| S&P 500, trailing week only (8/10-8/14) | +0.4% to +0.5% (3rd straight winning week) |
| Bot vs S&P (period) | -5.07 pp |
| Trades | 0 new (W:0 / L:0 / open:1 — XOM, opened 7/15, predates this period) |
| Win rate | N/A — no trade has ever closed since account inception |
| Best trade | N/A |
| Worst trade | N/A |
| Profit factor | N/A |

### Closed Trades
| Ticker | Entry | Exit | P&L | Notes |
| — | — | — | — | None — the only trade ever taken (XOM, 7/15) is still open |

### Open Positions at Week End
| Ticker | Entry | Close | Unrealized | Stop |
| XOM | $144.77 (800sh, 7/15) | $160.10 | +$12,264.00 (+10.59%) | $145.50 GTC trailing 10% (hwm $161.67) |

### What Worked
- XOM position stayed solidly profitable, +10.59% unrealized (entry $144.77 → $160.10)
- GTC 10% trailing stop kept ratcheting up correctly on its own (hwm now $161.67, stop $145.50) — the automated protection worked even while logging didn't
- Zero losing trades — no capital impaired, ever, since account inception

### What Didn't Work
- Zero new trades for 3+ consecutive weeks (0/3 weekly allowance used every week) while the S&P 500 rallied +5.36% — chronic under-deployment (~12-13% vs. 75-85% target) turned into a large, real opportunity cost, not just a paper concern
- Scheduled daily workflows show no logged activity 7/24 → 8/13 — either automation stopped firing or stopped writing to memory; either way it's a reliability failure, not a strategy one
- No weekly review fired for 4 straight Fridays (7/17, 7/24, 7/31, 8/7) — the one mechanism designed to catch exactly this kind of drift never ran
- Still a single-name, single-sector (Energy) book after a full month — no progress toward the 5-6 position diversification target

### Key Lessons
- "Patience > activity" was meant to mean waiting for a dated catalyst, not going dark — an account that logs nothing for three weeks isn't being disciplined, it's unmonitored
- Under-deployment during a strong rally (S&P +5.36% in 3 weeks) is now the single biggest drag on returns this account has produced — bigger than any per-trade risk taken to date
- Logging gaps compound: once TRADE-LOG/RESEARCH-LOG go dark, later reviews can't reconstruct what happened or why, which is exactly when a review is needed most

### Adjustments for Next Week
- Priority one: confirm pre-market/market-open/midday/daily-summary routines are actually firing on schedule before anything else — this is the root blocker, not a strategy fix
- Once confirmed running, prioritize screening 1-2 new positions to close the deployment gap, using the existing 3-trades/week allowance
- Keep XOM's trailing stop as-is (10%, hwm $161.67) — unrealized +10.59% is still under the +15% tighten trigger, no action needed
- No TRADING-STRATEGY.md rule change this week — the failure is operational (workflow reliability), not a bad rule; not touching the rulebook over a logging gap

### Overall Grade: D — capital was protected and the one position performed well, but a month of near-total inactivity during a market rally, compounded by a 3-week blackout in the bot's own logging and reviews, is a real cost, not a neutral outcome.
