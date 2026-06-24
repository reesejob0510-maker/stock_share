# Evidence Ladder

Source grading for Hayes-style crypto macro research.

---

## Tier 1 — Authoritative (use to anchor all claims)

| Source | What it covers | URL |
|---|---|---|
| Federal Reserve H.4.1 | Fed balance sheet (weekly) | federalreserve.gov/releases/h41/ |
| NY Fed RRP data | Daily reverse repo balance | newyorkfed.org |
| US Treasury Fiscal Data | TGA balance (daily) | fiscaldata.treasury.gov |
| FRED (St. Louis Fed) | Aggregated macro data, M2, WALCL, RRPONTSYD | fred.stlouisfed.org |
| CME FedWatch Tool | Market-implied Fed rate probabilities | cmegroup.com/markets/interest-rates/cme-fedwatch-tool |
| FOMC statements | Official Fed guidance | federalreserve.gov/monetarypolicy/fomc.htm |
| BLS CPI/PCE | Inflation data | bls.gov, bea.gov |

---

## Tier 2 — Strong (institutional on-chain and derivatives data)

| Source | What it covers |
|---|---|
| Glassnode | On-chain analytics (BTC/ETH), funding rates, leverage ratio, realized cap |
| CryptoQuant | Exchange flows, miner behavior, estimated leverage ratio, exchange reserves |
| Coinglass | Live funding rates across exchanges, OI by exchange, liquidation data |
| DefiLlama | DeFi TVL, protocol-level lending rates, liquidation dashboards |
| Deribit | Options data: implied volatility, put/call ratio, max pain |
| CME futures basis | Institutional positioning in BTC/ETH futures |
| Nansen | On-chain wallet categorization (smart money, exchange wallets) |

---

## Tier 3 — Good (public commentary and secondary analysis)

| Source | What it covers |
|---|---|
| Arthur Hayes Substack (Maelstrom) | Hayes's public macro theses and analysis |
| BitMEX Research | Original research from the exchange's research arm |
| Real Vision | Macro interviews; Raoul Pal, other macro investors |
| Bloomberg / Reuters / WSJ | Market news; useful for event context |
| Messari / The Block | Crypto industry data, VC flows, on-chain metrics |
| CoinDesk | Industry news and regulatory developments |

**Usage**: Tier 3 sources provide context and narrative framing. Do not use them as primary evidence for quantitative claims (e.g., "funding rates are elevated") — verify those with Tier 1 or Tier 2.

---

## Tier 4 — Use with caution

| Source | Concern |
|---|---|
| Twitter / X crypto accounts | Unverified; often directionally biased |
| Reddit / Telegram price calls | No methodology; often noise |
| "On-chain analysts" without methodology | Verify claims against Tier 1–2 sources |
| YouTube crypto influencers | Potential conflicts of interest |
| Token project websites | Promotional material; treat as marketing |

---

## Evidence requirements by claim type

| Claim type | Minimum evidence required |
|---|---|
| USD liquidity direction | Tier 1 data (Fed H.4.1, TGA, RRP) + 4-week trend |
| Funding rate judgment | Tier 2 (Glassnode or Coinglass) + historical context |
| On-chain leverage risk | Tier 2 (DefiLlama liquidation + CryptoQuant leverage ratio) |
| Macro event impact | Tier 1 (official announcement) + Tier 3 for context |
| Cycle phase judgment | Tier 1 + Tier 2 + historical precedent from Tier 3 |

---

## Data freshness requirements

| Data type | Maximum acceptable lag |
|---|---|
| TGA balance | 1 day (daily data) |
| RRP balance | 1 day (daily data) |
| Fed balance sheet | 1 week (weekly data) |
| Funding rates | 4 hours (changes rapidly) |
| On-chain liquidation levels | 1 day |
| DeFi lending rates | 1 day |
| M2 data | 1 month (monthly release) |

**Note on stale data**: Always check the data freshness. "Current" funding rate from a week ago is meaningless. If live tools are not available, explicitly state "based on data last verified on [date]" and recommend the user check the live source.

---

## When to say "I don't know"

The following require live data that may not be available:

- Current TGA level (changes daily).
- Current funding rates (change every 8 hours).
- Current on-chain liquidation levels (change with price).
- Current FOMC decision (cannot be inferred).

When live data is unavailable, provide:
1. The framework for interpreting the data once the user checks.
2. The exact URL to find the relevant data point.
3. The threshold that would change the conclusion.
