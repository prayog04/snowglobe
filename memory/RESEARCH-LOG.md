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

## 2026-07-20 — Pre-market Research (run inline during market-open; entry was missing)

### Account
- Equity: $1,001,943.99
- Cash: $884,183.99
- Buying power: $3,866,463.96 (margin)
- Positions: 1 (XOM, 800 sh)
- Daytrade count: not reported by API today (no day trades taken)

### Market Context
- WTI ~$82-84, Brent ~$88-90 — elevated on renewed US-Iran/Strait of Hormuz tension after a brief ceasefire-talk lull
- S&P 500 futures: roughly flat/mixed (~7,478-7,497), testing the 7,500 handle after Friday's (7/17) options-expiration selloff to monthly lows
- VIX: ~18.3-18.8, up from 16.7 last Thu (7/16) — vol creeping higher
- Today's catalysts: AI-capex anxiety weighing on Nasdaq; newly hawkish Fed (Chair Kevin Warsh) ahead of July 28-29 FOMC; Q2 earnings season ramping (JNJ, DPZ, AMC pre-open; JPM, TSLA, LUV after close)
- Earnings before open: JNJ, DPZ, Dynex Capital, AMC, STLD, WRB, CCK
- Economic calendar: none major today (CPI/PPI already out last week); Leading Indicators (June) 10am ET; next big prints: jobs report Fri 7/25, FOMC decision 7/29
- Sector momentum: Energy #1 YTD (+24.6%, though slowing as oil chops), Technology #2 (+20.6%, cooling on AI-capex doubts), Industrials/Materials/Staples broadening leadership

### Trade Ideas
1. XOM (existing position) — thesis intact: Hormuz supply-risk premium back in oil, XOM guided Q2 net income $15.7-15.9B (~3x Q1). No new entry needed.
2. No new names screened with a fresh, dated catalyst today — Energy momentum is real but decelerating, and VIX ticking up into a FOMC-adjacent week argues for caution over chasing.

### Risk Factors
- **Audit-trail gap**: XOM buy (800 sh @ $144.77, filled 2026-07-15) and its GTC trailing stop were placed live but never logged to TRADE-LOG.md/RESEARCH-LOG.md, and no research/market-open/midday/daily-summary entries exist for 7/14 through 7/19. Backfilled the trade entry today; treating this as a scheduled-workflow reliability issue to flag, not a strategy issue — see notification.
- VIX rising into FOMC (7/28-29) — don't add fresh risk into a volatility uptick without a dated catalyst
- Oil/Hormuz headline risk cuts both ways for XOM — de-escalation would remove the premium fast
- Friday's (7/17) expiration-day selloff pushed futures to monthly lows — session could open soft

### Decision
HOLD — no new trades today. Existing XOM position (11.6% of equity) has an intact thesis and an active 10% GTC trailing stop (stop $135, hwm $150). No fresh, dated catalyst clears the bar for a new name; patience > activity, especially heading into a FOMC week with VIX drifting up.

## 2026-07-13 — Pre-market Research

### Account
- Equity: $1,000,000
- Cash: $1,000,000
- Buying power: $4,000,000 (margin, unused — 0 positions)
- Daytrade count: 0

### Market Context
- WTI / Brent: WTI $71.41 (-0.9%); Brent ~$76-79, up on US-Iran tensions / Strait of Hormuz risk
- S&P 500 futures: ~7,594, -0.34%
- VIX: 15.03 (calm, low vol)
- Today's catalysts: US-Iran tension flare pushing oil up 6-7% this week; Treasury Budget release; Q2 earnings season kicks off next week (big banks report Tue); SK Hynix IPO debut +14%; July FOMC hike odds jumped to 31% (from 17%), Sept to 84%, on oil-driven inflation fears
- Earnings before open: nothing major confirmed; FB Financial (FBK, regional bank) reporting
- Economic calendar: no CPI/PPI/FOMC/jobs today. June CPI prints tomorrow (Tue 7/14, 8:30am ET), consensus 3.8% YoY vs 4.2% prior — key catalyst
- Sector momentum: Energy + Consumer Staples leading YTD (defensive/inflation-hedge rotation); Tech/Comm Services/Discretionary/Financials lagging; Healthcare weakening; Real Estate/Utilities improving

