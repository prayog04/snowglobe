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

### Aug 19 — STOP TIGHTENED (backfilled 2026-09-01, see note)
Original 10% GTC trailing stop on XOM canceled and replaced with a 7% GTC trailing stop (per strategy rule: tighten to 7% at +15% unrealized). New stop: trail_percent 7%, hwm $166.74 at replacement time.

### Aug 27 — SELL, stop-out (backfilled 2026-09-01, see note)
| Ticker | Side | Shares | Exit | Stop that triggered | Entry | P&L | R:R realized |
|---|---|---|---|---|---|---|---|
| XOM | Sell (trailing stop fill) | 800 | $156.81 | 7% trailing, hwm $168.64 | $144.77 | +$9,632.00 (+8.32%) | ~0.83:1 of 2:1 target (target was ~$168; stop triggered on pullback from hwm $168.64 before target could be confirmed as held) |

**Note (logging-gap backfill):** No market-open/research entries exist for 2026-07-25 through 2026-08-31 — a five-week scheduled-workflow gap, the third and by far the largest documented so far (prior gaps: 7/14-7/19, 7/23). During this gap, live Alpaca history shows: (1) the original 10% trailing stop was replaced with a 7% trailing stop on 8/19 (consistent with the strategy's +15%-unrealized tighten rule, implying XOM crossed +15% sometime in early-to-mid August without a logged research entry), and (2) that 7% stop filled on 8/27 at $156.81 (hwm $168.64), closing the position for a realized gain of $9,632 (+8.32% on cost, +6.28% off the $168.64 high). Since the 8/27 exit through 2026-08-31, the account sat 100% in cash (0 positions, 0 open orders) for a full week+ with zero trades — a real, not just logged, deployment gap, since equity had been sitting idle even though the 75-85%-deployed target was never met. Backfilled from live Alpaca order history (`orders?status=closed`) during the 2026-09-01 market-open run. Equity as of 2026-09-01 pre-market: $1,009,629.23 (cash), up $9,629.23 from the $1,000,000 baseline — entirely attributable to the XOM round trip; no other activity occurred in the gap.

### Sep 1 — BUY
| Ticker | Side | Shares | Entry | Stop | Thesis | Target | R:R |
|---|---|---|---|---|---|---|---|
| XOM | Buy | 1000 | $162.91 | 10% trailing GTC (stop $146.53, hwm $162.81) | Fresh (dated today) US-Iran military escalation reigniting Strait of Hormuz supply-disruption risk; WTI ~$86.5 (+2.7%+), Brent ~$91, both up sharply on the day; XOM/energy equities rallying alongside crude. Same thesis structure as the profitable Jul 15-Aug 27 XOM round trip. | +16% (~$189) | ~2:1 |

**Notes:** First trade in 5 weeks — account had been 100% cash since the Aug 27 stop-out. Position sized at 1000sh / ~$162,910 = ~16.1% of $1,009,629 equity, under the 20% cap. Rules checked: 1 position open (≤6 ✓), 1 trade this week (≤3 ✓), 16.1% ≤ 20% ✓, catalyst dated today in RESEARCH-LOG ✓, no PDT restriction on this account. See RESEARCH-LOG 2026-09-01 for full research. Flagging again: the 5-week logging gap (7/25-8/31) also represents 5 weeks of real, not just logged, under-deployment — worth a process check on why the scheduled workflow stopped running/persisting.
