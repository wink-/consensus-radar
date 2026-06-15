# Consensus Radar

What are AI models telling retail traders to buy — and how do we position on the other side?

## Concept

Every day, thousands of retail traders ask Claude, ChatGPT, Gemini, and Grok for stock picks. Those models recommend the same names, the same strategies, the same LEAPS. That creates predictable options flow.

**The LLM isn't your analyst. The LLM is your read on what everyone else's analyst is telling them.**

This project queries 4 top-tier AI models with 4 different prompts (simulating what retail traders actually ask) and aggregates the results into a consensus signal.

## Models Queried
- Claude Opus 4.8 (via OpenRouter)
- GPT 5.5 (via Codex CLI / OpenAI plan)
- Gemini 3.1 Pro (via OpenRouter)
- Grok 4.3 (via OpenRouter)

## How It Works

1. 4 prompts crafted by each model (see `prompt-*.md`)
2. Each prompt sent to all 4 models = 16 runs
3. Tickers, strategies, and conviction parsed from responses
4. Consensus scored: ticker mentions, strategy distribution, model agreement
5. Signal mapped against SPX positioning (credit spreads)

## Key Findings (June 12, 2026)

| Ticker | Consensus | Signal |
|--------|-----------|--------|
| IWM    | 16/16     | Unanimous small-cap rotation |
| SPY    | 15/16     | Broad market always mentioned |
| MSFT   | 13/16     | #1 individual stock pick |
| SMH    | 11/16     | Semi sector ETF |
| V      | 11/16     | Quality/defensive rotation |
| NVDA   | 11/16     | Momentum play |

**Strategy signal:** Crowd is buying calls (LEAPS, bull spreads). Not selling premium. Put spreads appear in only 8/16 runs.

## Repo Structure

```
prompt-v1.md              # Prompt by Claude Opus 4.8
prompt-gpt55.md           # Prompt by GPT 5.5
prompt-gemini31pro.md     # Prompt by Gemini 3.1 Pro
prompt-grok43.md          # Prompt by Grok 4.3
prompt-comparison.md      # Side-by-side prompt analysis
matrix/                   # 16 response files
  {prompt}-on-{model}.md  # e.g., opus-on-gpt55.md
  _analysis.json          # Structured consensus data
  _index.json             # Token counts and metadata
matrix-results.md         # Full analysis
results-v1.md             # Original single-prompt results
```

## Cost

~$0.44 per full 16-run matrix (12 via OpenRouter, 4 via Codex CLI).
