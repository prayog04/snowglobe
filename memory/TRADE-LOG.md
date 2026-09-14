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

### Sep 14 — Reliability Gap Note (backfilled from Alpaca order history)
No market-open, midday, pre-market, or EOD entries exist in TRADE-LOG.md or RESEARCH-LOG.md for any date between 2026-07-24 and 2026-09-14 — roughly 7 weeks / 33+ trading days where scheduled routines did not persist to this log, despite real trades executing on the live paper account in that window. Reconstructed from Alpaca's full order history during today's EOD run:

### Aug 27 — SELL (backfilled 2026-09-14, see note)
| Ticker | Side | Shares | Exit | Trigger | Realized P&L | Notes |
|---|---|---|---|---|---|---|
| XOM | Sell | 800 | $156.81 | 7% trailing stop (tightened from 10% on 8/19 at hwm $166.74, filled 8/27 off hwm $168.64) | +$9,632.00 (+8.32%) | Closed the 7/15 800sh position. No RESEARCH-LOG entry documents the 8/19 tighten action. |

### Sep 1 — BUY (backfilled 2026-09-14, see note)
| Ticker | Side | Shares | Entry | Stop | Thesis | Target | R:R |
|---|---|---|---|---|---|---|---|
| XOM | Buy | 1000 | $162.90998 | 10% trailing GTC (stop $152.505, hwm $169.45 as of 9/14) | **Undocumented** — no RESEARCH-LOG entry exists for this date | — | — |

**Note:** Between 7/24 and 9/1 the original XOM position (800sh @ $144.77) had its trailing stop tightened 10%→7% on 8/19 (consistent with the strategy's "+15% → tighten to 7%" rule, entry $144.77 vs. hwm $166.74 ≈ +15.2%), then stopped out on 8/27 at $156.81 for a realized gain of ~$9,632 (+8.3%). A brand-new 1000sh XOM position was opened 9/1 at $162.90998 (~16% of equity) with a fresh 10% GTC trailing stop — but **no pre-trade documentation exists** for this re-entry, violating the PROJECT-CONTEXT.md rule that "every trade must be documented BEFORE execution." No trades occurred 9/2 through 9/13; the only order activity in that stretch is the standing stop's high-water-mark updates. This is a scheduled-workflow reliability failure at least as severe as the 7/14-7/19 and 7/23 gaps already flagged — routines are either not firing or firing but failing before the commit/push step, since trades are clearly still reaching the account. **Flagging for operator review.**

### Sep 14 — EOD Snapshot (Day 45, Monday)
**Portfolio:** $1,011,809.14 | **Cash:** $846,719.24 (83.7%) | **Day P&L:** -$900.10 (-0.09%) | **Phase P&L:** +$11,809.14 (+1.18%)

| Ticker | Shares | Entry | Close | Day Chg | Unrealized P&L | Stop |
|---|---|---|---|---|---|---|
| XOM | 1000 | $162.90998 | $165.0899 | -0.54% | +$2,179.92 (+1.34%) | $152.505 GTC trailing 10% (hwm $169.45) |

**Notes:** First EOD snapshot since the ~7-week logging gap (see note above) — Day count resumes at Day 45 (45 trading days since 7/13 launch, excluding Labor Day 9/7). Current state per live Alpaca data only, since the log itself was stale: equity $1,011,809.14, up +$11,809.14 (+1.18%) cumulative since the $1,000,000 baseline. Today itself was quiet — no new orders, day P&L -$900.10 (-0.09%) purely from XOM's -0.54% intraday move off Friday's close. Single position (XOM, 1000sh) is only 16.3% deployed vs. the 75-85% target, continuing the long-running under-deployment pattern, though the deeper issue today is the audit-trail gap, not deployment. Trades today: none. Trades this week (new week starts today): 0/3. Next session should prioritize (1) diagnosing why scheduled routines stopped persisting for 7 weeks, and (2) backfilling a RESEARCH-LOG rationale for the undocumented 9/1 XOM re-entry.
