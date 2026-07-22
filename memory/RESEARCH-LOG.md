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

## 2026-07-21 — Pre-market Research (run inline during market-open; entry was missing)

### Account
- Equity: $1,003,263.99
- Cash: $884,183.99
- Buying power: $3,870,159.96 (margin, 4x)
- Positions: 1 (XOM, 800 sh), deployed $119,080 = **11.9%** of equity — still well below 75-85% target
- Daytrade count: not reported by API (0 day trades taken)
- Trades this week (since Mon 7/20): 0

### Market Context
- WTI ~$82 (-0.6%), Brent ~$88-90 (flat/slightly down) — Iran ceasefire-mediation headlines easing the risk premium slightly
- S&P 500 futures: ~7,485-7,526, +0.5-0.6% premarket on Iran ceasefire hopes + earnings focus
- VIX: ~17.6-18.6, down from Monday's 18.65-18.77 — vol easing
- Today's catalysts: semiconductor/AI-infra earnings pop (NVDA +6.2% premarket, AVGO +7.8% premarket on strong data-center/Tier-1 guidance), GM beat + Panasonic-Tesla Cybertruck battery deal, Shopify layoffs + AI capex reallocation; 87% of 54 S&P reporters beating so far
- Earnings before open: GM, MMM, NOC, GPC (none in our Energy/Materials/Staples momentum lane)
- Economic calendar: no CPI/PPI/FOMC/jobs today; next FOMC 7/29, next CPI 8/12; weekly jobless claims Thu
- Sector momentum YTD: Energy #1 (+22-30%), Materials #2 (+11-17%), Consumer Staples #3 (+11-16%), Industrials #4 (+12-16%) leading; Tech (-3.4% price YTD, despite today's AI pop), Financials, Consumer Discretionary lagging
- CVX correction: no CVX earnings printed 7/20 as prior log assumed — Q2 report now confirmed for 7/31; Monday's 1.2% CVX gain was oil-price/sentiment driven, not an earnings reaction
- XOM (existing position): ~$148.6, +1.0% — Iraq requested to buy $350M stake in an Exxon oilfield (positive); activist investor proxy fight pushing for new leadership vs CEO Woods, and Trump said he's "inclined to keep Exxon out" of Venezuela (both headline noise, not thesis-breaking). Goldman Hold $157 PT; Piper Sandler/Jefferies Buy; avg PT $166.90

### Trade Ideas
1. No new name today — today's hottest movers (NVDA, AVGO semis pop) sit in Tech, our weakest YTD sector; chasing a one-day AI rally there contradicts the "follow sector momentum" rule and the account's Energy/Materials/Staples-leadership framework.
2. GM/MMM/NOC earnings beats are real but sit in Discretionary/Industrials-adjacent names with no tie to our current thesis or a 2:1 R:R setup screened yet — watchlist only, not actionable today.
3. Materials (LIN/FCX/XLB) — still the #2 YTD sector, but no company-specific dated catalyst today — doesn't clear the entry checklist.

### Risk Factors
- CVX earnings pushed to 7/31 — prior log's assumption of a 7/20 print was wrong; don't treat CVX as an imminent catalyst until confirmed closer to date
- XOM headline noise (activist proxy fight, Venezuela comments) — governance overhang worth monitoring but not thesis-breaking; no action needed, stop still 10% GTC trailing (stop $135, hwm $150)
- Still only 1 of 5-6 target positions, 11.9% deployed vs 75-85% target for a second straight session — under-deployment flagged twice now with no new catalyst clearing the bar; watch for the risk of "patience" drifting into pure inertia if this persists past this week without a genuine dated catalyst

### Decision
HOLD — no new trades today. XOM thesis intact, stop active. No name clears the specific-catalyst + sector-momentum bar; today's AI/semis rally is a Tech (laggard sector) event, not aligned with strategy. Materials/Staples remain the more strategy-aligned watchlist candidates pending a dated trigger.

## 2026-07-22 — Pre-market Research (run inline during market-open; entry was missing)

