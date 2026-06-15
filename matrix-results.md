# Consensus Radar — 4x4 Matrix Results
## June 12, 2026

16 runs: 4 prompts × 4 models (1 missing: gemini-on-gpt55 due to OpenRouter issue)

## Models
| Model | OpenRouter ID |
|-------|--------------|
| Claude Opus 4.8 | anthropic/claude-opus-4.8 |
| GPT 5.5 | openai/gpt-5.5 |
| Gemini 3.1 Pro | google/gemini-3.1-pro-preview |
| Grok 4.3 | x-ai/grok-4.3 |

## Prompts
| Prompt | Style | Author |
|--------|-------|--------|
| opus | Conversational, structured, conviction ranking | Claude Opus 4.8 |
| gpt | Formal, comprehensive, 11 fields per trade | GPT 5.5 |
| gemini | Options-literate, PMCC/diagonal aware | Gemini 3.1 Pro |
| grok | Casual, human-sounding, text-to-a-buddy | Grok 4.3 |

---

## TICKER CONSENSUS (across all 16 runs)

| Ticker | Mentions | Strength | Notes |
|--------|----------|----------|-------|
| IWM    | 14/16    | ██████████████ | Unanimous small-cap rotation play |
| SPY    | 14/16    | ██████████████ | Always mentioned as context vehicle |
| SMH    | 12/16    | ████████████ | Semi sector ETF, strong consensus |
| MSFT   | 11/16    | ███████████ | #1 individual stock pick |
| V      | 11/16    | ███████████ | Visa — surprising, but liquidity/quality |
| NVDA   | 9/16     | █████████ | Momentum play, not universal |
| QQQ    | 7/16     | ███████ | Tech index, moderate |

### Key findings:
- **IWM is the #1 consensus trade** — 14/16 runs recommend small caps
- **MSFT is the #1 individual stock** — beaten-down quality name
- **SMH over NVDA** — models prefer the sector ETF over the single stock
- **V (Visa)** appears as a quality/defensive play in 11/16 runs
- **AMD barely registers** (2/16) despite being in the same space as NVDA

## BY PROMPT (what each prompt surface)

| Ticker | Opus prompt | GPT prompt | Gemini prompt | Grok prompt |
|--------|-------------|------------|---------------|-------------|
| IWM    | 4/4         | 4/4        | 3/4           | 3/4         |
| SPY    | 4/4         | 4/4        | 2/4           | 4/4         |
| SMH    | 3/4         | 3/4        | 3/4           | 3/4         |
| MSFT   | 4/4         | 0/4        | 3/4           | 4/4         |
| V      | 4/4         | 4/4        | 1/4           | 2/4         |
| NVDA   | 4/4         | 2/4        | 0/4           | 3/4         |

### Prompt sensitivity:
- **GPT prompt never surfaces MSFT** (0/4) — its formal structure may bias toward different picks
- **Opus prompt is most consistent** — surfaces the same names across all 4 models
- **Gemini prompt drops NVDA** (0/4) — options-literate prompt may avoid overextended names
- **Grok prompt is most bullish** — casual style gets the most directional long picks

## BY MODEL (what each AI recommends)

| Ticker | Opus | GPT 5.5 | Gemini | Grok |
|--------|------|---------|--------|------|
| IWM    | 4/4  | 2/4     | 4/4    | 4/4  |
| SPY    | 4/4  | 3/4     | 4/4    | 3/4  |
| SMH    | 4/4  | 2/4     | 2/4    | 4/4  |
| MSFT   | 3/4  | 2/4     | 3/4    | 3/4  |
| V      | 3/4  | 2/4     | 4/4    | 2/4  |
| NVDA   | 3/4  | 2/4     | 2/4    | 2/4  |

### Model personality:
- **Gemini** is the most consistent on IWM and V — quality/rotation focused
- **Opus** is the most bullish — surfaces the most tickers across prompts
- **GPT 5.5** is the most selective — fewer tickers, more concentrated picks
- **Grok** mirrors Opus but with more NVDA/momentum exposure

---

## STRATEGY CONSENSUS (across all 16 runs)

| Strategy       | Mentions | Notes |
|----------------|----------|-------|
| Spread         | 14/16    | Dominant strategy type |
| LEAPS          | 13/16    | Long-dated calls on quality names |
| Call spread    | 11/16    | Bull call spreads most common |
| Bull call      | 10/16    | Directional long with defined risk |
| Credit spread  | 10/16    | Some models recommend selling premium |
| Put spread     | 9/16     | Less common but present |
| Covered call   | 7/16     | Income on existing positions |
| Shares         | 7/16     | Direct stock ownership |
| Cash reserve   | 5/16     | Some models say keep dry powder |
| Diagonal/PMCC  | 7/16     | Sophisticated options structures |

### Strategy signal:
- **The crowd is being told to BUY options** (LEAPS, bull calls) — not sell
- **Put spreads appear in 9/16** — some hedging, but minority
- **Credit spreads (selling premium) in 10/16** — some models recommend it
- **PMCC/diagonal in 7/16** — the Gemini prompt surfaces this more

---

## IMPLICATIONS FOR SPX CREDIT SPREADS

1. **IWM consensus = breadth improvement** — small caps leading means SPX has a broad base, not just mega-cap tech. Put credit spreads are safer.

2. **MSFT as #1 stock pick** — the crowd is buying MSFT calls. Market makers delta-hedge by buying MSFT stock. MSFT is a top-3 SPX component. This creates bid pressure.

3. **LEAPS buying = long delta crowd** — retail is being told to buy calls, not sell. You're on the other side collecting theta.

4. **NVDA is NOT unanimous** (9/16) — the crowd is less sure about NVDA than MSFT. NVDA momentum may be fading as a crowd trade.

5. **V as a surprise consensus** — if the crowd is buying Visa, that's a defensive quality rotation. Means some traders are hedging with quality, not just YOLOing tech.

6. **Put spreads appear in 9/16** — a meaningful minority of AI recommendations include downside protection. Watch for put buying flow on SPX/SPY.

---

## FILES

### Prompts (what each model crafted)
- `prompt-v1.md` — Opus prompt
- `prompt-gpt55.md` — GPT 5.5 prompt
- `prompt-gemini31pro.md` — Gemini 3.1 Pro prompt
- `prompt-grok43.md` — Grok 4.3 prompt

### Matrix responses (4x4 = 16 files)
- `matrix/opus-on-opus.md` through `matrix/grok-on-gpt55.md`

### Analysis
- `matrix/_index.json` — raw index with token counts
- `matrix/_analysis.json` — structured analysis data
- `results-v1.md` — original single-prompt results
- `prompt-comparison.md` — prompt style comparison
