# Market Source Playbook

Quick reference for global macro data sources used in Raoul Pal-style analysis.

---

## Central Bank Balance Sheets

| Central bank | Data source | URL |
|---|---|---|
| US Federal Reserve | FRED (WALCL) | fred.stlouisfed.org/series/WALCL |
| European Central Bank | ECB SDW | sdw.ecb.europa.eu |
| Bank of Japan | BOJ Statistics | boj.or.jp/statistics |
| People's Bank of China | PBOC Statistics | pbc.gov.cn → Statistics |
| Bank of England | BOE Database | bankofengland.co.uk/statistics |
| Bank of Canada | BOC Statistics | bankofcanada.ca/rates |
| Reserve Bank of Australia | RBA Statistics | rba.gov.au/statistics |

---

## M2 Money Supply

| Economy | Source | Notes |
|---|---|---|
| US M2 | FRED: M2SL | Weekly, seasonally adjusted |
| Eurozone M2 | ECB SDW: BSI.M.U2.Y.V.M20.X.1.U2.2300.Z01.E | Monthly |
| Japan M2 | BOJ: M2 series | Monthly |
| China M2 | PBOC statistics portal (人民银行 M2 数据) | Monthly |
| UK M2 | BOE Statistics: M2 | Monthly |
| Global M2 combined | Construct manually; or use Bloomberg WGDPM2 index (requires access) | |

---

## Credit Impulse

| Economy | Source | Notes |
|---|---|---|
| China credit impulse | PBOC: aggregate financing to real economy | Key leading indicator; monthly |
| Global credit impulse | BIS Credit Statistics + national central banks | Requires manual aggregation |
| US bank credit | FRED: TOTBKCR | Total bank credit |
| ECB bank lending survey | ECB | Quarterly; qualitative + quantitative |

---

## Demographic Data

| Data needed | Source | URL |
|---|---|---|
| Global population projections | UN Population Division | population.un.org |
| Working-age population ratios | World Bank | data.worldbank.org |
| Dependency ratios by country | OECD | stats.oecd.org |
| US cohort size by age | US Census Bureau | census.gov/data/tables/time-series/demo/popest/2020s-national-detail |
| Retirement age trends | OECD | oecd.org/employment/oecd-employment-outlook |

---

## Debt and Fiscal

| Data needed | Source | URL |
|---|---|---|
| Global debt/GDP | IMF Global Debt Database | imf.org/external/datamapper |
| Government debt/GDP by country | World Bank | data.worldbank.org |
| US federal debt | FRED: GFDEBTN | fred.stlouisfed.org |
| US CBO 10-year fiscal outlook | CBO | cbo.gov/publication/fiscal-outlook |
| BIS debt statistics | BIS | bis.org/statistics/totcredit.htm |

---

## Cross-Asset Market Data

| Data needed | Source | Notes |
|---|---|---|
| BTC / ETH price | TradingView, CoinGecko | |
| S&P 500 | TradingView: SPX | |
| Gold | TradingView: XAUUSD | |
| DXY (Dollar Index) | TradingView: DXY | Key cross-asset signal |
| US 10Y yield | TradingView: US10Y or FRED: DGS10 | |
| TIPS yield (real rate) | FRED: DFII10 | 10-year real rate |
| VIX | CBOE | |
| USDJPY | TradingView: USDJPY | BOJ carry trade proxy |
| EM equity index | iShares EEM ETF or MSCI EM | |

---

## Crypto GLI Beta Data

| Data needed | Source | Notes |
|---|---|---|
| BTC vs Global M2 correlation | Construct on TradingView | Overlay BTC/USD and Global M2 chart |
| BTC vs DXY | TradingView | DXY falling = BTC bullish |
| BTC dominance | TradingView: BTC.D | Altcoin vs BTC cycle indicator |
| Crypto market cap total | TradingView: TOTAL | |
| BTC halving countdown | Various crypto sites | e.g., nicehash.com/bitcoin-halving |

---

## Raoul Pal's Public Content

| Content | Source | Notes |
|---|---|---|
| Long-form macro explanations | Real Vision YouTube | Free content on macro education |
| Current market commentary | Raoul Pal on X: @RaoulGMI | Mix of free and subscriber-only |
| Real Vision interviews | realvision.com | Some free, some subscription |
| GMI institutional research | globalmacroinvestor.com | Paid subscription required |
