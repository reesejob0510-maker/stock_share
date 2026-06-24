# Valuation Methods

Use this file when estimating intrinsic value and margin of safety.

> *"Price is what you pay; value is what you get."* — Warren Buffett
> *"It is far better to buy a wonderful company at a fair price than a fair company at a wonderful price."* — Warren Buffett

---

## Guiding principles

1. **Never use beta or CAPM** for the discount rate. Buffett uses 10% as his informal hurdle — roughly the long-run return of US equities. Higher for riskier or less certain businesses.
2. **Margin of safety is mandatory**. No matter how confident the estimate, apply a 25–50% discount to the intrinsic value before calling it cheap.
3. **Two methods minimum**. If different approaches give materially different answers, figure out why before proceeding.
4. **Conservative assumptions win**. It is better to miss a stock because you were too conservative than to overpay because you were too optimistic.
5. **Valuation without moat is dangerous**. Run the moat and financial quality analysis first; valuation is the last step, not the first.

---

## Method 1 — Owner Earnings DCF

This is Buffett's primary valuation framework, introduced in the 1986 Berkshire letter.

### Step 1: Estimate normalized owner earnings

- Owner Earnings = Net income + D&A − Maintenance Capex
- Use a 3–5 year average to normalize for cycles.
- Adjust for one-time items: litigation settlements, restructuring charges, non-recurring gains.
- Check: Does FCF from the cash flow statement broadly confirm the estimate?

### Step 2: Choose a growth rate

- **Conservative**: GDP + inflation (3–5% for developed markets) — use for mature businesses or uncertain growth.
- **Moderate**: 6–10% — use when there is clear evidence of organic growth runway and competitive advantage.
- **Do not exceed 10–12%** in terminal growth for the DCF base case. High growth assumptions require a separate sensitivity check.

### Step 3: Apply the discount rate

- Use 10% as the default hurdle rate.
- Use 12% for businesses with more uncertainty, smaller float, or higher cyclicality.
- Do not adjust for short-term macro views on rates — the goal is long-term owner value.

### Step 4: Calculate present value

Simple two-stage model:

```
Stage 1 (years 1–10): Discount each year's growing owner earnings at the hurdle rate.
Stage 2 (terminal value): (Year 10 owner earnings × (1 + terminal growth)) / (hurdle rate − terminal growth)
Terminal value discounted back to today.
Total intrinsic value = PV of Stage 1 + PV of Terminal Value
```

### Step 5: Apply margin of safety

- **High confidence** (wide moat, clear financials, long track record): 25% discount.
- **Medium confidence** (narrow moat, some uncertainty): 35–40% discount.
- **Lower confidence** (uncertain moat, complex financials): 50% discount or pass.

**Buy zone**: Current price < (Intrinsic value × margin of safety discount).

---

## Method 2 — Historical Multiple Anchoring

When DCF assumptions are highly uncertain, anchor to what the market has historically paid for the same quality of business.

### Identify the right multiple

- **P/E**: best for stable earners with consistent capital structure.
- **P/FCF**: better for capital-light businesses where earnings and FCF diverge.
- **EV/EBIT or EV/EBITDA**: use for capital-intensive businesses or when comparing across capital structures.
- **P/B**: most useful for financial businesses (banks, insurers) where book value approximates liquidation value.

### Compare vs history

- Pull 7–10 year range of the business's own trading multiple.
- Identify the "normal" range when the moat was intact and growth was stable.
- Current discount or premium vs normal range: is it explained by a real change in the business, or is it sentiment?

### Cross-check vs peers

- Compare multiples against direct competitors with similar moat quality.
- A business trading at a discount to peers with better financials deserves investigation.

---

## Method 3 — Earnings Yield vs Opportunity Cost

Buffett's informal cross-check: compare the earnings yield of the business to alternatives.

**Earnings yield** = Normalized EPS / Current stock price = inverse of P/E

**Comparison**:
- 10-year Treasury yield (risk-free rate).
- S&P 500 earnings yield (broad market comparison).
- Other candidates in the same analysis.

**When it is useful**:
- A high-quality business with 7–8% earnings yield and durable moat is attractive vs a 4% Treasury.
- A business at 20× P/E (5% earnings yield) needs a very clear growth story to justify the spread.

**Limitations**:
- Does not account for growth; use alongside DCF for growth businesses.
- Less useful when interest rates are abnormally low or high.

---

## Method 4 — Retained Earnings Test (Buffett's long-term check)

> *"We feel that each dollar of retained earnings... should be reinvested only if the business can reasonably be expected to return $1 of market value for each $1 retained."*

**Formula**: For every $1 of retained earnings over 5–10 years, has the market cap grown by at least $1?

- Calculate: Retained earnings cumulative (net income − dividends over period).
- Compare to: Market cap increase over same period.
- A ratio above 1.0 means management is creating value with retained capital; below 1.0 means capital allocation is questionable.

---

## Putting it together — the value range

After running two or more methods:

| Range | Meaning | Action |
|---|---|---|
| **Cheap** | Current price < intrinsic value × (1 − margin of safety) by all methods | High research priority |
| **Fair** | Current price roughly equals intrinsic value; margin of safety is thin | Monitor; wait for better entry or stronger growth evidence |
| **Expensive** | Current price > intrinsic value by most methods | Low priority unless moat is widening |
| **Uncertain** | Methods diverge materially or assumptions are too fragile | Flag key assumptions; identify what would need to be true to justify current price |

---

## Common valuation mistakes

**Mistake 1 — Using the market's growth assumptions**
: The consensus growth estimate is already in the price. Build your own estimate from fundamental evidence.

**Mistake 2 — Not normalizing earnings**
: A cyclical peak year overstates earnings capacity. A cyclical trough understates it. Use 3–5 year normalized earnings.

**Mistake 3 — Ignoring capex**
: "Earnings" that require heavy capital reinvestment to sustain are not owner earnings. Always check maintenance capex.

**Mistake 4 — Treating terminal value as precise**
: 60–80% of a DCF value often comes from terminal value. Small changes in terminal growth rate create large changes in value. Run scenarios: bear (2%), base (3–4%), bull (5%).

**Mistake 5 — Skipping the margin of safety**
: Even a correct intrinsic value estimate can be wrong by 20–30% due to assumption error. The margin of safety is not optional.
