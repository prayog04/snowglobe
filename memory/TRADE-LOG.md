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

### Aug 27 — SELL (backfilled 2026-09-09, see note)
XOM 800 sh sold via 7% GTC trailing stop @ $156.81 (hwm $168.64), closing the Jul 15 entry (avg cost $144.77). Realized P&L: +$9,632.00 (+8.31%).

**Note:** This exit filled live on Alpaca (2026-08-27 13:40:14 UTC) via a trailing stop that was tightened from 10% to 7% on 2026-08-19, carrying forward the high-water mark from the original Jul 15 position. It was never committed to this log — no scheduled workflow (pre-market, market-open, midday, or EOD) appears to have run at all between 2026-07-24 and 2026-09-09, a 47-day gap. Backfilled from live Alpaca order history during the 2026-09-09 daily-summary run. No research-log rationale exists for the exit timing.

### Sep 01 — BUY (backfilled 2026-09-09, see note)
| Ticker | Side | Shares | Entry | Stop | Thesis | Target | R:R |
|---|---|---|---|---|---|---|---|
| XOM | Buy | 1000 | $162.90998 | 10% trailing GTC (stop $149.085, hwm $165.65 as of 9/9) | Unknown — no research-log entry exists for this trade | Unknown | Unknown |

**Note:** This entry filled live on Alpaca (2026-09-01 13:43:59 UTC) as a market buy, with a fresh 10% GTC trailing stop attached the same session. Same 47-day scheduled-workflow gap (2026-07-24 to 2026-09-09) as the Aug 27 exit above — no market-open, pre-market, midday, or EOD entries exist for that entire stretch despite live trading activity continuing on the account. No thesis, catalyst, or sizing rationale is on file for this trade. Backfilled from live Alpaca order history during the 2026-09-09 daily-summary run. **Flagging as a critical operational failure**: the account traded blind (no logged research, no dated catalyst check, no documented stop-tightening rule application) for over six weeks — the scheduled-run reliability gaps first noted 2026-07-20 and 2026-07-24 were never fixed and instead worsened into a full outage.

### Sep 09 — EOD Snapshot (Day 43, Wednesday)
**Portfolio:** $1,011,169.24 | **Cash:** $846,719.24 (83.7%) | **Day P&L:** +$3,790.00 (+0.38%) | **Phase P&L:** +$11,169.24 (+1.12%)

| Ticker | Shares | Entry | Close | Day Chg | Unrealized P&L | Stop |
|---|---|---|---|---|---|---|
| XOM | 1000 | $162.91 | $164.45 | +2.36% | +$1,540.02 (+0.95%) | $149.09 GTC trailing 10% (hwm $165.65) |

**Notes:** First scheduled run to execute since Jul 24 — a 47-day gap during which the bot kept trading live (via the standing GTC trailing stop and manual/unlogged decisions) but nothing was recorded. Backfilled two trades above: the Jul 15 XOM position was stopped out for a gain on Aug 27 (+8.31%, +$9,632 realized) when its trail tightened to 7% off a $168.64 high, then a new 1,000-share XOM position was opened Sep 1 at $162.91 with a fresh 10% GTC trailing stop — no research rationale is on file for that re-entry. No trades executed today; XOM closed $164.45 (+2.36% on the day), unrealized +$1,540 (+0.95%) against the Sep 1 cost basis, stop sitting at $149.09 off a $165.65 high. Portfolio equity $1,011,169.24, up $3,790 (+0.38%) vs. yesterday's $1,007,379.24 close and up $11,169.24 (+1.12%) cumulative since the $1,000,000 launch baseline. Deployment is 16.3% of equity — well under the 75-85% target — with only 1 of 5-6 target positions open. Trades this week (since Mon Sep 7): 0/3. Top priority before any new trade: diagnose why the scheduled workflows stopped firing for 47 days so this outage doesn't recur.
