# Research Log

Daily pre-market research entries will be appended here.
Format each entry:

## YYYY-MM-DD — Pre-market Research

### Account
- Equity: $X
- Cash: $X
- Buying power: $X
- Daytrade count: N

### Market Context
- WTI / Brent:
- S&P 500 futures:
- VIX:
- Today's catalysts:
- Earnings before open:
- Economic calendar:
- Sector momentum:

### Trade Ideas
1. TICKER — catalyst, entry $X, stop $X, target $X, R:R X:1
2. ...

### Risk Factors
- ...

### Decision
TRADE or HOLD (default HOLD if no edge)

## 2026-07-13 — Pre-market Research (run inline from market-open workflow)

### Account
- Equity: $1,000,000
- Cash: $1,000,000
- Buying power: $4,000,000
- Positions: none
- Daytrade count: 0

### Market Context
- WTI: ~$74.5/bbl (+4.3% d/d) | Brent: ~$79.1/bbl (+4.3% d/d) — surge on U.S.-Iran tensions, Strait of Hormuz shipping risk
- S&P 500 futures: ~-0.3% premarket
- VIX: ~15 (low), opened ~16.06
- Today's catalysts: US Treasury Budget release; no major pre-open earnings (JPM/WFC/GS/BAC/C report tomorrow 7/14); June CPI due 7/14
- Sector momentum: Energy leading YTD (+20-22%), Tech lagging (~-2%) — "Great Rotation" into cyclicals/defensives
- Trade ideas (energy momentum, catalyst = Iran/Hormuz-driven oil spike): XOM, CVX, OXY

### Risk Factors
- **Routine fired at 04:57 UTC (00:57 AM ET) — market does NOT open until 9:30 AM ET.** Alpaca quotes returned are stale Friday-close data with abnormal/illiquid bid-ask spreads (e.g. XOM bid $130.58 / ask $145.11), unusable for entry pricing.
- Energy trade is a crowded, already-run momentum play (oil already +4%+ on the news) — real entry price at actual open could gap well beyond a safe, non-chasing level.
- CPI print tomorrow (7/14) adds macro risk right after any new entry.

### Decision
HOLD — no orders placed. Market is closed; execution data is stale/unreliable. Flagging cron scheduling issue (routine ran ~8.5h before open) rather than trading on bad data. Re-evaluate XOM/CVX/OXY energy momentum thesis once live quotes are available at/after 9:30 AM ET.
