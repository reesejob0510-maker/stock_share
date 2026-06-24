# USD Liquidity Framework

Use this file when diagnosing the net direction of US dollar liquidity — the primary macro driver in Hayes's framework.

> *"Bitcoin is a high-beta call option on global liquidity. When the dollar printing press runs hot, Bitcoin goes up. When it runs cold, Bitcoin goes down. Everything else is noise."* — Arthur Hayes (paraphrased from public essays)

---

## The Three-Component Model

**Net USD Liquidity = Fed Assets + TGA Drawdown − Reverse Repo Balance**

All three are publicly observable. The direction of each component, and their combined force, determines the net liquidity environment for risk assets.

---

## Component 1: Federal Reserve Balance Sheet

**What it measures**: Total assets held by the Federal Reserve. Expansion = money creation (QE). Contraction = money destruction (QT).

**Why it matters for crypto**: QE injects reserves into the banking system, which flows into risk assets. QT drains reserves, tightening financial conditions.

**Key modes**:
| Mode | Description | Crypto implication |
|---|---|---|
| **QE (quantitative easing)** | Fed buying bonds; balance sheet expanding | Strongly bullish |
| **Taper** | QE slowing but still positive | Moderately bullish; watch pace |
| **Pause** | Balance sheet flat | Neutral; other components matter more |
| **QT (quantitative tightening)** | Fed selling or not reinvesting; balance sheet shrinking | Bearish; rate matters |
| **QT slowdown / pause** | QT pace decreasing | Turning point; watch for reversal |
| **Emergency facilities** | BTFP, repo facilities activated | Bullish (liquidity injection) |

**Data source**: Federal Reserve H.4.1 Statistical Release (weekly, Thursday). federalreserve.gov/releases/h41/

**Key metrics to track**:
- Total assets (all Federal Reserve banks).
- Securities held outright (Treasuries + MBS).
- Week-over-week change.
- Year-over-year change.

---

## Component 2: Treasury General Account (TGA)

**What it measures**: The US government's operating account at the Federal Reserve. It holds tax receipts and bond issuance proceeds.

**Why it matters**: When TGA falls (government spending or inability to issue new debt), money flows INTO the private sector → bullish. When TGA rises (government issuing new debt and accumulating cash), money is DRAINED from the private sector → bearish.

**The debt ceiling dynamic** (highly relevant for timing):

| Phase | What happens | Liquidity effect |
|---|---|---|
| **Debt ceiling binding** | Treasury cannot issue new debt; must drawdown TGA | TGA falls → bullish |
| **Debt ceiling suspension/raise** | Treasury can issue debt again; TGA rebuilds | TGA rises → bearish (short-term) |
| **Post-rebuild normalization** | TGA stabilizes; spending resumes | Returns to neutral |

**The "refill and drain" cycle**: After each debt ceiling resolution, Treasury refills TGA → temporary bearish. Then resumes normal spending → gradual drain → neutral to bullish.

**Data source**: US Treasury Fiscal Data (daily). fiscaldata.treasury.gov → "Treasury Balance" or "Daily Treasury Statement."

**Key metrics**:
- Daily TGA balance.
- 4-week change (is it rising or falling?).
- Level vs historical norm (~$500B "target" balance).

---

## Component 3: Reverse Repo (RRP)

**What it measures**: Money market funds and banks park idle cash at the Fed overnight via the reverse repo facility. High RRP = cash sitting idle, not in the financial system. Falling RRP = cash flowing back into financial system.

**Why it matters**: When RRP falls, the cash that was parked at the Fed flows into money markets, bank reserves, and risk assets. This is a liquidity injection into the private financial system without any Fed action.

**Key dynamics**:
- 2021–2022: RRP rose to ~$2.6 trillion (idle cash from COVID stimulus parked at Fed).
- 2023–2024: RRP declined as short-term yields fell below the RRP rate, causing money to flow back out.
- When RRP approaches zero, this liquidity source is exhausted.

**Data source**: NY Federal Reserve daily RRP data. newyorkfed.org → Markets → Repo and Reverse Repo Agreements.

**Key metrics**:
- Daily RRP balance.
- 4-week change.
- Is it declining (bullish) or rising (bearish)?
- How close to zero? (Approaching zero = RRP tailwind exhausted)

---

## The Combined Signal

### How to synthesize

Run each component through the directional check:

| Component | Bullish signal | Bearish signal |
|---|---|---|
| Fed balance sheet | Expanding or pause from QT | Active QT |
| TGA | Falling (drawdown) | Rising (rebuild) |
| RRP | Falling (cash returning to system) | Rising (cash leaving system) |

**Net liquidity judgment**:
- 3/3 bullish → strong positive environment for risk assets
- 2/3 bullish → moderate positive
- 1/3 bullish → neutral / slight positive
- 0/3 bullish or 2/3 bearish → negative environment
- 3/3 bearish → strong negative environment

### The nuance: rate of change > level

Hayes consistently emphasizes *change* over level. A tightening that is slowing is more bullish than a tightening that is accelerating, even if the absolute level is still tightening.

> "It doesn't matter that the Fed is hiking — what matters is whether the market believes the hiking cycle is ending."

---

## Global Dollar Liquidity Extension

For a broader view, Hayes sometimes incorporates:

**Dollar strength (DXY)**:
- Strong USD = tighter global dollar liquidity (dollar-denominated debt becomes more expensive).
- Weak USD = looser global dollar liquidity.
- DXY turning down is a crypto-positive signal beyond the three components.

**Eurodollar system**:
- Cross-border USD lending, FX swap lines, offshore dollar creation.
- Tightening in the offshore dollar market (repo rates spiking, swap basis widening) signals global dollar stress → risk-off for crypto.
- Sources: BIS quarterly review, FX swap basis spreads (Bloomberg).

**China PBOC stimulus**:
- While not USD liquidity, large PBOC stimulus can substitute as global risk-on fuel.
- Relevant: 2023 "China reopening" provided a risk-on impulse even as Fed tightened.

---

## Quick Reference: Data Lookup Paths

| Data | Source | Update frequency |
|---|---|---|
| Fed balance sheet | federalreserve.gov/releases/h41/ | Weekly (Thursday) |
| TGA balance | fiscaldata.treasury.gov | Daily |
| NY Fed RRP | newyorkfed.org/markets | Daily |
| DXY index | Bloomberg, TradingView, Investing.com | Real-time |
| FRED (all combined) | fred.stlouisfed.org | Various |
| WALCL (Fed assets) | FRED: WALCL | Weekly |
| TGA on FRED | FRED: WDTGAL | Weekly |
| RRP on FRED | FRED: RRPONTSYD | Daily |
