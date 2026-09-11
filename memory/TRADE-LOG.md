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

### Aug 27 — SELL, stop-out (backfilled 2026-09-11, see note)
| Ticker | Side | Shares | Exit | Stop Type | Realized P&L | Entry (Jul 15) | Hold |
|---|---|---|---|---|---|---|---|
| XOM | Sell | 800 | $156.81 | 7% trailing GTC triggered (hwm $168.64) | +$9,632.00 (+8.32%) | $144.77 | 43 days |

### Sep 1 — BUY (backfilled 2026-09-11, see note)
| Ticker | Side | Shares | Entry | Stop | Thesis | Target | R:R |
|---|---|---|---|---|---|---|---|
| XOM | Buy | 1000 | $162.90998 | 10% trailing GTC (stop $150.633, hwm $167.37 as of 9/11) | Not on file — no RESEARCH-LOG entry exists for 9/1; re-entry into existing Energy-sector thesis name after the 8/27 stop-out, same session also placed the 10% GTC trailing stop | Not on file | Not on file |

**Note — major logging gap:** No RESEARCH-LOG or TRADE-LOG entries exist between 2026-07-24 and 2026-09-11 (roughly 6-7 weeks / ~33 trading days). Reconstructed from live Alpaca order history during the 2026-09-11 market-open run:
- The original 800sh XOM position (entered 7/15 @ $144.77, 10% GTC trailing stop) had its stop replaced at some point with a tighter 7% trail (consistent with the strategy's "tighten to 7% at +15% gain" rule — position was then up double digits) — that 7% trailing stop triggered and filled 8/27 @ $156.81, closing the position for a realized +$9,632 (+8.32%) over a 43-day hold.
- A new 1000sh XOM position was opened 9/1 via market buy @ $162.90998, with a fresh 10% GTC trailing stop placed the same session (source: `access_key`, i.e. a scheduled/API session did run 9/1) — but neither the entry rationale nor the trade itself was ever written to RESEARCH-LOG or TRADE-LOG.
- No sessions appear to have logged anything (and possibly did not run) from 9/2 through 9/10.
- This is a more severe recurrence of the "logging gap" pattern already flagged on 7/20 and 7/24 — now spanning ~7 weeks and including one real, unlogged trade rather than just missed no-trade check-ins. Flagging for operator review; this session is proceeding with today's (9/11) market-open check using live Alpaca data as ground truth.

### Sep 11 — Market-open check
No new trades. 1 open position (XOM, 1000 sh @ $162.90998 avg), GTC trailing stop 10% active (stop $150.633, hwm $167.37), unrealized +$2,010.02 (+1.23%). Deployed $164,920 = 16.3% of $1,011,639.24 equity — well under the 75-85% target. Trades this week (since Mon 9/7): 0/3. See RESEARCH-LOG 2026-09-11 for full context — HOLD decision; no verified sector-momentum leaderboard or dated company-specific catalyst for a new name today, and today's US core CPI (Aug) print is still pending at time of this check, adding near-term macro uncertainty. Also see backfill note above (Aug 27/Sep 1) for the ~7-week logging gap discovered and reconstructed this session.
