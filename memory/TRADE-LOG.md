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

### Aug 27 — STOP FILLED (backfilled 2026-09-02, see note)
| Ticker | Side | Shares | Fill Price | Trail | Realized P&L |
|---|---|---|---|---|---|
| XOM | Sell (trailing stop) | 800 | $156.81 | 7% GTC (hwm $168.64) | +$9,632.00 (+6.65% on the position) |

**Note:** GTC trailing stop filled live on Alpaca 2026-08-27 13:40 UTC, closing the original XOM position opened 7/15. Trail had tightened to 7% per the +15% profit rule as XOM ran past $168. This exit was never logged — no scheduled workflow ran between 7/24 and 9/1 (see EOD note below).

### Sep 01 — BUY (backfilled 2026-09-02, see note)
| Ticker | Side | Shares | Entry | Stop | Thesis | Target | R:R |
|---|---|---|---|---|---|---|---|
| XOM | Buy | 1000 | $162.90998 | 10% trailing GTC (stop $148.52, hwm $165.02 as of 9/1) | Not on file — no RESEARCH-LOG entry exists for this trade | — | — |

**Note:** Market buy filled live on Alpaca 2026-09-01 13:43 UTC, re-entering XOM after the 8/27 stop-out, with a 10% GTC trailing stop attached same session. No pre-market/market-open RESEARCH-LOG entry or TRADE-LOG entry exists for this decision — violates the "every trade documented before execution" rule in PROJECT-CONTEXT.md. Backfilled from live order history during the 2026-09-02 daily-summary run.

### Sep 02 — EOD Snapshot (Day 38, Wednesday)
**Portfolio:** $1,010,969.24 | **Cash:** $846,719.24 (83.8%) | **Day P&L:** -$300.00 (-0.03%) | **Phase P&L:** +$10,969.24 (+1.10%)

| Ticker | Shares | Entry | Close | Day Chg | Unrealized P&L | Stop |
|---|---|---|---|---|---|---|
| XOM | 1000 | $162.91 | $164.25 | -0.18% | +$1,340.02 (+0.82%) | $148.52 GTC trailing 10% (hwm $165.02) |

**Notes:** MAJOR LOGGING GAP: no scheduled workflow (pre-market/market-open/midday/daily-summary) committed anything to this repo between 2026-07-24 and 2026-09-01 — a full 5-week, ~25-trading-day blackout, the worst instance of the reliability issue flagged repeatedly in late July. Reconstructed from live Alpaca order history: the original 800sh XOM position (entry $144.77, opened 7/15) hit its 7% trailing stop on 8/27 at $156.81, realizing +$9,632 (+6.65%) — the trail-tightening rule worked as designed even with no bot supervision. The account then sat in cash until 9/1, when a fresh 1000sh XOM buy filled at $162.91 with a new 10% GTC trailing stop attached same session; no research rationale for this specific re-entry exists anywhere in RESEARCH-LOG.md, breaking the document-before-execution rule. Today (9/2) itself was quiet: no new trades, XOM basically flat (-0.18%), stop resting safely below at $148.52. Trades this week (since Mon 8/31): 1/3 (the 9/1 buy). Deployment is 16.2% vs. the 75-85% target. Flagging the multi-week outage as the top priority — the scheduled workflows must be confirmed running (and committing) before trusting this log again; consider a monitoring/alert on missed runs.