### Trade Ideas
1. XOM — catalyst: Iran/Strait of Hormuz oil spike + Energy sector YTD leadership, entry ~market, stop -8%, target +16%, R:R 2:1 (WAIT for CPI print first)
2. CVX — same Energy-momentum catalyst as XOM, entry ~market, stop -8%, target +16%, R:R 2:1 (WAIT for CPI print first)
3. PG or KO — Consumer Staples flight-to-safety/inflation-hedge rotation, entry ~market, stop -7%, target +14%, R:R 2:1 (WAIT for CPI print first)

### Risk Factors
- June CPI prints tomorrow (7/14) — major volatility event, could reverse sector rotation fast
- Iran/oil headline risk cuts both ways — de-escalation would slam Energy longs
- Rate-hike odds repricing (31% July, 84% Sept) — rising oil = rising inflation = hawkish Fed = broad equity headwind
- Day 0 — zero positions, zero live P&L data to validate any read yet

### Decision
HOLD — Day 0, no positions. CPI print tomorrow is the key catalyst; entering Energy/Staples momentum names ahead of it is unnecessary risk. Patience > activity. Revisit trade ideas post-CPI.

## 2026-07-20 — Pre-market Research

### Account
- Equity: $1,002,015.99
- Cash: $884,183.99
- Buying power: $3,866,665.56 (margin, 4x)
- Daytrade count: not returned by account endpoint (0 trades executed since inception)
- Deployed: $117,832 in XOM only = **11.8%** of equity — well below 75-85% target
- Open position: XOM 800sh @ $144.77, current ~$147.3-147.9, unrealized +$2,016 (+1.7%), GTC trailing-stop 10% live (stop $135, hwm $150)

### Market Context
- WTI ~$82-84 (+2-4%), Brent ~$88-90 (+4.6%) — Iran/Strait of Hormuz risk premium persists despite reported peace-talk headlines easing some tension
- S&P 500 futures: ~7,496-7,518, flat/slightly bullish bias into the open
- VIX: ~18.3-18.5 (moderate, up from mid-teens last week)
- Today's catalysts: TSMC record Q2 (AI/HPC 61% of revenue, capex raised to $60-64B) — bullish semis/AI-infra; China approved "Apple Intelligence" — Alibaba/Tencent rallied; Japan AI-hardware (SoftBank, Tokyo Electron, Kioxia) sliding on valuation reset — AI rotation from hardware to applications; Fed Chair Kevin Warsh hawkish "prices too high" comments stoking rate-cut-timing uncertainty
- Earnings before open: CVX 6:15am (Energy peer to our XOM position), Dominion Energy, Cboe Global Markets, Domino's Pizza, AMC, Dynex Capital, Arbor Realty, Cleveland-Cliffs. PepsiCo + Delta report later this week — first real test of Q2 season strength
- Economic calendar: nothing today — June CPI already printed 7/14 (3.5% YoY, cooler than 3.8% forecast); next CPI not until 8/12. No FOMC this week
- Sector momentum YTD: Energy (+17-23%), Materials (+15-17%), Consumer Staples (+12-16%) leading; Financials (-7%), Consumer Discretionary (-4%), broad Tech (-3%, though semis/hardware sub-sectors still strong) lagging

### Trade Ideas
1. CVX — catalyst: reports Q2 earnings 6:15am ET today, same Energy-momentum tailwind as our XOM position (oil +4-5% this week). WAIT for print + reaction before entering (do not buy blind into earnings); if reaction confirms strength, entry ~market, stop -8%, target +16%, R:R 2:1
2. Consumer Staples (PG/KO/COST) — catalyst: sector YTD leadership + defensive/inflation-hedge rotation; PepsiCo earnings later this week is the confirming/disconfirming catalyst for the group. WAIT for PEP print, entry ~market, stop -7%, target +14%, R:R 2:1
3. Materials (LIN/FCX/XLB) — catalyst: YTD momentum leader, no company-specific trigger today — does not clear the "specific catalyst" bar in the entry checklist yet; watchlist only

### Risk Factors
- Only 1 position, 11.8% deployed vs 75-85% target — account has sat idle for a full week (no trade/research log entries 7/14-7/19); worth confirming whether scheduled workflows are actually running daily
- Oil spike is double-edged: further Iran/Hormuz de-escalation would reverse the Energy tailwind fast (headline risk both ways)
- Fed Chair Warsh's hawkish rate-cut pushback adds macro uncertainty into a market already digesting AI-spending anxiety (Nasdaq retreated last week)
- CVX earnings this morning could move XOM/Energy complex sharply in either direction — do not chase pre-print

