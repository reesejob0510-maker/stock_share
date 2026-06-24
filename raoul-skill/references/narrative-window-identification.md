# Narrative Window Identification

Use this file when determining which narrative is currently driving markets — macro vs fundamental, and the dominant crypto narrative.

---

## Why Narrative Windows Matter

Raoul Pal observes that the *framework* most relevant to investment decisions changes with the dominant market narrative.

- When markets are in **macro trading mode**: The GLI direction and central bank actions dominate. Company earnings, technology fundamentals, and valuations matter less. Use Raoul.skill.
- When markets are in **fundamental trading mode**: Company quality, earnings growth, and technology adoption matter. Macro provides a backdrop but not the primary driver. Use Buffett.skill, Serenity.skill, or Cathie.skill.
- In practice, most markets have **both simultaneously** — but one dominates, and identifying which is crucial for portfolio sizing and thesis confidence.

---

## Cross-Asset Correlation: The Primary Signal

**The diagnostic**: In macro trading mode, asset classes that normally have different drivers move together. Calculate rolling correlations:

| Pair | Normal correlation | Macro trading mode |
|---|---|---|
| S&P 500 and BTC | ~0.3 | > 0.6 |
| Gold and equities | ~0.1 | > 0.4 |
| EM equities and USD | ~-0.4 | < -0.6 (amplified) |
| US bonds and equities | ~-0.2 | Can flip positive |

**How to check**: Use TradingView or Bloomberg to plot 30-day rolling correlation between major asset classes. When correlations spike toward 1.0 (or -1.0 for inverse pairs), macro is dominating.

**Raoul's observation**: During major Fed tightening or easing cycles, cross-asset correlation converges. "Everything goes up" or "everything goes down" together. This is the GLI dominating.

---

## Macro Volatility Indicators

Secondary signals that indicate macro-driven markets:

- **VIX** (equity vol): > 25 sustained = elevated macro uncertainty; framework shifts to macro.
- **MOVE index** (bond vol): > 100 = significant rate market uncertainty; macro dominating.
- **Currency vol (CVIX)**: Elevated FX vol indicates macro regime shifts underway.
- **BTC realized vol correlation to SPX**: When BTC vol and SPX vol are highly correlated, macro is the primary driver for crypto too.

---

## The Macro Calendar as Narrative Anchor

Markets price and reprice macro narratives around specific scheduled events:

**Tier 1 events (highest market impact)**:
- FOMC meeting decisions + press conference.
- US CPI / PCE inflation prints.
- US Non-Farm Payrolls.
- Fed Chair speeches (Jackson Hole, Congressional testimony).

**Tier 2 events**:
- ECB/BOE/BOJ rate decisions.
- US quarterly earnings season (shifts narrative toward fundamentals).
- Quarterly Treasury Refunding Announcement (QRA).

**Narrative window timing**: In the ~2 weeks before a major FOMC meeting, markets typically shift to macro trading mode — prices are driven by expectations for the decision. After the meeting, if the result is as expected, the narrative can shift back to fundamentals.

---

## Crypto-Specific Narrative Windows

Crypto has three recurring narrative modes:

### 1. Liquidity Beta Narrative (most common)

**When it dominates**:
- BTC correlation with SPX and global risk assets is high (> 0.6).
- Funding rates react quickly to macro news (Fed announcements, risk-on/off days).
- "Bitcoin follows risk assets" is the dominant market commentary.

**Investment implication**: Raoul.skill and Arthur.skill are most applicable. Position based on GLI direction and funding rate structure.

**Typical timing**: Bear markets; early recovery phases; periods of macro uncertainty.

---

### 2. Technology / Adoption Narrative

**When it dominates**:
- BTC/ETH correlation with SPX declines.
- On-chain metrics (active addresses, transaction volumes, developer activity) drive price narrative.
- ETF approval discussions, DeFi usage, and Layer 2 adoption dominate news cycle.
- Institutional custody and corporate treasury adoption news.

**Investment implication**: Cathie.skill is most applicable for technology S-curve positioning. Raoul.skill still provides the macro tailwind/headwind.

**Typical timing**: After liquidity turns positive; mid-bull market; ETF approval cycles.

---

### 3. Regulatory / Event Narrative

**When it dominates**:
- Short-term price moves driven by regulatory announcements, enforcement actions, or legislative progress.
- SEC ETF decisions, CFTC jurisdiction rulings, Congressional hearings.
- Exchange collapses (FTX), stablecoin depegs, protocol hacks.

**Investment implication**: Short-term positioning. Macro and fundamental frameworks provide longer-term context but don't drive the immediate move.

**Raoul's view on regulation**: Regulatory clarity is ultimately bullish — it reduces uncertainty and opens the door to institutional capital. Short-term regulatory shocks are noise within the long-term adoption trend.

---

## Bitcoin Halving Narrative Window

The Bitcoin halving (every ~4 years, next approximately April 2028) has historically anchored a distinct narrative cycle:

- **Pre-halving accumulation** (~6–12 months before): Awareness builds; early positioning.
- **Post-halving supply shock** (~3–6 months after): Narrative of reduced sell pressure from miners.
- **Bull market peak** (~12–18 months post-halving): Historical pattern; retail FOMO + leverage buildup.

**Raoul's framework**: The halving cycle interacts with the GLI cycle. When halving coincides with GLI expansion (as in 2020), the result is amplified upside. When it coincides with GLI contraction, the supply shock is insufficient to overcome macro headwinds.

---

## Practical Narrative Window Assessment

For any current market question, run this three-step check:

**Step 1: Cross-asset correlation check**
- Are equities, bonds, gold, and crypto moving together (> 0.5 correlation)? → Macro narrative dominant.
- Are they diverging? → Fundamental narratives may be reasserting.

**Step 2: Recent catalyst identification**
- What was the last major price move? Was it driven by a macro event (Fed, CPI) or a crypto-specific event (ETF, protocol)?
- Macro event → confirms macro window. Crypto event → potential narrative shift to tech or regulatory.

**Step 3: Upcoming calendar events**
- Is an FOMC meeting within 3 weeks? → Pre-FOMC macro positioning likely.
- Is it earnings season? → Narrative may shift toward fundamentals.
- Is there a pending crypto regulatory decision? → Regulatory narrative window.

Output: state which narrative is dominant and which skill framework is most applicable.
