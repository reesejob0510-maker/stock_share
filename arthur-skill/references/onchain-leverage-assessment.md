# On-Chain Leverage Assessment

Use this file when assessing whether the DeFi and on-chain system carries dangerous leverage that amplifies price risk.

---

## Why On-Chain Leverage Matters to Hayes

Arthur Hayes views on-chain leverage as the mechanism that amplifies crypto price moves in both directions. When leverage is low and well-distributed, the system is resilient. When leverage is concentrated near current prices, a modest price decline triggers cascading liquidations that push prices much lower than fundamentals would imply.

> *"DeFi is a beautiful machine for amplifying greed and fear. When everyone is levered long on-chain, the liquidation cascade can turn a 10% dip into a 40% crash."* — Hayes (paraphrased from public writing)

---

## Key Metrics and Assessment Framework

### 1. DeFi Lending Protocol Rates

**What it measures**: The annualized borrow rate for stablecoins (USDC, DAI, USDT) on major lending protocols (AAVE, Compound, MakerDAO).

**Why it matters**: When demand to borrow stablecoins is high, it means traders are borrowing stables to buy more crypto (leveraged long). High stablecoin borrow rates = high on-chain leverage demand.

**Interpretation**:
| Annualized USDC borrow rate | Leverage condition |
|---|---|
| < 3% | Very low demand for leverage; system unleveraged |
| 3% – 8% | Normal; moderate demand |
| 8% – 15% | Elevated; leverage building |
| > 15% | High leverage demand; systemic risk increasing |
| > 30% | Extreme; similar to pre-LUNA/pre-FTX conditions |

**Sources**: AAVE (app.aave.com → Markets), Compound (compound.finance), MakerDAO (makerburn.com), DefiLlama (defillama.com/yields).

---

### 2. Liquidation Level Density

**What it measures**: The concentration of collateralized loan liquidation thresholds relative to the current price of BTC or ETH.

**Why it matters**: If a large volume of loans will be liquidated if BTC falls 5%, then a 5% price drop will trigger forced selling of BTC collateral, which pushes price lower, triggering more liquidations — a cascade.

**Assessment levels**:
- **Safe** (>15% distance): Most liquidation walls are far from current price. Small price moves don't trigger cascades.
- **Elevated** (5–15% distance): Meaningful liquidation volume within range. A correction could accelerate.
- **Dangerous** (<5% distance): Large liquidation walls very close. Any dip risks amplified selling.

**How to check**:
1. DefiLlama liquidation dashboard (defillama.com/liquidations) — aggregates AAVE, Compound, MakerDAO, and Venus.
2. Glassnode "Liquidation Level" metric for exchange leverage.
3. Loanscan or Debank for individual large positions.

**Key interpretation**: Identify the price at which the largest "liquidation wall" is hit. Calculate % distance from current price.

---

### 3. MakerDAO / AAVE Health Factor Distribution

**What it measures**: For AAVE specifically, the "health factor" of loans. A health factor of 1.0 = the loan is at the liquidation threshold. Health factor < 1.0 = liquidated.

**Risk interpretation**:
- What % of total AAVE collateral value is held by positions with health factor < 1.5?
- A high concentration of health factors between 1.0 and 1.5 means a moderate price drop would trigger a wave of liquidations.

**Sources**: AAVE risk dashboard, DeBank, Dune Analytics (custom queries).

---

### 4. Exchange Leverage Ratio (CryptoQuant)

**What it measures**: CryptoQuant's "Estimated Leverage Ratio" = Open Interest / Coin Reserve on exchange. Higher ratio = more OI relative to the actual coins available, implying higher leverage.

**Historical context**:
- Leverage ratio peaks have historically preceded major corrections in both directions.
- BTC estimated leverage ratio > 0.2 = elevated; > 0.3 = high risk.

**Sources**: CryptoQuant (cryptoquant.com → Exchange → Estimated Leverage Ratio).

---

### 5. Stablecoin Peg Stability

**What it measures**: Whether major algorithmic or overcollateralized stablecoins are maintaining their peg.

**Relevance**: Stablecoin depeg events are early warning signals for systemic stress. When DAI, FRAX, or USDT shows peg pressure, it indicates either:
- Rush for collateral redemption (deleveraging pressure).
- Confidence loss in the DeFi collateral stack.

**Historical examples**: UST depeg (May 2022) triggered a $500B+ market cap collapse. Monitoring this is critical during leverage buildups.

**Sources**: CoinGecko (stablecoin peg monitor), Curve 3pool balance (when unbalanced, indicates USDT/USDC/DAI stress).

---

## Composite Leverage Risk Score

Run each metric through the risk assessment:

| Metric | Low risk | Medium risk | High risk |
|---|---|---|---|
| Stablecoin borrow rate | < 5% | 5%–15% | > 15% |
| Nearest liquidation wall distance (BTC) | > 15% | 5%–15% | < 5% |
| AAVE health factor < 1.5 (as % of TVL) | < 5% | 5%–15% | > 15% |
| Exchange leverage ratio | < 0.15 | 0.15–0.25 | > 0.25 |
| Stablecoin peg stability | All at par | Minor depeg (< 0.5%) | Significant depeg |

**Score**:
- 4–5 low: System unleveraged; safe to add exposure if macro is positive.
- 2–3 low: Moderate leverage; exercise normal caution.
- 3+ medium or any high: Elevated systemic risk; reduce size or avoid adding leverage.
- 2+ high: Dangerous; risk of cascade if price moves adversely.

---

## Cross-Referencing with Macro

On-chain leverage assessment must be paired with the USD liquidity framework:

| USD Liquidity | On-chain leverage | Recommended posture |
|---|---|---|
| Positive | Low | Accumulate aggressively; best setup |
| Positive | High | Accumulate with smaller size; set stop below nearest liquidation wall |
| Neutral | Low | Hold; wait for liquidity direction |
| Neutral | High | Reduce leverage; take partial profits |
| Negative | Any | Defensive; reduce all leveraged exposure |
| Negative | High | Maximum caution; risk of cascade drawdown |
