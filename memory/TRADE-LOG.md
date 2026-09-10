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

### Aug 19 — Trail tightened (backfilled 2026-09-10, see note)
| Ticker | Action | Old Stop | New Stop | Trigger |
|---|---|---|---|---|
| XOM | Tighten trailing stop | 10% GTC (hwm $166.74) | 7% GTC (hwm $168.64) | Position hit +15.2% unrealized vs. $144.77 entry — per rule, tighten trail 10%→7% at +15% |

**Note:** No RESEARCH-LOG or TRADE-LOG entry exists for this action; reconstructed from Alpaca order history (old 10% trailing-stop order id `2b7b0c8a...` canceled 2026-08-19T13:39:15Z, replaced same session by a 7% trailing-stop order id `e3db5144...`, hwm $168.64). The tighten itself matches strategy rule 6 correctly — only the logging was missed.

### Aug 27 — SELL (backfilled 2026-09-10, see note)
| Ticker | Side | Shares | Exit | Realized P&L | Reason |
|---|---|---|---|---|---|
| XOM | Sell | 800 | $156.81 | +$9,624.00 (+8.32%) | 7% GTC trailing stop hit (hwm $168.64, stop $156.8352) — winning exit, stop did its job |

**Note:** Closes the original 7/15 XOM position (800sh @ $144.77) for a realized gain. No TRADE-LOG or RESEARCH-LOG entry exists for this exit; reconstructed from Alpaca order history (order id `e3db5144...`, filled 2026-08-27T13:40:14Z). Account sat fully in cash (XOM flat) from 8/27 until the 9/1 re-entry below.

### Sep 01 — BUY (backfilled 2026-09-10, see note)
| Ticker | Side | Shares | Entry | Stop | Thesis | Target | R:R |
|---|---|---|---|---|---|---|---|
| XOM | Buy | 1000 | $162.90998 | 10% trailing GTC (stop $150.633, hwm $167.37 as of 9/10) | **Not documented** — no pre-market/market-open research entry exists justifying this re-entry | — | — |

**Note:** Fresh XOM position (market buy, order id `2b7b0c8a-...`... — filled 2026-09-01T13:43:59Z), 10% GTC trailing stop attached same session (order id `240c38d4...`). Backfilled from live Alpaca order history during the 2026-09-10 midday scan — **no research-log or trade-log entry exists for 8/28 through 9/9 at all**, a ~6-week logging gap far larger than the earlier 7/14-7/19 and 7/23 gaps already flagged in this file. Rules were followed correctly on the account itself (tighten-at-+15%, stop-out, cash sit, re-entry) but none of it was recorded or reasoned about in these memory files — this scheduled workflow appears to not have run (or not committed) for over a month. Flagging as a high-priority reliability issue; re-entry thesis is unverified against current fundamentals/catalyst until a proper research entry is done.

### Sep 10 — Midday scan
No cut, no tighten, no new trade. 1 open position (XOM, 1000sh @ $162.90998), unrealized +1.65% ($2,685) — well below both the -7% cut threshold and the +15%/+20% tighten thresholds; existing 10% GTC trailing stop (stop $150.633, hwm $167.37) is already correct and left untouched (never move a stop down / never tighten within 3% of price — N/A here, no tighten triggered). No intraday thesis-breaking news encountered; XOM up modestly (+0.83%) with the broader tape, nothing sharp enough to warrant ad-hoc Perplexity research. Primary action this session was backfilling the Aug 19 / Aug 27 / Sep 1 activity above (see notes) — flagging the ~6-week memory-logging gap as the main finding of this run. See RESEARCH-LOG 2026-09-10 addendum.
