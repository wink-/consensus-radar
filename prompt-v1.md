# Consensus Radar — Prompt v1

## Origin
Crafted by Claude Opus 4.8 via OpenRouter on 2026-06-12.
Designed to simulate what a sophisticated retail trader would ask an AI financial advisor.

## The Prompt

Hey, I want to put some capital to work over the next 1-3 months and need your help thinking through specific trades. Let me give you my situation and the current market backdrop, then I'm hoping you can give me 5 concrete ideas I can actually execute.

**My account:**
- $50K in a Schwab brokerage account
- Approved for defined-risk options (vertical spreads, LEAPS, covered calls)
- Horizon is 1-3 months, though I'm fine holding LEAPS longer
- Risk tolerance is moderate-to-aggressive — I can stomach drawdowns but I don't want to blow up the account on one bad trade

**Current market data (as of [DATE]):**
- SPY: [PASTE PRICE / recent move]
- VIX: [PASTE LEVEL]
- 10Y yield: [PASTE]
- Recent market action: [PASTE — e.g., what the last week looked like, any Fed/earnings/macro events, what's leading vs. lagging]
- Sector performance: [PASTE — which sectors are hot/cold, any rotation you're seeing]
- Anything else on my radar: [PASTE — specific tickers, earnings dates, news you want factored in]

**What I'm looking for:**

Give me 5 distinct trade ideas. I want a mix of approaches, not 5 versions of the same bet:
- At least one **LEAPS** play on a quality name that's been beaten down but has a catalyst or mean-reversion case
- At least one **momentum / trend-continuation** play
- At least one **sector rotation** idea based on what's actually working right now
- Use covered calls or spreads where they make sense to define risk

For each idea, I need the specifics so I can place the order:
1. **Ticker and the thesis** in 2-3 sentences — why now?
2. **Exact structure**: strikes, expiration, debit/credit, and whether it's a spread, LEAP, covered call, etc.
3. **Position size** — how much of the $50K, and how many contracts/shares, with the max loss in dollars
4. **Risk/reward**: breakeven, max profit, max loss, and a rough probability read if you can
5. **What would make you wrong** — the invalidation point or where I should cut it

A few ground rules:
- Keep total risk reasonable across all 5 — I don't want to deploy the whole account at once or have everything correlated to one macro outcome
- Prefer liquid underlyings with tight options spreads (no thinly-traded junk)
- Be honest about which of these are higher-conviction vs. lottery-ticket-ish
- If something in the current market makes you want to sit on cash instead of forcing a 5th idea, tell me that

Rank them by conviction at the end and tell me which one you'd put on first if I could only do one today.

## Market Context (fill before running)

Date: June 12, 2026
SPY: 756.08 (just bounced from 725 low on June 10, +4.4% in 2 days)
VIX: ~18 (declining from spike, was 25+ earlier in week)
10Y yield: [TBD]
Recent market action: SPY had a 5% drawdown June 5-10, V-reversal recovery June 11-12. Tech led the bounce. Small caps (IWM) strongest structure.
Sector performance: Tech recovering hardest, defensives lagging, semis bouncing from oversold
On radar: MSFT down 18% from recent high, NVDA near ATH area, broad market recovery in progress

## Models to Query
1. anthropic/claude-opus-4.8 (done — baseline)
2. openai/gpt-latest
3. google/gemini-pro-latest
4. x-ai/grok-4.3
