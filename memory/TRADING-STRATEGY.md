# Trading Strategy

## Mission
Beat the S&P 500 over the challenge window. Stocks only — no options, ever.

## Capital & Constraints
- Starting capital: ~$1,000,000 (PAPER account)
- Platform: Alpaca
- Instruments: Stocks ONLY
- PDT limit: 3 day trades per 5 rolling days (account < $25k) — not
  applicable at this account size, kept here as a standing reference

## Core Rules
1. NO OPTIONS — ever
2. 75-85% deployed
3. 5-6 positions at a time, max 20% each
4. 10% trailing stop on every position as a real GTC order
5. Cut losers at -7% manually
6. Tighten trail: 7% at +15%, 5% at +20%
7. Never within 3% of current price; never move a stop down
8. Max 3 new trades per week
9. Follow sector momentum
10. Exit a sector after 2 consecutive failed trades
11. Patience > activity
12. Logging integrity: every scheduled run must write to its memory
    file before finishing, even on a no-op/HOLD day. If a run can't
    reach memory or a wrapper script, alert via ClickUp immediately
    instead of skipping silently. A gap of 3+ consecutive missed
    trading-day log entries is an incident, not a footnote — flag it
    explicitly in the next entry that runs.
    (Added 2026-09-11: TRADE-LOG.md and RESEARCH-LOG.md went dark for
    7/24-9/11, ~7 weeks, hiding two real fills. Failed badly.)

## Entry Checklist
- Specific catalyst?
- Sector in momentum?
- Stop level (7-10% below entry)
- Target (min 2:1 R:R)
