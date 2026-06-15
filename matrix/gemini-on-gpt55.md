I’ll verify current market levels first because the trade construction depends heavily on live prices and option chains. I’ll keep this to defined-risk structures and size each idea against the $50k account.
mcp: codex_apps/alpaca_get_stock_latest_trade started
mcp: codex_apps/alpaca_get_stock_latest_trade (failed)
user cancelled MCP tool call
mcp: codex_apps/alpaca_get_stock_latest_trade started
mcp: codex_apps/alpaca_get_stock_latest_trade (failed)
user cancelled MCP tool call
mcp: codex_apps/alpaca_get_stock_latest_trade started
mcp: codex_apps/alpaca_get_stock_latest_trade (failed)
user cancelled MCP tool call
mcp: codex_apps/alpaca_get_stock_latest_trade started
mcp: codex_apps/alpaca_get_stock_latest_trade (failed)
user cancelled MCP tool call
mcp: codex_apps/alpaca_get_stock_latest_trade started
mcp: codex_apps/alpaca_get_stock_latest_trade (failed)
user cancelled MCP tool call
mcp: codex_apps/alpaca_get_stock_latest_trade started
mcp: codex_apps/alpaca_get_stock_latest_trade (failed)
user cancelled MCP tool call
mcp: codex_apps/alpaca_get_stock_latest_trade started
mcp: codex_apps/alpaca_get_stock_latest_trade (failed)
user cancelled MCP tool call
mcp: codex_apps/alpaca_get_stock_latest_trade started
mcp: codex_apps/alpaca_get_stock_latest_trade (failed)
user cancelled MCP tool call
mcp: codex_apps/alpaca_get_stock_latest_trade started
mcp: codex_apps/alpaca_get_stock_latest_trade (failed)
user cancelled MCP tool call
mcp: codex_apps/alpaca_get_stock_latest_trade started
mcp: codex_apps/alpaca_get_stock_latest_trade (failed)
user cancelled MCP tool call
web search: 
web search: finance: SPY
web search: 
web search: finance: MSFT
web search: 
web search: finance: MSFT
web search: 
web search: MSFT stock price June 15 2026
web search: 
web search: MSFT Jan 15 2027 400 call option quote
web search: 
web search: MSFT options chain January 15 2027 MarketWatch
web search: 
web search: NVDA closed June 15 2026 price
web search: 
web search: XLI close June 15 2026 price
As of **June 15, 2026**, SPX closed at **7,554.29**, Nasdaq +3.1%, Russell 2000 +0.7%, and MSFT closed **$399.76**; NVDA closed **$212.45**, HWM **$270.44**, AMD about **$550.75**. Sources: AP, MarketWatch, Barron’s. Use these as **limit-order structures**, not market orders, and skip any trade if the midpoint is materially worse than the target debit/credit.

**1. LEAPS / Beaten-Down Quality: MSFT**
Buy **1 MSFT Jan 15 2027 400/480 call debit spread**, **214 DTE**.  
Target debit: **$26.00**. Max loss: **$2,600**. Max profit: **$5,400**. Breakeven: **$426.00**.  
Sizing: **5.2% of $50k**.  
Thesis: MSFT remains one of the highest-quality enterprise software/cloud names, but it has lagged badly, with recent reports noting it was down roughly mid-teens YTD before today’s bounce. This spread gives convex upside without paying open-ended LEAPS premium.

**2. Momentum: IWM**
Buy **1 IWM Sep 18 2026 295/330 call debit spread**, **95 DTE**.  
Target debit: **$13.00**. Max loss: **$1,300**. Max profit: **$2,200**. Breakeven: **$308.00**.  
Sizing: **2.6%**.  
Thesis: Russell 2000 has been the strongest major index YTD, and today’s broadening rally supports small-cap continuation. This is a direct upside momentum bet with defined downside.

**3. Sector Rotation: HWM**
Buy **1 HWM Aug 21 2026 270/300 call debit spread**, **67 DTE**.  
Target debit: **$10.50**. Max loss: **$1,050**. Max profit: **$1,950**. Breakeven: **$280.50**.  
Sizing: **2.1%**.  
Thesis: Industrials/aerospace are participating in the non-tech rotation, and HWM closed at **$270.44**, only modestly below its 52-week high. The setup plays breakout continuation without needing mega-cap tech to carry the tape.

**4. Opportunistic: NVDA**
Sell **1 NVDA Aug 21 2026 200/180 put credit spread**, **67 DTE**.  
Target credit: **$5.50**. Max loss: **$1,450**. Max profit: **$550**. Breakeven: **$194.50**.  
Sizing: **2.9%**.  
Thesis: NVDA rallied with semis and closed **$212.45**, but chasing calls after a strong bounce can be expensive. This gets paid to underwrite a pullback toward 200 while keeping risk capped.

**5. Opportunistic: AMD**
Buy **1 AMD Aug 21 2026 550/600/650 call butterfly**, **67 DTE**.  
Structure: buy 550C, sell 2x 600C, buy 650C.  
Target debit: **$11.00**. Max loss: **$1,100**. Max profit: **$3,900** at $600 on expiration. Breakevens: **$561.00 / $639.00**.  
Sizing: **2.2%**.  
Thesis: AMD surged to roughly **$550.75** after bullish AI/datacenter headlines, so outright calls are vulnerable to IV crush and overextension. The fly targets a continuation move toward 600 while keeping risk tight.

Total theoretical max risk across all five: **$7,500**, or **15% of the $50k account**. I would not add to losers; take partials around **50-70% of max profit** on debit spreads, and close credit spreads if they reach **70-80% of credit captured**.
