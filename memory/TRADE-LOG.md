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

**LOGGING GAP: 2026-07-24 to 2026-08-27 — no scheduled workflow entries exist for this entire stretch (~24 trading days).** No RESEARCH-LOG or TRADE-LOG entries were written in that window. Alpaca order history shows two events that happened with zero log record: (1) on 2026-08-19 the XOM GTC trailing stop was replaced, tightening from 10% to 7% (hwm $166.74 → new stop basis), consistent with the strategy's "+15% tighten to 7%" rule but never logged; (2) on 2026-08-27 (today) that 7% trailing stop triggered and closed the full XOM position — see backfilled SELL record and EOD snapshot below. This is a serious reliability gap: scheduled runs were silent for over a month while the sole position ran up, got its stop correctly tightened, and then fully exited, none of it recorded until this run reconstructed it from live Alpaca data.

### Aug 19 — Stop tightened (backfilled from order history, entry was missing)
XOM GTC trailing stop replaced: 10% trail → 7% trail, high-water mark $166.74 at time of replacement (XOM +15.2% from $144.77 entry, crossing the strategy's +15% tighten trigger). No corresponding market-open/research entry exists for 2026-08-19; reconstructed from Alpaca closed-orders history during this 2026-08-27 EOD run.

### Aug 27 — SELL (stop-out, backfilled from order history)
| Ticker | Side | Shares | Fill Price | Entry | Realized P&L | Reason |
|---|---|---|---|---|---|---|
| XOM | Sell | 800 | $156.81 | $144.77 | +$9,632.00 (+8.32%) | 7% GTC trailing stop triggered intraday (hwm $168.64, tightened from 10%→7% on 2026-08-19) |

**Note:** Filled 2026-08-27 13:40 UTC during market hours. Position fully closed — account now 100% cash, zero open positions. XOM peaked at a $168.64 high-water mark (+16.5% from entry) before the 7% trail caught the pullback to $156.81, still locking in +8.32% on the full ~6-week hold. Stop mechanism worked exactly as designed; the failure here is purely a logging one (see gap note above), not a strategy or execution failure.

### Aug 27 — EOD Snapshot (Day 34, Thursday)
**Portfolio:** $1,009,631.99 | **Cash:** $1,009,631.99 (100%) | **Day P&L:** -$1,104.00 (-0.11%) | **Phase P&L:** +$9,631.99 (+0.96%)

| Ticker | Shares | Entry | Close | Day Chg | Unrealized P&L | Stop |
|---|---|---|---|---|---|---|
| — | — | — | — | — | — | — |

**Notes:** Account is fully flat — the sole position (XOM, held since Jul 15) was stopped out intraday today via its 7% GTC trailing stop at $156.81, closing 800 shares for a realized gain of +$9,632.00 (+8.32%) on the trade. Day P&L is slightly negative (-$1,104, -0.11%) purely from XOM giving back ground between yesterday's mark and today's stop-out price ahead of the sale; Phase P&L remains positive at +$9,632.00 (+0.96%) since launch, all of it from this one closed trade. Cash is 100% deployed to zero — 0 of 5-6 target positions, 0% deployed vs. the 75-85% target. No new trades today beyond the automatic stop-out (0/3 new-position trades used this week, Mon Aug 24-today). Flagging again for tomorrow: this run also surfaced and backfilled a ~24-trading-day logging gap (2026-07-24 to 2026-08-27) during which the stop was correctly tightened and then triggered with no log entries at all — see gap note above. Next session's clear priority: source 1-2 new candidates per the sector-momentum framework now that the account is fully in cash, and confirm scheduled workflows are actually firing daily going forward.
