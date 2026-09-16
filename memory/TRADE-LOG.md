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

### Aug 19 — Stop tightened (backfilled 2026-09-16, see note)
XOM's 10% GTC trailing stop (from 7/15) was canceled and replaced with a 7% GTC trailing stop, consistent with the strategy's "tighten to 7% at +15%" rule. New stop: trail 7%, hwm $168.64 as of replacement.

**Note:** No research-log entry exists for 8/19; reconstructed from live Alpaca order history during the 2026-09-16 market-open run.

### Aug 27 — SELL, stop triggered (backfilled 2026-09-16, see note)
| Ticker | Side | Shares | Exit | Stop Type | Orig. Entry | Realized P&L | Hold Period |
|---|---|---|---|---|---|---|---|
| XOM | Sell | 800 | $156.81 | 7% GTC trailing stop (tightened 8/19 from 10%, hwm $168.64) | $144.77 (7/15) | +$9,632.00 (+8.32%) | ~6 weeks |

**Note:** Position fully closed when the 7% GTC trailing stop triggered and filled 2026-08-27 13:40 UTC — the stop mechanism worked as designed, no manual action taken (or needed) at the time. Backfilled from live Alpaca order history during the 2026-09-16 market-open run; see Risk Factors in RESEARCH-LOG 2026-09-16 for the logging-gap writeup.

### Sep 1 — BUY (backfilled 2026-09-16, see note)
| Ticker | Side | Shares | Entry | Stop | Thesis | Target | R:R |
|---|---|---|---|---|---|---|---|
| XOM | Buy | 1000 | $162.90998 | 10% trailing GTC (stop $152.676, hwm $169.64 as of 9/16) | Re-entry into Energy-sector leadership after the 8/27 stop-out; Energy remained #1 YTD sector | Not documented — no research-log entry exists for 9/1 | Not documented |

**Note:** Filled live 2026-09-01 13:43:59 UTC; 10% GTC trailing stop placed same session and still working correctly as of 9/16 (status "new", stop $152.676, hwm $169.64). No research-log rationale exists for this entry since no pre-market run occurred that day. Backfilled from live Alpaca order history during the 2026-09-16 market-open run.

### Sep 16 — Market-open check
No new trades. 1 open position (XOM, 1000 sh @ $162.90998 avg, current ~$165.89, +1.83% unrealized), 10% GTC trailing stop active (stop $152.676, hwm $169.64) — well below the +15%/+20% tighten thresholds, no stop action needed. Trades this week (since Mon 9/14): 0/3. Deployed: $165,890 / $1,012,609.24 equity = **16.4%** — still below the 75-85% target, 1 of 5-6 max positions. See RESEARCH-LOG 2026-09-16 for full context — HOLD decision; today's earnings slate (Lennar, LuxExperience, Aeluma, and other small-caps) has no name in our Energy/Materials/Staples momentum lane, and no fresh XOM/CVX-specific or Hormuz catalyst was found. **Flagging a major logging gap**: no RESEARCH-LOG or TRADE-LOG entries exist between 2026-07-24 and today (~8 weeks) despite real trading activity in that window (XOM stopped out 8/27 for a +8.32% gain, re-entered 9/1) — reconstructed and backfilled today from live Alpaca order history (see entries above).
