# Market Source Playbook

Quick reference for finding data across different markets and data types.

---

## Macro / USD Liquidity

| Data needed | Source | Path |
|---|---|---|
| Fed balance sheet (weekly) | Federal Reserve | federalreserve.gov/releases/h41/ |
| WALCL (Fed total assets, FRED) | FRED | fred.stlouisfed.org/series/WALCL |
| TGA balance | US Treasury | fiscaldata.treasury.gov → Daily Treasury Statement |
| WDTGAL (TGA on FRED) | FRED | fred.stlouisfed.org/series/WDTGAL |
| NY Fed daily RRP | NY Fed | newyorkfed.org/markets/desk-operations/repo-reverse-repo |
| RRPONTSYD (RRP on FRED) | FRED | fred.stlouisfed.org/series/RRPONTSYD |
| DXY (dollar index) | TradingView | tradingview.com → DXY |
| US M2 | FRED | fred.stlouisfed.org/series/M2SL |
| FOMC calendar | Federal Reserve | federalreserve.gov/monetarypolicy/fomccalendars.htm |
| CME FedWatch (rate probabilities) | CME Group | cmegroup.com/markets/interest-rates/cme-fedwatch-tool |
| US CPI | BLS | bls.gov/cpi/ |
| US PCE | BEA | bea.gov → Personal Income |
| US NFP | BLS | bls.gov/emp/ |
| QRA announcement | US Treasury | home.treasury.gov → Debt Management → Quarterly Refunding |

---

## Crypto Derivatives and Positioning

| Data needed | Source | Path |
|---|---|---|
| BTC/ETH funding rates (aggregated) | Coinglass | coinglass.com/funding |
| Funding rate history (Glassnode) | Glassnode | glassnode.com → Derivatives → Funding Rates |
| Open Interest by exchange | Coinglass | coinglass.com/open-interest |
| OI history (Glassnode) | Glassnode | glassnode.com → Derivatives → Open Interest |
| Estimated leverage ratio | CryptoQuant | cryptoquant.com → Market Data → Estimated Leverage Ratio |
| CME BTC futures basis | CME | cmegroup.com → Bitcoin Futures |
| Options implied volatility | Deribit | deribit.com → BTC Options |
| Options put/call ratio | Glassnode | glassnode.com → Derivatives → Put/Call Ratio |

---

## On-Chain Leverage and DeFi

| Data needed | Source | Path |
|---|---|---|
| AAVE lending rates | AAVE app | app.aave.com → Markets |
| Compound lending rates | Compound | compound.finance → Markets |
| DeFi yields (aggregated) | DefiLlama | defillama.com/yields |
| Liquidation dashboard | DefiLlama | defillama.com/liquidations |
| Total DeFi TVL | DefiLlama | defillama.com |
| Curve 3pool balance (stablecoin stress) | Curve | curve.fi/#/ethereum/pools/3pool/deposit |
| Stablecoin peg monitor | CoinGecko | coingecko.com → Stablecoins |
| Large AAVE positions | DeBank | debank.com |
| Dune Analytics (custom on-chain) | Dune | dune.com |
| Nansen (smart money on-chain) | Nansen | nansen.ai |

---

## BTC / ETH On-Chain

| Data needed | Source | Path |
|---|---|---|
| BTC realized cap | Glassnode | glassnode.com → Market Indicators → Realized Cap |
| MVRV ratio | Glassnode | glassnode.com → Market Indicators → MVRV Ratio |
| Exchange inflows/outflows | Glassnode / CryptoQuant | Both provide exchange flow data |
| BTC long-term holder supply | Glassnode | glassnode.com → Supply → LTH Supply |
| Miner revenue | Glassnode | glassnode.com → Mining → Revenue |
| BTC active addresses | Glassnode | glassnode.com → Addresses → Active Addresses |

---

## Cross-Asset Correlation

| Data needed | Source | Method |
|---|---|---|
| BTC vs SPX correlation | TradingView | Plot SPX and BTCUSD; use "Correlation" indicator |
| Gold vs BTC correlation | TradingView | Plot XAUUSD and BTCUSD |
| Cross-asset heatmap | Bloomberg | Market Heatmap (requires access) |
| VIX (equity vol) | CBOE | cboe.com/tradable_products/vix/ |
| MOVE index (bond vol) | CBOE | ICE MOVE Index |

---

## Global Liquidity (for global context)

| Data needed | Source | Path |
|---|---|---|
| ECB balance sheet | ECB | sdw.ecb.europa.eu |
| BOJ balance sheet | BOJ | boj.or.jp/statistics |
| PBOC balance sheet | PBOC | pbc.gov.cn → Statistics |
| Global M2 approximation | FRED (individual series) | Aggregate USD/EUR/JPY/CNY M2 manually |
| BIS cross-border banking | BIS | bis.org/statistics/bankstats.htm |
