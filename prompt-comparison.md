# Consensus Radar — Prompt Comparison v1
## June 12, 2026

Each model was asked: "Write a prompt that a sophisticated retail trader would use to get AI stock/options trade recommendations."

---

## Claude Opus 4.8

Tone: Conversational but structured. Asks for 5 ideas with a mix of LEAPS, momentum, and sector rotation. Includes ground rules about liquidity, conviction honesty, and the option to sit on cash. Ends with "rank by conviction, tell me which one to put on first."

Key features:
- Placeholders for SPY, VIX, 10Y yield, sector performance, "anything else on radar"
- Asks for invalidation points ("what would make you wrong")
- Asks for probability read
- Explicit "don't deploy the whole account" constraint
- "Be honest about conviction vs lottery-ticket-ish"

Length: Medium. Natural-sounding, not overly formal.

---

## GPT 5.5

Tone: More formal and comprehensive. The most detailed output format — asks for 11 specific fields per trade including exit plan, key risks, catalysts, and risk/reward ratio. Explicitly mentions Robinhood/Schwab/Thinkorswim by name.

Key features:
- Asks for QQQ and IWM prices in addition to SPY/VIX
- Sector ETF list: XLK, XLF, XLE, XLY, XLV, XLI, SMH
- Asks for "major macro events coming up" (CPI, Fed, earnings, jobs)
- 1-3% risk per trade guideline
- "Estimated entry price" with option pricing
- Exit plan with profit target, time-based exit, and adverse move logic
- "Don't give me generic ideas — specific executable setups"
- Adjusts toward defensive if market is unfavorable

Length: Long. Most thorough prompt of the four.

---

## Gemini 3.1 Pro

Tone: Casual but knowledgeable. Uses terms like "Poor Man's Covered Calls" and "diagonals" — signals a trader who knows options mechanics. Asks for "quantitative options strategist" roleplay.

Key features:
- Mentions diagonals/PMCC explicitly (more options-literate)
- "Naked calls/puts are off the table" — explicit constraint
- 5 ideas but with specific structure: 1 LEAPS, 1 momentum, 1 sector rotation, 2 "opportunistic"
- Asks for exact DTE, not just expiration dates
- "Give me setups I can literally pull up on Schwab or Robinhood and execute today"
- "What are we trading?" — action-oriented closer

Length: Medium-short. Most concise of the four.

---

## Grok 4.3

Tone: The most casual and human-sounding. Reads like a text message to a trading buddy. Short sentences, minimal formatting, conversational.

Key features:
- Shortest prompt by far
- "Nothing crazy directional with undefined risk"
- "Realistic ideas I could actually put on in Schwab or Robinhood this week"
- "Appreciate it" closer
- Asks for "rough risk/reward" not exact math
- "Why you're looking at that name" — wants the thesis, not just the trade
- Most relaxed about formatting requirements

Length: Short. Most natural-sounding.

---

## COMPARISON TABLE

| Feature              | Opus  | GPT 5.5 | Gemini | Grok  |
|---------------------|-------|---------|--------|-------|
| Length               | Med   | Long    | Med    | Short |
| Formality            | Med   | High    | Med    | Low   |
| Specificity          | High  | Highest | High   | Med   |
| Exit plan requested  | No    | Yes     | No     | Yes   |
| Conviction ranking   | Yes   | No      | No     | No   |
| Cash option          | Yes   | Yes     | No     | No   |
| Macro events asked   | No    | Yes     | No     | No   |
| Probability asked    | Yes   | No      | No     | No   |
| Options sophistication| Med  | Med     | High   | Low   |
| Human-sounding       | Yes   | Somewhat| Yes    | Most  |

## WHAT THIS TELLS US

The prompts differ in sophistication and detail. When we query the
models with these prompts, we'll get different outputs:

- GPT 5.5's prompt → most detailed responses, most structured
- Grok's prompt → most natural responses, might be vaguer
- Gemini's prompt → most options-literate, PMCC/diagonal aware
- Opus's prompt → best for ranking/conviction scoring

For the consensus radar, the prompt differences mean:
- GPT's prompt will surface more trade ideas (11 fields per trade)
- Grok's prompt will surface what casual traders would get
- Gemini's prompt will get more sophisticated options structures
- Opus's prompt gives us conviction ranking built in

We should test all 4 prompts against all 4 models to see which
prompt produces the best consensus data. That's a 4x4 matrix.

## FILES
- prompt-v1.md — Claude Opus prompt
- prompt-gpt55.md — GPT 5.5 prompt
- prompt-gemini31pro.md — Gemini 3.1 Pro prompt
- prompt-grok43.md — Grok 4.3 prompt
