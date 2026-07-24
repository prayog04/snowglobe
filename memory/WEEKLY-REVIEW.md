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

## Week ending 2026-07-24

### Stats
| Metric | Value |
|--------|-------|
| Starting portfolio | $1,002,071.99 (Fri 7/17 close, carried to Mon 7/20 open — see note) |
| Ending portfolio | $1,009,735.99 |
| Week return | +$7,664.00 (+0.76%) |
| S&P 500 week | -0.6% |
| Bot vs S&P | +1.36% |
| Trades | 0 (W:0 / L:0 / open:1) |
| Win rate | N/A — no closed trades |
| Best trade | N/A — no closed trades (XOM open, +$9,736 / +8.41% unrealized) |
| Worst trade | N/A — no closed trades |
| Profit factor | N/A — no closed trades |

**Note on starting portfolio:** No clean single "Monday AM" equity figure exists — two Jul 20 research-log entries show $1,001,943.99 and $1,002,015.99 (a ~$72 spread), and neither is clearly the true pre-open mark due to this cycle's logging gaps. Using Friday 7/17 close ($1,002,071.99, Alpaca `last_equity`), the same baseline the Jul 20 EOD snapshot used for its own day-P&L calc, as the most defensible week-start figure.

### Closed Trades
| Ticker | Entry | Exit | P&L | Notes |
| — | — | — | — | No closed trades this week |

### Open Positions at Week End
| Ticker | Entry | Close | Unrealized | Stop |
|---|---|---|---|---|
| XOM | $144.77 (800 sh, filled 7/15) | $156.94 | +$9,736 (+8.41%) | $142.71 GTC trailing 10% (hwm $158.57) |

### What Worked
- XOM (Energy, Strait of Hormuz/Iran risk-premium thesis) up +8.4% unrealized — the sector-momentum + dated-catalyst framework correctly identified the trade
- 10% GTC trailing stop ratcheted up automatically with price (hwm $158.57, stop $142.71) with zero manual intervention needed
- Discipline held against noise: did not chase the AI/semis pop (NVDA/AVGO) or the Fri 7/24 oil reversal — both stayed outside the Energy/Materials/Staples momentum lane
- Refused to force a trade on unreliable Perplexity data (7/24 AM: contradictory WTI/VIX prints, mismatched dates) rather than acting on bad inputs
- Portfolio beat the S&P 500 this week (+0.76% vs -0.6%), entirely carried by the single XOM position

### What Didn't Work
- Deployment stuck at ~12% vs. 75-85% target for 6 straight sessions; 0/3 weekly trade allowance used again — no second name ever cleared the "dated catalyst" bar
- Two scheduled-workflow logging gaps this cycle: 7/14-7/19 fully missing, and 7/23 market-open/research entry missing — XOM's entry had to be backfilled after the fact
- Research data quality degraded repeatedly (7/22 earnings calendar contradictory; 7/24 AM prices/VIX internally inconsistent) — blocked new-candidate evaluation on 2+ sessions
- Zero diversification — one Energy name is 100% of deployed capital; account is carrying most of its risk budget in cash, unused
- CVX earnings date was misread once (assumed 7/20, actually 7/31) before being caught — needs a cross-check step

### Key Lessons
- The entry checklist (specific catalyst + sector momentum + 2:1 R:R) is filtering correctly, but combined with genuine catalyst scarcity it's leaving the account chronically under-deployed — "patience > activity" is being honored almost too literally
- XOM diverging from oil itself (XOM up 7/24 while WTI/Brent reversed sharply lower) is a risk to watch, not yet a thesis break; the trailing stop is the built-in defense
- Scheduled-run reliability (missed premarket/market-open logs) is a distinct risk from strategy risk — incomplete audit trails undermine confidence in a trade's rationale even when the trade itself worked out

### Adjustments for Next Week
- Actively screen Materials and Consumer Staples (current #2/#3 YTD sectors) early in the week for a dated catalyst instead of defaulting to HOLD by inertia; use the 3-trade weekly allowance if a real catalyst appears
- Cross-verify Perplexity output against a second source (or live Alpaca quotes) before writing off a session's research as unreliable
- Confirm all 5 scheduled routines actually fired every day next week; investigate the 7/14-7/19 and 7/23 gaps
- Watch XOM for the +15% trail-tighten trigger (currently +8.4%, stop tightens to 7% at +15%)
- Revisit CVX as a possible second Energy name after its confirmed 7/31 earnings print

### Overall Grade: B-
Solid single-trade result and disciplined risk management, but 6 straight sessions at ~12% deployment (vs. 75-85% target) and two logging gaps are real process issues, not just bad luck.
