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

---

## ⚠️ LOGGING GAP: 2026-07-24 → 2026-09-14 (~7.5 weeks, no scheduled runs committed)

No market-open/midday/EOD/research entries exist for this entire stretch, yet Alpaca order history shows the account kept trading correctly per the strategy rules. Backfilled below from live Alpaca order history during the 2026-09-14 midday scan. **This is a third and far more severe instance of the reliability gap first flagged 2026-07-20 and 2026-07-24** — scheduled workflows stopped committing to this repo for weeks while real (paper) trades executed with zero documented thesis or review.

### Aug 19 — Trail tightened 10% → 7% (backfilled 2026-09-14)
| Ticker | Action | Trigger | Old Stop | New Stop |
|---|---|---|---|---|
| XOM | Tighten trail | Position hit +15.2% unrealized (hwm $166.74 vs $144.77 entry) | 10% trailing (hwm $166.74, stop ~$150.07) | 7% trailing (order e3db5144, hwm growing from $166.74) |

**Note:** Correctly executed per Rule 6 (tighten to 7% at +15%). No corresponding RESEARCH-LOG or TRADE-LOG entry exists — discovered only via Alpaca order history (original 10% order `c8388a7a` canceled 2026-08-19T13:39:15Z, replacement 7% order `e3db5144` submitted same second).

### Aug 27 — SELL (stopped out) (backfilled 2026-09-14)
| Ticker | Side | Shares | Entry | Exit | Realized P&L | Reason |
|---|---|---|---|---|---|---|
| XOM | Sell (trailing stop fill) | 800 | $144.77 | $156.81 | +$9,632.00 (+8.31%) | 7% GTC trailing stop triggered (hwm $168.64 → stop $156.8352, filled $156.81) |

**Note:** Full close of the original Jul 15 position via the tightened trailing stop — a clean, profitable exit per the mechanical stop rule, working exactly as designed. Never logged. Position sat flat (0 holdings) from 2026-08-27 to 2026-09-01.

### Sep 1 — BUY (backfilled 2026-09-14)
| Ticker | Side | Shares | Entry | Stop | Thesis | Target | R:R |
|---|---|---|---|---|---|---|---|
| XOM | Buy | 1000 | $162.90998 | 10% GTC trailing (order `240c38d4`, stop set same session) | **UNDOCUMENTED — no RESEARCH-LOG entry exists for 8/28-9/1; catalyst/thesis unknown** | — | — |

**Note:** Re-entry into XOM after the Aug 27 stop-out, same day-of-week pattern (market buy + same-session GTC trailing stop) as the original Jul 15 entry, suggesting the scheduled market-open/pre-market workflow did run and execute the trade logic correctly — it just never committed its log/research output to this repo. **Flagged for operator: verify whether pre-market research actually ran for 9/1 (check ClickUp history / other storage) since no rationale is recoverable from git.**

### Sep 14 — Midday scan
No new action. Current state pulled live from Alpaca:
- **Position:** XOM, 1000 sh @ avg $162.90998, current $164.30, unrealized +$1,390.02 (+0.85%) — well inside all thresholds (no -7% cut, no +15%/+20% tighten; today's -1.02% intraday move is normal noise, not a thesis break)
- **Stop:** GTC trailing 10% live (order `240c38d4`, stop $152.505, hwm $169.45) — untouched, correctly below price with room
- **Account:** Equity $1,011,169.24 (+1.12% since launch), cash $846,719.24 (83.7%), deployed 16.3% (1 of 5-6 target positions) — under-deployed, consistent with the pre-gap pattern
- No losers to cut, no tighten trigger, no sharp/unexplained move warranting Perplexity research today.

**Action taken this session:** backfilled the entire Aug 19 – Sep 1 trade history above from Alpaca order history (see gap note). No live orders were placed or canceled by this session — informational backfill only.