### Account
- Equity: $1,006,815.99
- Cash: $884,183.99
- Buying power: $3,880,105.56 (margin, 4x)
- Positions: 1 (XOM, 800 sh @ $144.77, current ~$153.29, unrealized +$6,812 / +5.88%), deployed $122,632 = **12.2%** of equity — still well below 75-85% target
- GTC trailing stop live on XOM: stop $138.69, hwm $154.10
- Daytrade count: not reported by API (0 day trades taken)
- Trades this week (since Mon 7/20): 0/3

### Market Context
- WTI ~$85-88 (+2.5-4%), Brent ~$91-93 (+2-2.5%) — six-week highs. Iran ceasefire has collapsed; Secretary Rubio said Iran is "not serious" about peace talks, reversing the de-escalation that had pressured oil lower
- S&P 500 futures: ~7,520, -0.3-0.4% premarket — Dow/S&P soft, Nasdaq -0.7-0.8% (chip-stock weakness), ahead of Alphabet/Tesla/IBM/Texas Instruments earnings after today's close
- VIX: ~18.8
- Today's catalysts: Iran ceasefire collapse driving oil to 6-week highs; energy shares leading global gains; Big Tech (GOOGL, TSLA, IBM, TXN, GE Vernova, PM, T) all report after the close — AI-momentum test, not a premarket item
- Earnings before open: none clearly confirmed in our sector lane; big reports are after-hours today
- Economic calendar: no CPI/PPI/FOMC/jobs before open; UK CPI overnight (not a US market mover)
- Sector momentum YTD: Energy #1 (+29-30%, some sources 23%), Materials #2 (+9-17% depending on source), Consumer Staples top-3 — Energy leadership reconfirmed and extended by today's ceasefire-collapse headline
- XOM (existing position): $153.29, up another leg on the same oil move; institutional buying reported (Jennison Associates raised stake), Q2 earnings confirmed for 7/31 (not today) — thesis fully intact, no new action needed beyond the existing trailing stop

### Trade Ideas (evaluated, not taken)
1. CVX — catalyst real and dated (ceasefire collapse, oil 6-wk highs, Wolfe upgraded to Outperform 7/2 $210 PT, consensus PT ~$206-216, 52-wk high $214.71). BUT current price already ~$191-193, up from ~$165 three weeks ago — most of the move is already priced in. Upside to consensus PT is only ~+10-12%; against our mandatory 10% trailing stop that's a ~1:1 R:R, well short of the 2:1 minimum on the entry checklist. Wide/erratic quote spread (bid $182.83 / ask $195) also a data-quality flag this morning. PASS — chasing, not entering.
2. OXY — same oil catalyst, current ~$57.58, consensus PT ~$64.2-64.5 (+11-12%), 52-wk high $67.45 (+17%). Analyst consensus is only "Hold" (10 buy/16 hold), weaker conviction than CVX/XOM. Similar ~1:1 R:R against the 10% trailing stop. PASS.
3. No Energy name today clears 2:1 R:R from current (already-elevated) levels. Watchlist for a pullback entry into CVX/OXY if oil gives back some of today's spike and price resets closer to the $170s/$50s.

### Risk Factors
- Oil/Iran headline risk cuts both ways — any de-escalation headline would reverse today's Energy tailwind fast, as it already did earlier this month (CVX/XOM fell 4-7% on the last ceasefire announcement)
- Big Tech earnings after the close (GOOGL, TSLA, IBM, TXN) could swing broad-market sentiment/VIX into tomorrow's session regardless of our Energy positioning
- Still only 1 of 5-6 target positions, 12.2% deployed vs 75-85% target for a fourth straight session — under-deployment remains flagged, but today's Energy names don't clear the R:R bar at current (post-rally) prices; forcing a marginal-R:R trade just to hit a deployment number would violate the discipline the checklist exists to enforce
- XOM has no new company-specific risk; governance/proxy-fight noise from 7/21 unchanged

### Decision
HOLD — no new trades today. XOM thesis intact and strengthening on the same catalyst; existing 10% GTC trailing stop stands (stop $138.69, hwm $154.10). CVX/OXY both have a genuine, dated catalyst but neither clears 2:1 R:R at today's already-elevated prices — flagged as pullback watchlist candidates, not chased. Patience > activity; under-deployment (12.2% vs 75-85%) stays an open flag for a session with a fresh setup at a better entry price.
