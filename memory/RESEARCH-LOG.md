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

## 2026-07-13 — Pre-market Research

### Account
- Equity: $1,000,000
- Cash: $1,000,000 (100%)
- Buying power: $4,000,000 (margin, unused)
- Daytrade count: 0
- No open positions, no open orders (Day 1 — fresh launch)

### Market Context
- WTI: ~$71.41 (-0.93%) / Brent: ~$76.01 (-0.38%), off recent highs but elevated on U.S.-Iran tension (Strait of Hormuz risk premium, Brent briefly spiked toward $77-79)
- S&P 500 futures: ~7,594 (-0.34%), "taking a breather" after last week's gains
- VIX: 15.03 (Fri close) — low/complacent, but geopolitical tail risk (Iran) not fully priced
- Today's catalysts: Treasury Budget release; Q2 earnings season kicks off (big banks GS/JPM/WFC report Tue); SK Hynix US debut +14% (AI-chip demand strong); Iran ceasefire breakdown driving oil bid
- Earnings before open today: none major (FBK, small-caps only per Nasdaq calendar)
- Economic calendar: no CPI/PPI/FOMC/jobs today — June CPI prints tomorrow (7/14, consensus ~4.2% y/y), a likely volatility catalyst
- Sector momentum: rotation into defensives/cyclicals — Consumer Staples, Industrials, Materials, Energy leading; Real Estate/Utilities improving; Healthcare weakening; Tech/Comms/Discretionary/Financials lagging despite YTD gains

### Trade Ideas (watchlist only — not acted on)
1. XLE / energy majors — catalyst: Iran-driven oil spike + sector momentum leadership; wait for pullback entry, stop ~7-8% below entry, target 2:1 R:R. Needs live quote confirmation (data feed down, see Risk Factors).
2. XLI or select industrials — catalyst: momentum leadership + no single-name earnings risk this week. Same entry/stop framework pending quote access.
3. Defer bank exposure (JPM/GS/WFC) until after Tue earnings print — avoid entering into binary event.

### Risk Factors
- Day 1 launch — no track record, no calibration on execution yet
- CPI print tomorrow (7/14) — high-vol catalyst, avoid sizing up into it
- Iran/Strait of Hormuz headline risk — oil and broad market gap risk both ways
- Alpaca market-data quote endpoint (data.alpaca.markets) blocked at network/proxy level (403 CONNECT tunnel, "policy denial") for all tickers — trading API (paper-api.alpaca.markets) unaffected. Could not confirm live entry prices; needs infra fix (proxy allowlist) before any live order can be sized
- Big bank earnings Tue — sector-wide financials volatility

### Decision
HOLD — Day 1, no positions to manage, CPI print tomorrow argues for patience. Quote data feed also needs to be fixed before any order can be sized/placed. Will revisit post-CPI with live pricing restored.
