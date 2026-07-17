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

### Jul 17 — Position Update (Friday)
**Portfolio:** $1,003,111.99 | **Cash:** $884,183.99 (88.1%) | **Day P&L:** +$2,168.00 (+0.22%) | **Phase P&L:** +$3,111.99 (+0.31%)

| Ticker | Shares | Entry | Close | Day Chg | Unrealized P&L | Stop |
|---|---|---|---|---|---|---|
| XOM | 800 | $144.77 | $148.66 | +1.86% | +$3,112.00 (+2.69%) | Trailing 10% GTC — stop $135.00 (hwm $150) |

**Notes:** Market-open run for 2026-07-17. **Backfill / data-integrity flag:** the XOM entry (800 sh @ $144.77, filled 2026-07-15 13:42 UTC, order id `31366dd1-7ad6-405b-9eea-68713cc3c771`) and its GTC 10% trailing stop (placed same day, order id `c8388a7a-30ab-466b-90fa-0576863e7635`) were executed by a prior session that never appears in this log or in RESEARCH-LOG.md — those files jump straight from 2026-07-13 to today with no committed record of the 7/14–7/16 decision, catalyst, target, or R:R. Confirmed via live Alpaca order history rather than repo memory; original thesis is not recoverable. No new trades placed today — broad risk-off tape (VIX 16.73, +6.76%; S&P futures -0.90%; AI/chip selloff) and no fresh documented catalyst; decision HOLD per RESEARCH-LOG 2026-07-17. 1 of 3 weekly trade slots used this week (XOM, Wed 7/15).
