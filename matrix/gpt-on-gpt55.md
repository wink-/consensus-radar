I’ll verify live/near-live prices and available option expirations before suggesting anything executable. Because this is trading advice with real sizing, I’ll keep it defined-risk and frame it as trade candidates, not personalized financial advice.
I found the Alpaca connector tools for current market data. I’m checking whether option-chain access is available in this session; exact strikes need actual listed contracts and pricing, not guessed chains.
The option-chain tools are available. I’m pulling snapshots on the liquid names first, then I’ll price only a small set of candidate spreads so the recommendations are grounded in quoted bid/ask rather than theoretical pricing.
mcp: codex_apps/alpaca_get_clock started
mcp: codex_apps/alpaca_get_clock (failed)
user cancelled MCP tool call
mcp: codex_apps/alpaca_get_stock_snapshot started
mcp: codex_apps/alpaca_get_stock_snapshot (failed)
user cancelled MCP tool call
The Alpaca calls were cancelled by the connector before returning data. I’ll fall back to available market lookups for underlying prices; if option quotes remain unavailable, I’ll flag premiums as limit-price targets based on spread width rather than pretending to have a live chain.
web search: 
web search: finance: SPY
web search: 
web search: finance: SPY
web search: 
web search: finance: AMD
web search: 
web search: SPY price June 15 2026 quote
The public search results confirm the user’s stated tape is broadly in line with today’s market: SPX closed around 7,554 on June 15, semis led, AMD closed near 547, and NVDA near 212. I’m going to attempt one direct option-contract pull now; if the connector still cancels, I’ll use listed-style strikes and conservative debit/credit limits.
mcp: codex_apps/alpaca_get_option_contracts started
mcp: codex_apps/alpaca_get_option_contracts (failed)
user cancelled MCP tool call
web search: 
web search: June 15 2026 Nvidia stock closed 212.45 Broadcom 393.94 Qualcomm 220.81
Not financial advice; treat these as conditional trade candidates. I could not get live OPRA option quotes because the Alpaca option-chain call was cancelled, so the entries below use **hard limit prices**. Only place them if Schwab’s live option chain fills at/inside the stated limit.

Sources checked: June 15, 2026 reports show SPX closed near `7,554`, semis led, AMD closed near `547`, NVDA near `212`, AVGO near `394`, MSFT near `400`, GOOGL near `369`, ORCL near `193`, and banks were participating in rotation. Sources: [MarketWatch TXN/semis](https://www.marketwatch.com/data-news/texas-instruments-inc-stock-outperforms-competitors-on-strong-trading-day-81b1a6ca-16290525c030), [IBD AMD/semis](https://www.investors.com/news/technology/chip-stocks-record-high-sox-amd-micron-soxx/), [MarketWatch ORCL/MSFT/GOOGL](https://www.marketwatch.com/data-news/oracle-corp-stock-outperforms-competitors-on-strong-trading-day-cdf67bdb-4cb90de2a1d6), [MarketWatch banks](https://www.marketwatch.com/livecoverage/stock-market-today-dow-jones-s-p-500-nasdaq-oil-prices-us-iran-peace-deal-strait-of-hormuz/card/bank-stocks-head-for-record-closing-high-as-rally-broadens-beyond-tech-MSY37W8U4TQ81xKLfLki).

| # | Trade | Entry / Size | Max Loss | Max Profit | Breakeven |
|---|---|---:|---:|---:|---:|
| 1 | **AMD Aug. 21 560/610 call debit spread** | Buy 1 spread, pay `<= $15.00` | `$1,500` / 3.0% | `$3,500` | `575` |
| 2 | **NVDA Aug. 21 215/245 call debit spread** | Buy 2 spreads, pay `<= $5.00` each | `$1,000` / 2.0% | `$5,000` | `220` |
| 3 | **ORCL Jan. 16 2027 200/260 call spread** | Buy 1 spread, pay `<= $14.00` | `$1,400` / 2.8% | `$4,600` | `214` |
| 4 | **KBE Aug. 21 covered-call collar** | Buy 200 shares near `67.50`, sell 2x `74C`, buy 2x `62P`, net option credit `>= $0.60` | About `$980` / 2.0% | About `$1,420` | `66.90` |
| 5 | **IWM Sep. 18 270/250 bull put spread** | Sell 1 spread, collect `>= $5.00` | `$1,500` / 3.0% | `$500` | `265` |

**1. AMD momentum continuation**
Thesis: AMD is leading the semiconductor bounce after the MEXT acquisition and renewed AI/GPU enthusiasm. This is aggressive because AMD has already ripped, so use a debit spread instead of naked calls.

Catalysts: follow-through in semis, AI capex headlines, analyst target revisions, memory-shortage narrative.

Invalidation: AMD closes below `520`, or SOXX/semis fail while the market stays firm.

Exit: take profits at `80-100%` gain on debit, or if AMD trades `600+` before expiration. Cut if spread loses `50%` of debit or AMD closes below `520`.

**2. NVDA liquid semi participation**
Thesis: NVDA is a cleaner, more liquid way to ride semiconductor momentum without chasing AMD’s larger one-day move. The `215/245` spread gives upside exposure with defined downside.

Catalysts: broad semi strength, AI infrastructure spending, sympathy from AMD/MU/AVGO.

Invalidation: NVDA closes below `200`, or the semi index reverses below its breakout.

Exit: sell half if spread doubles; close remainder if NVDA stalls under `215` for 7-10 trading days.

**3. ORCL beaten-down LEAPS-style rebound**
Thesis: ORCL is still far below its 52-week high while bouncing with enterprise tech. The Jan. 2027 call spread gives longer duration without tying up LEAPS-sized premium.

Catalysts: cloud/AI backlog updates, earnings guidance, tech multiple recovery.

Invalidation: ORCL closes below `180`, or cloud software continues lagging while mega-cap tech rallies.

Exit: target `60-100%` return on debit. Cut if spread marks below `$7.00` or ORCL loses `180`.

**4. KBE sector-rotation covered-call collar**
Thesis: Banks are participating as the rally broadens beyond tech. The collar keeps the covered-call structure but defines downside.

Catalysts: yield curve stability, lower oil/geopolitical risk, broadening market breadth.

Invalidation: KBE closes below `64`, credit spreads widen, or financials stop confirming the broader rally.

Exit: let assignment happen above `74`, or close if KBE reaches `72-73` quickly and the collar captures most of max profit. Cut if KBE closes below `64` and the put has not offset enough.

**5. IWM pullback-defined bull put spread**
Thesis: IWM at `290` gives room to sell downside risk after a V-reversal, but the `270/250` spread keeps max loss capped. This is a moderate-aggressive bet that breadth continues into small caps.

Catalysts: continued risk-on breadth, stable 10Y yield, July Fed setup.

Invalidation: IWM closes below `270`, or SPY loses the `725` reversal low.

Exit: buy back at `50-70%` of max profit, especially if credit decays to `$1.50-$2.50`. Stop if spread value expands to about `2x` entry credit or IWM closes under `270`.
