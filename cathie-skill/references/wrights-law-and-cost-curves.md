# Wright's Law and Cost Curves

Use this file when analyzing the cost trajectory of a disruptive technology.

> *"For every cumulative doubling of units produced, costs fall by a constant percentage."*
> — Theodore Wright, 1936 (applied to aviation manufacturing)

ARK Invest applies Wright's Law as the primary forecasting tool for disruptive technology cost curves. It is more reliable than Moore's Law (time-based) because it ties cost decline to production volume — which is observable and verifiable.

---

## The Mechanics

**Formula**: Cost(N) = Cost(1) × N^(−b)

Where:
- N = cumulative units produced
- b = learning parameter = log(1 − learning rate) / log(2)
- Learning rate = % cost decline for every doubling of cumulative production

**Simpler framing**: If the learning rate is 20%, then every time total cumulative production doubles, the cost falls by 20%.

---

## Learning Rates by Technology

| Technology | Learning Rate | Source basis |
|---|---|---|
| Lithium-ion batteries | ~18% | BloombergNEF historical data |
| Solar PV (modules) | ~20–24% | IRENA, BloombergNEF |
| Wind turbines (onshore) | ~12–15% | IRENA |
| DNA sequencing (short-read) | ~40% | NIH, Illumina cost data |
| Semiconductor logic (transistors/cost) | ~28–30% | ITRS, industry data |
| LED lighting | ~20% | DOE data |
| Humanoid robot components (est.) | ~15–20% | ARK estimates (verify) |
| LiDAR sensors | ~30–40% | Company disclosures, industry |

> ⚠️ **Evidence note**: Learning rates are derived from historical data. Early-stage technologies may have less data; use ARK or BloombergNEF estimates with medium confidence, not strong.

---

## How to Apply Wright's Law in Analysis

### Step 1: Find current cumulative production

- For batteries: cumulative GWh deployed (BloombergNEF annual BNEF Battery Price Survey).
- For solar: cumulative GW installed (IRENA World Solar Capacity Statistics).
- For sequencing: cumulative genomes sequenced (Illumina IR data, NIH).
- For robotics: cumulative unit shipments (IFR World Robotics Report).

### Step 2: Estimate current cost

- Use the most recent benchmark available (BloombergNEF, IRENA, company disclosures).
- Note: "cost" means manufacturing cost, not retail price. Use cost where possible; use price as a proxy when cost is unavailable, but note the limitation.

### Step 3: Project doublings to the target threshold

- How many more doublings of cumulative production are needed to reach the cost threshold?
- At the current growth rate in annual production, how long will those doublings take?
- This gives a timeline estimate: "at current production growth, the $60/kWh battery threshold is reached around [year]."

### Step 4: Identify what changes at each threshold

Different cost levels enable qualitatively different use cases:

**Battery cost thresholds**:
| Cost ($/kWh) | Threshold enabled |
|---|---|
| $200 | EV cost parity with ICE in premium segment |
| $100 | EV cost parity with ICE in mid-market; utility storage for peak shifting |
| $60 | Grid-scale storage economic vs new gas peaker plants in most markets |
| $40 | V2G viable; residential storage mainstream |

**DNA sequencing cost thresholds**:
| Cost ($/genome) | Threshold enabled |
|---|---|
| $1,000 | Clinical genomics for rare disease diagnosis |
| $200 | Oncology profiling in major cancer centers |
| $100 | Routine liquid biopsy at scale |
| $10 | Population-scale annual cancer screening viable |

**LiDAR cost thresholds**:
| Cost ($/unit) | Threshold enabled |
|---|---|
| $500 | Autonomous robo-taxi economics viable at small scale |
| $100 | Mass-market autonomous vehicle integration possible |
| $50 | Consumer ADAS-level sensor affordable |

---

## Wright's Law vs Moore's Law

| | Wright's Law | Moore's Law |
|---|---|---|
| **Driver** | Cumulative production volume | Time |
| **Predictability** | Higher (tied to observable variable) | Can break at physical limits |
| **Application** | Batteries, solar, sequencing, robotics | Semiconductors (historically) |
| **ARK's use** | Primary forecasting tool | Secondary reference |

---

## Common Mistakes in Cost Curve Analysis

**Mistake 1 — Using price instead of cost**
Retail prices include margins, subsidies, and competitive dynamics. Where possible, use manufacturer cost benchmarks (BNEF for batteries, IRENA for solar).

**Mistake 2 — Extrapolating the learning rate at low volume**
Learning rates can compress as production scales and easy efficiency gains are captured. The rate may slow in later S-curve phases.

**Mistake 3 — Ignoring materials constraints**
A technology may hit a materials bottleneck that breaks the cost curve (e.g., lithium, cobalt, or rare earth supply constraints). Check the bill of materials for key inputs.

**Mistake 4 — Confusing cost parity with adoption tipping point**
Cost parity is necessary but not sufficient. Infrastructure switching costs (charging networks, grid upgrades, skills retraining) can delay adoption even after cost parity is reached.

**Mistake 5 — Single-point estimates**
Always use scenarios. The learning rate is an average; variance around it is significant. Use bear/base/bull timelines for any cost threshold projection.

---

## Quick Reference: How to Present Cost Curve Analysis

Plain-language framing for final answers:

```
[Technology] current cost: $X per [unit]. 
Learning rate: ~Y% per doubling of cumulative production.
Cumulative production is currently doubling approximately every Z years.
At this rate, the $[threshold] target — which unlocks [use case] — is reached around [year range].
Bear case (slower adoption): [year+2]. Bull case (faster scale): [year-2].

Key materials risk: [input] supply could compress the learning rate if [condition].
Key competitive risk: [alternative technology] could leapfrog if [condition].
```
