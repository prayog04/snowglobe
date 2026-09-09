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

### Aug 19 — Trail tightened (backfilled 2026-09-09, see note)
Original 10% GTC trailing stop (stop $150.07, hwm $166.74) canceled and replaced with a 7% GTC trailing stop, consistent with strategy rule "tighten trail to 7% at +15%" — entry $144.77, hwm $166.74 = +15.2% unrealized at time of tightening. No research-log entry documents this action.

### Aug 27 — SELL, stop-out (backfilled 2026-09-09, see note)
| Ticker | Side | Shares | Exit | Stop trigger | Thesis | Realized P&L |
|---|---|---|---|---|---|---|
| XOM | Sell (stop-out) | 800 | $156.81 | 7% GTC trailing stop, hwm $168.64 | Original 7/15 Hormuz/Energy-momentum thesis; trailing stop hit as XOM pulled back off its high | +$9,632.00 (+8.32% vs. $144.77 entry) |

**Note:** Filled live on Alpaca 2026-08-27 13:40 UTC (order created 8/19). Flat in XOM from 8/27 until the 9/1 re-entry below. Never logged here — no RESEARCH-LOG or TRADE-LOG entries exist for 7/25 through 8/31, a 5-week scheduled-workflow gap. Backfilled from Alpaca order history during the 2026-09-09 market-open run.

### Sep 1 — BUY, re-entry (backfilled 2026-09-09, see note)
| Ticker | Side | Shares | Entry | Stop | Thesis | Target | R:R |
|---|---|---|---|---|---|---|---|
| XOM | Buy | 1000 | $162.91 | 10% trailing GTC (stop $149.09, hwm $165.65 as of 9/9) | Re-entry into Energy-sector momentum (sector still #1 YTD, Brent/WTI elevated); no dated company-specific catalyst on file | not documented | not documented |

**Note:** Filled live on Alpaca 2026-09-01 13:43 UTC; 10% GTC trailing stop placed same session (correct per procedure). No research-log rationale exists for this trade — backfilled from Alpaca order history during the 2026-09-09 market-open run. This is a second, more severe instance of the audit-trail gap first flagged 2026-07-20/07-24: a full stop-out and a full re-entry both occurred with zero research or trade-log documentation, during a ~6-week stretch (7/25–9/8) with no market-open/research/EOD entries at all. Flagging as a scheduled-automation reliability failure, not a strategy failure — see notification.

### Sep 9 — Market-open check
No new trades. 1 open position (XOM, 1000 sh @ $162.91 avg), 10% GTC trailing stop active (stop $149.09, hwm $165.65), 16.3% of equity deployed. Trades this week (since Mon 9/7): 0/3. Inline pre-market research: Energy still #1 YTD sector (+24-36% depending on source), Brent ~$98-99 (elevated), VIX ~15.7-16.6 (moderate), Fed decision 9/16 (~56% odds of a 25bp hike per one source) is the next major macro catalyst — not today. No dated, company-specific catalyst found for a new name today. HOLD — existing thesis intact, stop correctly sized, no fresh catalyst clears the entry bar. See RESEARCH-LOG 2026-09-09 for full detail and the audit-trail gap writeup.
