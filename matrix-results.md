# Consensus Radar — 4x4 Matrix Results (Complete)
## June 12, 2026

16/16 runs complete. 4 prompts × 4 models.

## Models
| Model | Source |
|-------|--------|
| Claude Opus 4.8 | OpenRouter |
| GPT 5.5 | Codex CLI (OpenAI plan) |
| Gemini 3.1 Pro | OpenRouter |
| Grok 4.3 | OpenRouter |

---

## TICKER CONSENSUS (16/16 runs)

| Ticker | Mentions | Strength |
|--------|----------|----------|
| IWM    | 16/16    | ████████████████ UNANIMOUS |
| SPY    | 15/16    | ███████████████ STRONG |
| MSFT   | 13/16    | █████████████ STRONG |
| SMH    | 11/16    | ███████████ STRONG |
| V      | 11/16    | ███████████ STRONG |
| NVDA   | 11/16    | ███████████ STRONG |
| QQQ    | 6/16     | ██████ moderate |
| AMD    | 4/16     | ████ weak |

### Key findings:
- **IWM is unanimous (16/16)** — every prompt, every model says buy small caps
- **MSFT is the #1 individual stock (13/16)** — beaten-down quality name
- **NVDA is strong but not unanimous (11/16)** — momentum play, some models skip it
- **SMH over single semis** — models prefer the ETF over AMD/NVDA individually
- **V (Visa) is a surprise strong consensus** — quality/defensive rotation

## BY PROMPT

| Ticker | Opus | GPT | Gemini | Grok |
|--------|------|-----|--------|------|
| IWM    | 4/4  | 4/4 | 4/4    | 4/4  |
| SPY    | 4/4  | 4/4 | 3/4    | 4/4  |
| MSFT   | 4/4  | 1/4 | 4/4    | 4/4  |
| SMH    | 3/4  | 2/4 | 3/4    | 3/4  |
| V      | 4/4  | 4/4 | 1/4    | 2/4  |
| NVDA   | 4/4  | 2/4 | 1/4    | 4/4  |

### Prompt sensitivity:
- **GPT prompt drops MSFT** (1/4) — formal structure biases away from it
- **Opus prompt is most consistent** — same picks across all models
- **Gemini prompt drops V** (1/4) — options-literate focus on different names
- **Grok prompt is most bullish** — casual style gets the most directional picks

## BY MODEL

| Ticker | Opus | GPT 5.5 | Gemini | Grok |
|--------|------|---------|--------|------|
| IWM    | 4/4  | 4/4     | 4/4    | 4/4  |
| SPY    | 4/4  | 4/4     | 4/4    | 3/4  |
| MSFT   | 3/4  | 4/4     | 3/4    | 3/4  |
| SMH    | 4/4  | 1/4     | 2/4    | 4/4  |
| V      | 3/4  | 2/4     | 4/4    | 2/4  |
| NVDA   | 3/4  | 4/4     | 2/4    | 2/4  |

### Model personality:
- **GPT 5.5** is the most MSFT/NVDA bullish — picks the mega-caps
- **Gemini** is the most V/quality focused — defensive rotation
- **Opus** is the most SMH/sector focused — ETF over single names
- **Grok** mirrors Opus but with less V exposure

---

## STRATEGY CONSENSUS

| Strategy       | Mentions |
|----------------|----------|
| LEAPS          | 15/16    |
| Spread         | 15/16    |
| Call spread    | 12/16    |
| Credit spread  | 10/16    |
| Bull call      | 9/16     |
| Put spread     | 8/16     |
| Shares         | 8/16     |
| Covered call   | 7/16     |
| Diagonal/PMCC  | 8/16     |
| Cash reserve   | 5/16     |

### Strategy signal:
- **Crowd is buying options** (LEAPS, bull calls) — not selling
- **Credit spreads appear in 10/16** — some models recommend selling premium
- **Put spreads in 8/16** — minority hedging
- **PMCC/diagonal in 8/16** — sophisticated structures being recommended

---

## IMPLICATIONS FOR SPX CREDIT SPREADS

1. **IWM unanimous = breadth is back** — small caps leading means SPX has a broad base. Put credit spreads are safer when breadth is strong.

2. **MSFT 13/16 = crowd is buying MSFT calls** — market makers delta-hedge by buying stock. MSFT is top-3 SPX component. Structural bid pressure.

3. **LEAPS buying (15/16) = retail is net long delta** — you're on the other side collecting theta on short-dated spreads.

4. **NVDA strong (11/16) but not unanimous** — momentum is there but some models are cautious. Less crowding than MSFT.

5. **V as consensus (11/16)** — some traders are rotating into quality/defensive. Means the crowd isn't all-in on growth. Mixed signals = choppier = good for premium sellers.

6. **Credit spreads in 10/16** — the AI crowd is being told to SELL premium too, not just buy. This means more competition on the short side, but also more liquidity.

---

## COST

OpenRouter: ~$0.44 (Opus + Gemini + Grok × 4 prompts each)
Codex CLI: $0 (included in OpenAI plan)
Total: ~$0.44 for 16 consensus data points

## FILES

### Prompts
- `prompt-v1.md` — Opus prompt
- `prompt-gpt55.md` — GPT 5.5 prompt
- `prompt-gemini31pro.md` — Gemini 3.1 Pro prompt
- `prompt-grok43.md` — Grok 4.3 prompt

### Matrix (16 responses)
- `matrix/{prompt}-on-{model}.md` — e.g., `opus-on-gpt55.md`

### Analysis
- `matrix/_analysis.json` — structured data
- `matrix-results.md` — this file
- `results-v1.md` — original single-prompt results
- `prompt-comparison.md` — prompt style comparison