### Decision
HOLD — CVX and PEP/DAL earnings this week are the real triggers; no name today clears the "specific catalyst" checklist item pre-print. Flag for next session: account is materially under-deployed (11.8% vs 75-85% target, 1 of 5-6 max positions) — once CVX/PEP earnings clarify, prioritize adding 1-2 positions per the 3-trades/week allowance rather than sitting fully idle again.

## 2026-07-21 — Pre-market Research

### Account
- Equity: $1,002,815.99
- Cash: $884,183.99
- Buying power: $3,868,905.56 (margin, 4x)
- Daytrade count: 0 (not returned by API; no day trades taken)
- Deployed: $118,632 in XOM only = **11.8%** of equity — still well below 75-85% target
- Open position: XOM 800sh @ $144.77, current $148.29, unrealized +$2,816 (+2.4%), GTC trailing-stop 10% live (stop $135, hwm $150)
- Open orders: 1 (XOM trailing-stop sell, unchanged)

### Market Context
- WTI ~$82.1-83.2 (flat/-0.4%), Brent ~$88.4-88.9 (flat/-0.8%) — Iran/Strait of Hormuz risk premium persists but has stopped climbing this week
- S&P 500 futures: ~7,527, +0.57% premarket — Nasdaq 100 futures +1.3%, led by a semiconductor rebound (NVDA +6.2%, AVGO +7.8% premarket) on confirmed AWS capex increases (~$8.2B) and AVGO's Q3 guidance beat ($16.8B rev, +12% vs consensus)
- VIX: 17.58, down from 18.65 Monday close — vol easing back after last week's uptick
- Today's catalysts: chip/AI-infra rebound (NVDA, AVGO, IREN +18% on new AI cloud contracts) reversing last week's AI-capex anxiety; Eli Lilly down on a failed GLP-1 trial (biotech drag); Apple/Tesla lagging the Nasdaq; new US tariffs on Canadian goods in focus; Fed Chair Warsh testified before House Financial Services Committee 10am ET yesterday (hawkish-leaning, "prices too high")
- Earnings before open: none major confirmed for today — GM, Starbucks, AT&T, VF Corp all reported Monday 7/20; next real test is later this week
- Economic calendar: nothing major today — June CPI already printed 7/14 (3.5% YoY, cooled from 4.2%, core flat MoM); next CPI not until 8/12; no FOMC this week
- Sector momentum YTD: Energy (+15.9-23%) and Materials (+15.9-17.4%) still leading, Consumer Staples (+11-15%) and Industrials improving; Technology YTD still negative-to-flat (-3.4% to +2.9%) despite today's sharp semis bounce; Financials/Discretionary/Comm Services lagging

### Trade Ideas
1. XOM (existing position) — thesis intact: Hormuz premium holding, Energy still #1 YTD sector, Wells Fargo raised PT to $158, Morgan Stanley to $137. No new entry needed; stop unchanged at $135 (10% GTC trailing, hwm $150).
2. AVGO/semis — catalyst is real (confirmed AWS capex, strong Q3 guide) but the move already happened premarket (+7.8%); chasing a gap that size violates "never buy blind" discipline, and Tech remains a YTD sector laggard despite the bounce — doesn't clear the sector-momentum checklist item. Watchlist only; would need a pullback to a defensible entry with a fresh catalyst.
3. Materials (LIN/FCX) — YTD momentum leader, but no company-specific dated catalyst today — same gap as prior sessions. Watchlist only.

### Risk Factors
- Still only 1 of 5-6 target positions, 11.8% deployed vs 75-85% target — third consecutive session flagging under-deployment; no new trade has cleared the full entry checklist (specific catalyst + sector momentum + defensible entry) since XOM
- Today's semis rally is a single-day, gap-driven move — high chase risk, easy to reverse if AI-capex skepticism resurfaces (as it did last week)
- Middle East/oil headline risk still cuts both ways for the XOM thesis — a de-escalation headline would remove the premium quickly
- VIX pulled back to 17.58 (from 18.65) — no acute stress signal, but Warsh's hawkish tone keeps macro uncertainty alive into next month's CPI/FOMC

### Decision
HOLD — no new trades today. XOM position (11.8% of equity) has an intact thesis and active 10% GTC trailing stop. Today's best-looking setup (AVGO/semis) already gapped up sharply pre-market with no pullback entry, so it doesn't meet the "never chase" discipline; Materials still lacks a dated, company-specific catalyst. Patience > activity — continue watching AVGO/semis and Materials for a cleaner entry, and revisit the under-deployment gap once one clears the checklist.
