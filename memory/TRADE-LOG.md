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

### Aug 19 — Stop tightened (backfilled 2026-09-09)
Canceled the 10% GTC trailing stop on the original XOM 800sh @ $144.77 position (hwm $166.74, stop $150.07 at cancellation — position was ~+15.1% unrealized) and replaced it with a 7% trail per the "+15% -> tighten to 7%" rule. Never committed to this log when executed; discovered today (9/9) while reconciling live Alpaca order history against this log during the midday scan.

### Aug 27 — SELL (stop-out, backfilled 2026-09-09)
| Ticker | Side | Shares | Exit | Realized P&L | Reason |
|---|---|---|---|---|---|
| XOM | Sell | 800 | $156.81 | +$9,632.00 (+8.32%) | 7% GTC trailing stop triggered off a $168.64 high-water mark — full exit of the 7/15 position |

**Note:** Filled 2026-08-27 13:40 UTC, never logged. Closed out the original XOM position (opened 7/15/26 @ $144.77) for a realized gain of +8.32% ($9,632) — a clean, rules-following exit (trail tightened 8/19 per the +15% rule, then triggered on a pullback). No corresponding log entry existed until this backfill.

### Sep 1 — BUY (backfilled 2026-09-09)
| Ticker | Side | Shares | Entry | Stop | Thesis | Target | R:R |
|---|---|---|---|---|---|---|---|
| XOM | Buy | 1000 | $162.90998 | 10% trailing GTC (stop $149.09, hwm $165.65 as of 9/9) | **UNKNOWN — no RESEARCH-LOG or TRADE-LOG entry exists for this entry.** No pre-market/market-open research on file supporting this re-entry. | — | — |

**Note:** Filled 2026-09-01 13:43 UTC with a 10% GTC trailing stop placed the same session; neither the trade nor any supporting research was ever logged. This is on top of two prior scheduled-workflow logging gaps already flagged in this log (7/14-7/19, and 7/23) — the gap this time spans **Jul 24 through Sep 9 (~7 weeks)** with zero RESEARCH-LOG or TRADE-LOG entries despite live trading activity (a stop-tighten, a full exit, and a new entry all occurred in that window). Operator should verify whether scheduled runs have been firing since 7/24, and what catalyst justified this 9/1 re-entry — no documented thesis exists to evaluate the current position against.

### Sep 9 — Midday check
No new trades this session. 1 open position (XOM, 1000sh @ $162.91 avg), current $164.90, unrealized +1.22% (intraday +2.64%) — well above the -7% cut threshold and well below the +15%/+20% tighten thresholds; 10% GTC trailing stop active and untouched (stop $149.09, hwm $165.65). No thesis-breaking news evaluated — no documented thesis exists to check against (see 9/1 backfill note above). Deployed capital ~16.3% ($164,870 of $1,011,589.24 equity) — still below the 75-85% target. No trading action taken today; no ClickUp alert sent per the Step 7 action-only rule. Flagging the 7-week logging gap and the undocumented 9/1 re-entry directly to the operator instead of via ClickUp.
