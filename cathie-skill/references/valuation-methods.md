# Valuation Methods

Use this file when estimating the 5-year value of an innovation company.

> ARK Invest's primary valuation framework centers on 5-year price targets derived from TAM scenarios and expected market share capture. These are not DCF models — they are scenario-based equity value estimates at a future point in time, discounted back to today.

---

## Guiding principles

1. **Value at convergence, not today**: Innovation companies look expensive on today's metrics. The question is whether the 5-year value justifies the current price.
2. **TAM is the future market, not today's market**: Cost declines create demand that does not exist today. The TAM at convergence is usually 3–10× the current addressable market.
3. **Scenarios, not point estimates**: Innovation timelines are uncertain. Always run bear / base / bull scenarios.
4. **Risk-adjust for technology and adoption uncertainty**: Pre-revenue or early-revenue companies require higher return requirements and wider scenario ranges.
5. **Do not use traditional PE or DCF for pre-FCF innovation companies**: These methods require earnings that do not yet exist. Use TAM-based scenario valuation.

---

## Method 1 — 5-Year TAM Scenario (ARK's primary method)

### Step 1: Define the convergence TAM

- Identify the total addressable population or use case.
- Estimate penetration at convergence (5 years, not full saturation).
- Estimate revenue or value per unit at convergence costs (not today's pricing).
- TAM = addressable population × penetration % × revenue per unit at convergence costs.

**Example — EV battery**:
- Global light vehicle production: ~90M units/year.
- EV penetration in 5 years: base case 40%.
- Battery content per vehicle at convergence pricing: $5,000.
- Battery TAM at convergence: 90M × 40% × $5,000 = $180B.

### Step 2: Estimate addressable market share

- What share of the convergence TAM can the target company capture?
- Rank by: cost curve leadership, IP/patent, production scale, go-to-market, regulatory position.
- Use comparable technology adoption cases for calibration.

### Step 3: Apply a revenue multiple

- For companies approaching FCF: use 5-year EV/Revenue or EV/EBITDA comparable to established peers in adjacent sectors.
- For pre-FCF companies: use EV/Revenue and flag the uncertainty.
- Apply a discounting factor for the 5-year time horizon (typically 10–15% annual discount).

### Step 4: Derive implied equity value

- Equity value in 5 years = TAM × market share % × revenue multiple.
- Discount back: Current fair value = 5-year equity value / (1 + discount rate)^5.
- Compare to current market cap to assess upside / downside.

### Step 5: Build three scenarios

| Scenario | Assumption | Probability weight |
|---|---|---|
| **Bear** | Slow adoption; cost curve stalls; competition intensifies | 25% |
| **Base** | Wright's Law holds; penetration reaches projected level | 50% |
| **Bull** | Faster adoption; additional use cases unlock; winner-takes-most | 25% |

Probability-weighted fair value = (Bear × 0.25) + (Base × 0.50) + (Bull × 0.25)

---

## Method 2 — Reverse DCF (for companies approaching FCF)

Use when the company is generating or approaching positive FCF.

**Goal**: Instead of projecting cash flows forward, find the growth rate implied by the current stock price, then judge whether that growth rate is reasonable.

**Steps**:
1. Estimate current revenue and FCF margin trajectory.
2. At the current stock price, what revenue growth rate over 5–10 years produces a DCF value equal to the current price (at 10% discount rate)?
3. Is that implied growth rate consistent with the S-curve position and TAM analysis?
4. If the implied growth rate is much lower than the evidence supports → cheap signal.
5. If the implied growth rate is much higher than evidence supports → expensive signal.

**Plain-language framing**:
- "At $X per share, the market implies X% annual revenue growth for 10 years. Given the S-curve position and TAM, that seems [conservative / reasonable / aggressive]."

---

## Method 3 — Cost Per Unit Threshold Valuation

Use for companies whose value is directly tied to a cost threshold being crossed.

**Logic**: When a cost threshold is crossed, a new use case opens and the addressable market expands step-function. The company's revenue opportunity changes qualitatively, not just quantitatively.

**Application**:
- Identify the next cost threshold for the technology (e.g., $60/kWh battery, $10 genome).
- Estimate the revenue opportunity unlocked at that threshold.
- Estimate when the threshold is crossed (Wright's Law projection).
- Value the option: what is the probability-weighted value of that revenue opportunity, discounted to today?

---

## Valuation red flags for innovation companies

| Signal | Implication |
|---|---|
| Stock price up 10× with no change in cost curve or penetration data | Narrative premium; high risk of de-rating |
| Revenue growing but unit economics deteriorating | Scaling is not producing cost learning; Wright's Law may not apply |
| TAM estimate based on today's pricing, not convergence pricing | TAM underestimated; also the company is pricing itself out of mass adoption |
| 5-year price target assumes 80%+ market share | Implausible in competitive markets; winner-takes-most is rare outside platforms |
| Pre-revenue company with $50B+ market cap | Requires near-perfect execution; extreme scenario sensitivity |
| Capital requirements exceed current cash + expected revenue for 3 years | Dilution risk; financing dependency is existential |

---

## A-share Innovation Valuation Adjustments

For A-share listed innovation companies, additional factors:

- **Policy premium / discount**: Government industrial policy (e.g., NEV subsidies, Made in China 2025) can accelerate or distort adoption curves. Separate policy-driven adoption from organic market adoption.
- **Subsidy cliff risk**: Many A-share EV and solar companies benefited from subsidies. Track subsidy phase-out schedules and test whether unit economics hold without subsidies.
- **VIE / dual-class structure**: For tech companies, understand governance and whether innovation IP is held in listed entity or related parties.
- **Localization tailwind**: Domestic substitution (国产替代) can add a market share tailwind not present in global comps. Quantify separately.
