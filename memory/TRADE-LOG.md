# Trade Log

## Day 0 — EOD Snapshot (pre-launch baseline)
**Portfolio:** $1,000,000.00 | **Cash:** $1,000,000.00 (100%) | **Day P&L:** $0 | **Phase P&L:** $0

No positions yet. Bot launches tomorrow.

### Jul 13 — EOD Snapshot (Day 1, Monday)
**Portfolio:** $1,000,000.00 | **Cash:** $1,000,000.00 (100%) | **Day P&L:** $0.00 (0.00%) | **Phase P&L:** $0.00 (0.00%)

| Ticker | Shares | Entry | Close | Day Chg | Unrealized P&L | Stop |
|---|---|---|---|---|---|---|
| — | — | — | — | — | — | — |

**Notes:** First trading day since launch. Account sat fully in cash with zero positions and zero orders — no trades executed today. Portfolio flat at $1,000,000, matching the pre-launch baseline exactly. No research or entries logged yet; next session should begin sourcing candidates per the strategy rulebook.

### Jul 20 — EOD Snapshot (Day 6, Monday)
**Portfolio:** $1,002,943.99 | **Cash:** $884,183.99 (88.2%) | **Day P&L:** +$872.00 (+0.09%) | **Phase P&L:** +$2,943.99 (+0.29%)

| Ticker | Shares | Entry | Close | Day Chg | Unrealized P&L | Stop |
|---|---|---|---|---|---|---|
| XOM | 800 | $144.77 | $148.45 | +0.74% | +$2,944.00 (+2.54%) | $135.00 GTC trailing 10% (hwm $150) |

**Notes:** Logging gap — this is the first EOD snapshot since Day 1 (Jul 13); no snapshots or research entries exist for Jul 14-17, and this routine appears not to have run over that stretch. Alpaca history shows one trade in that gap: XOM bought 800sh @ $144.77 on Jul 15 with a 10% GTC trailing stop attached same day, currently trailing at $135 off a $150 high. That trade has no corresponding research-log rationale on file. Today (Jul 20) had zero new orders. Day P&L computed from Alpaca's own last_equity ($1,002,071.99, Friday Jul 17 close) rather than the stale Jul 13 log line. Only 1 of 5-6 target positions open and ~12% deployed vs. the 75-85% target — well under-deployed for six trading days in. Trades this week: 0 (new week starts today).
### Jul 15 — BUY (backfilled 2026-07-20, see note)
| Ticker | Side | Shares | Entry | Stop | Thesis | Target | R:R |
|---|---|---|---|---|---|---|---|
| XOM | Buy | 800 | $144.77 | 10% trailing GTC (stop $135, hwm $150 as of 7/20) | Strait of Hormuz supply-risk premium on US-Iran tensions + Energy sector #1 YTD momentum; XOM guided Q2 net income ~3x Q1 | +16% (~$168) | ~2:1 |

**Note:** This trade filled live on Alpaca (2026-07-15 13:42 UTC) and its trailing stop was placed the same session, but neither was ever committed to this log — no market-open/pre-market entries exist for 7/14 through 7/19. Backfilled from live order history during the 2026-07-20 market-open run. Flagging as a scheduled-workflow reliability gap (see RESEARCH-LOG 2026-07-20).

### Jul 20 — Market-open check
No new trades. 1 open position (XOM), thesis intact, stop active. See RESEARCH-LOG 2026-07-20 for full context — HOLD decision, no dated catalyst for a new name.

### Jul 21 — Market-open check
No new trades. 1 open position (XOM), thesis intact, GTC trailing stop active (stop $135, hwm $150). Trades this week: 0/3. See RESEARCH-LOG 2026-07-21 for full context — HOLD decision, today's AI/semis rally is in the weakest YTD sector (Tech), not aligned with our Energy/Materials/Staples momentum framework; no dated catalyst clears the bar for a new name. Still under-deployed (11.9% vs 75-85% target) for a second straight session — flagged, not yet actionable.

### Jul 24 — Market-open check
No new trades. 1 open position (XOM), thesis intact, GTC trailing stop active (stop $142.71, hwm $158.57). Trades this week: 0/3. See RESEARCH-LOG 2026-07-24 for full context — HOLD decision; today's Perplexity research output was internally inconsistent/unreliable (oil and VIX prints spanning implausible ranges, mismatched dates), so no candidate could be verified against a real catalyst — not forcing a trade on bad data. XOM unrealized +8.59%, approaching (not yet at) the +15% trail-tighten threshold. Also note: no market-open or research entry exists for 7/23 — a second logging gap on top of the earlier 7/14-7/19 one.

