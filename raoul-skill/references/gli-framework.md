# Global Liquidity Index (GLI) Framework

Use this file when assessing the global liquidity cycle — the primary macro driver in Raoul Pal's framework.

> *"Global liquidity is the mother of all markets. When the world's central banks are all printing, everything goes up. When they all tighten, everything goes down. Bitcoin is just the most sensitive instrument to that tide."* — Raoul Pal (paraphrased from public interviews)

---

## What is the GLI?

The Global Liquidity Index (GLI) is Raoul Pal's term for the combined force of major central bank balance sheet expansion and M2 growth across the world's largest economies.

**Conceptual formula**:
> GLI = f(Fed balance sheet, ECB balance sheet, BOJ balance sheet, PBOC balance sheet, BOE balance sheet, Global M2)

In practice, Raoul weights the components by economic size and uses proprietary smoothing. The public methodology uses a simpler version:
- Count how many major CBs are expanding vs contracting.
- Track global M2 in USD terms (major CBs combined).
- Track the credit impulse (rate of change of new credit as % of GDP).

**⚠️ Methodology note**: Raoul's actual GLI construction is proprietary to GMI. The above is a public approximation. Outputs should be labeled "framework interpretation" when using this proxy.

---

## The Four GLI Phases

### Phase 1: GLI Expansion

**Characteristics**:
- Multiple major CBs expanding balance sheets simultaneously.
- Global M2 in USD terms accelerating.
- Credit impulse turning positive.
- Real interest rates negative or declining toward negative.

**Triggers for expansion**:
- Global recession or financial crisis forces coordinated CB easing.
- Inflation below target allows easing without political resistance.
- Currency wars: competitive devaluation by one CB forces others to respond.
- Debt servicing stress: CB must monetize to prevent sovereign debt crisis.

**Cross-asset implications**:
- Equities: broadly up; quality growth leads.
- Bonds: rally in early expansion (as rates cut); later underperform as growth returns.
- Gold: strong; real rate suppression is the primary driver.
- Bitcoin / crypto: highest beta; BTC often leads by 3–6 months.
- USD: weakens in expansion (more supply, risk-on flows to EM).

**Investment framing** (Raoul): "The tide is rising. Own the highest-beta instruments to global liquidity."

---

### Phase 2: GLI Peak / Plateau

**Characteristics**:
- Rate of expansion slowing; not yet contracting.
- Inflation rising; CB rhetoric shifting hawkish.
- Credit impulse flattening.
- Lagging assets (altcoins, EM, commodities) often have their biggest moves in this phase.

**Cross-asset implications**:
- Late-cycle signals. Value and commodity names catch up.
- Crypto: altcoin season; leverage builds; risk rising.
- Bonds: underperform; inflation eroding real returns.
- Gold: holds as inflation hedge.

**Investment framing**: "The peak is forming. Reduce leverage. Watch for the credit impulse rollover."

---

### Phase 3: GLI Contraction

**Characteristics**:
- CBs tightening (rate hikes + balance sheet reduction).
- Global M2 flat or declining.
- Credit impulse negative: credit conditions tightening.
- Real interest rates rising.

**Cross-asset implications**:
- Equities: de-rate; high-multiple growth names fall hardest.
- Bonds: initially rise as growth slows; then under pressure as inflation persists.
- Gold: mixed; strong if inflation stays elevated; weak if real rates rise sharply.
- Bitcoin / crypto: severe drawdown; high beta amplifies contraction.
- USD: strengthens (tighter liquidity, risk-off flows from EM).

**Investment framing**: "Contraction is painful. Capital preservation. Watch for the monetary policy pivot signal."

---

### Phase 4: GLI Trough / Pre-Expansion

**Characteristics**:
- CB tightening cycle ending; pivot signals emerging.
- Credit impulse bottoming and beginning to turn positive.
- Asset prices have already discounted most of the bad news.
- Leading indicators (ISM, PMI, housing) turning.

**Cross-asset implications**:
- The best long-term entry point for risk assets, especially high-beta.
- Bitcoin historically bottoms 6–12 months before GLI confirmed expansion.
- Gold: accumulate.
- Equities: begin building positions in quality growth.

**Investment framing**: "The trough is forming — or forming soon. Position for the next expansion cycle. BTC is the highest-conviction long-cycle bet."

---

## Credit Impulse — The Leading Indicator

The credit impulse measures the *change in new credit* as a % of GDP. It is a leading indicator for both economic activity and asset prices.

- **Positive and rising**: expansionary; leads GDP growth by ~9–12 months.
- **Positive and falling**: growth is still positive but decelerating.
- **Negative**: credit conditions contracting; leads slowdown.
- **Negative and turning**: trough; recovery signal.

**Why Raoul watches it**: Credit impulse often turns positive before the CB officially pivots — because commercial bank lending responds to the *expectation* of easier policy, not just the policy itself.

**Data source**: BIS credit-to-GDP data, FRED (private credit creation), China credit data (PBOC), ECB.

---

## Global M2 in USD Terms

A key shortcut: sum the M2 of major economies, converted to USD using spot exchange rates. When global M2 in USD terms is rising, liquidity is expanding globally. When falling, contracting.

**Composition** (approximate weight):
- US M2: ~35%
- Eurozone M2: ~25%
- China M2: ~20%
- Japan M2: ~10%
- Other (UK, Canada, Australia, EM): ~10%

**Data sources**:
- US M2: FRED (M2SL).
- Eurozone M2: ECB statistical data warehouse.
- China M2: PBOC statistics portal (人民银行 M2).
- Japan M2: BOJ statistics.
- Aggregate: Refinitiv/Bloomberg aggregation tools; or manual construction.

**Key signal**: Global M2 in USD terms tends to lead crypto market caps by 6–12 months with high correlation. When Raoul says "follow the M2," this is the data he refers to.

---

## BOJ — The Special Case

The Bank of Japan occupies a unique position in the GLI framework:

- BOJ has maintained ultra-loose policy (YCC — Yield Curve Control) for decades.
- Yen weakness from BOJ easing creates "yen carry trade": borrow in cheap yen, buy risk assets globally.
- When BOJ tightens (YCC adjustment): yen strengthens → carry trade unwinds → global risk-off.
- When BOJ eases further: yen weakens → carry trade expands → global liquidity tailwind.

**Raoul's specific watch**: BOJ policy changes are disproportionately impactful on global risk assets relative to Japan's economic size, because of the carry trade mechanism.

**Data source**: BOJ policy rate decisions, BOJ balance sheet (boj.or.jp), USDJPY exchange rate as proxy.

---

## GLI Quick Assessment Checklist

For a rapid GLI judgment, check:

- [ ] Fed: expanding, flat, or contracting?
- [ ] ECB: expanding, flat, or contracting?
- [ ] BOJ: tightening (yen carry unwind risk) or maintaining loose policy?
- [ ] PBOC: stimulating (rate cuts, RRR cuts, credit guidance) or restraining?
- [ ] Global M2 in USD: rising or falling YoY?
- [ ] Credit impulse: positive and rising / positive and falling / negative / bottoming?
- [ ] Count: how many of the 4 major CBs are net-positive to liquidity?

**Score**:
- 4/4 bullish → Strong GLI Expansion
- 3/4 bullish → Moderate GLI Expansion
- 2/4 → Neutral / Mixed
- 1/4 → Moderate GLI Contraction
- 0/4 → Strong GLI Contraction
