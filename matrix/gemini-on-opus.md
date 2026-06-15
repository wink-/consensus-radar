# Prompt: gemini | Model: opus

Model: anthropic/claude-4.8-opus-20260528
Tokens: 485 in / 2854 out

# Options Strategy Brief — June 12, 2026

Before the trades, two framing notes worth your time:

1. **You're buying into a 4.4% two-day bounce with VIX collapsing.** Premium is getting cheaper, which favors *buying* optionality (LEAPS, debit spreads) over *selling* it. But it also means you're chasing—size accordingly and don't deploy all $50k on day one.

2. **All strikes/premiums below are estimates** based on the levels you gave. You must verify actual fills on Schwab/RH before executing. I'll flag where my assumptions matter most.

Total deployment target: **~$18,000–22,000 (35-44% of account)**. Keeping dry powder is the trade here, not a bug.

---

## 1. LEAPS — MSFT (Beaten-Down Quality)

**Strategy:** Long LEAPS call (stock replacement)

**Mechanics:**
- MSFT down 18% from high = quality name on sale, AI capex fears likely overdone
- Buy **Jan 2028 $400 call** (deep ITM, ~18+ months DTE)
- Assume MSFT ~$420; the $400 LEAPS runs ~$75–85 with ~0.70 delta
- **1 contract** (estimate cost ~$8,000)

⚠️ *This is your single largest line. If $8k is too concentrated, drop to the $440 strike (~$55, lower delta) or skip to a PMCC structure to cut basis.*

**Position Sizing:** 1 contract ≈ $8,000 (16% of account). This is the max I'd allow on one name.

**Risk/Reward:**
- Max loss: premium paid (~$8,000), but deep ITM = behaves like 70 shares
- Max profit: uncapped
- Breakeven: ~$483 at expiry (well below prior high)

**Thesis:** An 18% drawdown on a fortress-balance-sheet name during a sector-wide AI capex scare is exactly when you accumulate via LEAPS. The 0.70 delta gives you 70-share exposure for ~$8k vs ~$29k in stock, and 18 months removes timing risk. Sell short calls against it later to convert to a PMCC if it stalls.

---

## 2. High-Probability Momentum — IWM Bull Put Spread

**Strategy:** Credit put spread (selling premium into the strongest structure)

**Mechanics:**
- You said IWM has the *strongest structure*—lean into that with a defined-risk credit spread
- ~40–45 DTE (late July expiry)
- Assume IWM ~$235: **Sell $222 put / Buy $217 put** ($5 wide)
- Target credit ~$1.25–1.50, short strike ~25-30 delta
- **2 contracts**

**Position Sizing:** Max risk = ($5.00 − $1.40) × 100 × 2 = **$720** (1.4% of account)

**Risk/Reward:**
- Max loss: ~$720
- Max profit: ~$280 (credit collected)
- Breakeven: ~$220.60
- ~70% probability of profit at entry

**Thesis:** Small caps showing the best technical structure during the recovery means dip-buyers are defending. Selling puts below support monetizes the bounce and VIX decay without needing IWM to rip—you just need it to *not collapse*. High POP, capital-efficient.

---

## 3. Sector Rotation — XLK Call Debit Spread (Semis/Tech Recovery)

**Strategy:** Bull call debit spread

**Mechanics:**
- Semis bouncing + tech recovering = ride the rotation back into tech with capped cost
- ~45 DTE
- Assume XLK ~$285: **Buy $285 call / Sell $300 call** ($15 wide)
- Net debit ~$6.00
- **2 contracts**

⚠️ *Alternative: SMH (semis pure-play) if you want higher beta—but XLK is cleaner risk/reward for the rotation thesis.*

**Position Sizing:** Cost = $6.00 × 100 × 2 = **$1,200** (2.4% of account)

**Risk/Reward:**
- Max loss: $1,200
- Max profit: ($15 − $6) × 100 × 2 = **$1,800**
- Breakeven: $291
- 1.5:1 reward/risk

**Thesis:** Semis leading the bounce is the classic risk-on tell; tech recovering after a 5% drawdown with VIX falling supports continuation. A debit spread caps your cost and removes the need to pay up for crushing IV. You're buying the recovery, not chasing the top tick.

---

## 4. Opportunistic — QQQ Diagonal (Time-Spread Recovery Play)

**Strategy:** Call diagonal (long-dated long, short-dated short = poor man's covered call mechanics)

**Mechanics:**
- QQQ recovering at 717; structure to profit from grind-up + theta
- Buy **Sep 2026 $710 call** (~95 DTE), assume ~$28
- Sell **Jul 2026 $735 call** (~35 DTE), assume ~$6
- Net debit ~$22
- **1 contract**

**Position Sizing:** Cost ≈ **$2,200** (4.4% of account)

**Risk/Reward:**
- Max loss: ~$2,200 (if QQQ collapses)
- Max profit: maximized near $735 at front-month expiry; roll the short call monthly
- Breakeven: ~$732 (front leg), improves with each roll
- You're financing the long call by selling time

**Thesis:** QQQ in recovery mode but possibly choppy near term—a diagonal profits from upward drift while the short call decays faster. Roll the short strike up/out monthly to keep harvesting premium. This is your "grind higher, not vertical" expression.

---

## 5. Opportunistic — VIX Collapse Fade / SPY Protection Hedge

**Strategy:** SPY put debit spread (cheap insurance, NOT a directional short)

**Mechanics:**
- VIX at 18 falling = puts are getting cheap; this is your portfolio hedge against a failed bounce
- ~45 DTE
- Assume SPY ~$756: **Buy $735 put / Sell $710 put** ($25 wide)
- Net debit ~$5.00
- **2 contracts**

**Position Sizing:** Cost = $5.00 × 100 × 2 = **$1,000** (2% of account)

**Risk/Reward:**
- Max loss: $1,000
- Max profit: ($25 − $5) × 100 × 2 = **$4,000**
- Breakeven: $730

**Thesis:** You're net-long across trades 1–4 in a market that just snapped +4.4% off lows with a possibly-fragile recovery. A cheap put spread (financed by VIX being low) pays 4:1 if the 725 retest fails, and costs almost nothing if the bounce holds. This isn't a bet against the market—it's the insurance that lets you stay aggressive on the other four.

---

## Portfolio Summary

| # | Trade | Direction | Capital at Risk | % Account |
|---|-------|-----------|-----------------|-----------|
| 1 | MSFT LEAPS | Bullish | ~$8,000 | 16% |
| 2 | IWM put spread | Bullish | $720 | 1.4% |
| 3 | XLK call spread | Bullish | $1,200 | 2.4% |
| 4 | QQQ diagonal | Bullish drift | $2,200 | 4.4% |
| 5 | SPY put spread | Hedge | $1,000 | 2% |
| | **TOTAL** | Net long + hedge | **~$13,120** | **~26%** |

**Net deployment ~26%, leaving ~$37k dry.** That's intentional—you're chasing a bounce; if it pulls back to 725-730, you redeploy at better prices. If it rips, you're long enough to win.

---

**One honest caveat:** Every premium and strike above is my *estimate*. The MSFT LEAPS sizing in particular swings hard on actual IV. Pull up real chains before committing, and if any fill is materially worse than quoted here, ping me and we'll re-tune.

Want me to build the management rules (profit targets, roll triggers, stop levels) for each before you execute?