### Jul 21 — EOD Snapshot (Day 7, Tuesday)
**Portfolio:** $1,005,623.99 | **Cash:** $884,183.99 (87.9%) | **Day P&L:** +$2,680.00 (+0.27%) | **Phase P&L:** +$5,623.99 (+0.56%)

| Ticker | Shares | Entry | Close | Day Chg | Unrealized P&L | Stop |
|---|---|---|---|---|---|---|
| XOM | 800 | $144.77 | $151.80 | +2.32% | +$5,624.00 (+4.86%) | $136.58 GTC trailing 10% (hwm $151.76) |

**Notes:** Quiet no-trade day, as previewed in the market-open check. XOM continued its run, up 2.3% intraday to $151.80, pushing the trailing stop's high-water mark to $151.76 and the stop itself up to $136.58 — the position is now up nearly 5% unrealized. Portfolio gained $2,680 (+0.27%) on the day, all from XOM's move; cash sat untouched at $884,184 (87.9%). Zero trades today, zero trades this week (0/3), and deployment remains stuck at ~12% vs. the 75-85% target for a third straight session — the bot continues to wait for a dated catalyst outside the weak Tech rally rather than force a trade.

### Aug 27 — SELL (backfilled 2026-09-11, see note)
| Ticker | Side | Shares | Fill | Stop Trigger | Realized P&L | R:R |
|---|---|---|---|---|---|---|
| XOM | Sell (trailing-stop exit) | 800 | $156.81 | 7% trail off hwm $168.64 | +$9,632.00 (+8.32%) | ~1.7:1 |

**Note:** Alpaca order history shows the original Jul 15 XOM position was exited via its trailing stop, filled 2026-08-27 13:40 UTC at $156.81 (stop had been tightened to 7% per strategy rule after the position crossed +15%, trailing a $168.64 high). This closes the Jul 15 trade for a realized gain of ~$9,632 (+8.32%). Backfilled from live order history — no scheduled run committed this to the log at the time.

### Sep 1 — BUY (backfilled 2026-09-11, see note)
| Ticker | Side | Shares | Entry | Stop | Thesis | Target | R:R |
|---|---|---|---|---|---|---|---|
| XOM | Buy | 1000 | $162.91 | 10% trailing GTC (stop $150.63, hwm $167.37 as of 9/11) | Not on file — no pre-market/market-open/research-log entry exists for 9/1 | n/a | n/a |

**Note:** Fresh XOM re-entry, filled 2026-09-01 13:43 UTC at $162.90998 (market order, 1000 sh), with a new 10% GTC trailing stop attached the same session. Backfilled from live order history during this 2026-09-11 EOD run.

### Sep 11 — SCHEDULED-RUN RELIABILITY GAP (flagged during EOD reconciliation)
**No memory-file activity (TRADE-LOG, RESEARCH-LOG, or any scheduled-run commit) exists between the last logged entry on 2026-07-24 and today, 2026-09-11 — a 7-week gap.** During that window Alpaca live order history shows a full round-trip that was never logged: the Jul 15 XOM position was stopped out on 2026-08-27 (+8.32% realized) and a new 1000-share XOM position was opened on 2026-09-01 at $162.91 with a fresh 10% trailing stop, still open today. Neither the exit, the re-entry thesis, nor ~44 trading days of pre-market/market-open/midday checks were committed to this repo. This is the same class of failure flagged on 2026-07-20 and 2026-07-24 (scheduled workflows not running or not persisting), now recurring at much larger scale — operator should verify the scheduling/commit pipeline for the pre-market, market-open, and midday routines.

### Sep 11 — EOD Snapshot (Day 44, Friday)
**Portfolio:** $1,012,859.24 | **Cash:** $846,719.24 (83.6%) | **Day P&L:** +$910.00 (+0.09%) | **Phase P&L:** +$12,859.24 (+1.29%)

| Ticker | Shares | Entry | Close | Day Chg | Unrealized P&L | Stop |
|---|---|---|---|---|---|---|
| XOM | 1000 | $162.91 | $166.14 | +0.55% | +$3,230.02 (+1.98%) | $150.63 GTC trailing 10% (hwm $167.37) |

**Notes:** Day P&L computed from Alpaca's own last_equity ($1,011,949.24, balance as of 9/10) since the log's last real snapshot predates today by 7 weeks — see the reliability-gap entry above. No trades today; the sole open order is the existing GTC trailing stop on the 1000-share XOM position (unchanged status, hwm $167.37, stop $150.63). Trades this week (Mon 9/7-today): 0/3. Portfolio sits at 16.4% deployed vs. the 75-85% target, well under target — consistent with the pattern already flagged before the gap, now compounded by seven weeks with no fresh research or candidate sourcing on file. Priority for the next session: confirm scheduled runs are executing and committing again, and resume active research given the prolonged under-deployment.
