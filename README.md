# Stock Analysis Skills

A collection of AI Agent skills for investment research, each embodying the publicly available analytical methodology of a legendary investor or macro thinker.

Each skill can be loaded into an AI Agent (Claude, GPT-4, etc.) to provide structured, source-backed investment research in that investor's style.

---

## The Five Skills

| Skill | Investor | Style | Core Framework |
|---|---|---|---|
| [serenity-skill](./serenity-skill/) | Serenity (Quantitative) | Quant / Cross-cycle | Systematic multi-strategy, cross-asset |
| [buffett-skill](./buffett-skill/) | Warren Buffett | Value investing | Moat analysis, Owner Earnings DCF |
| [cathie-skill](./cathie-skill/) | Cathie Wood | Disruptive innovation | S-curve, Wright's Law, 5-year TAM |
| [arthur-skill](./arthur-skill/) | Arthur Hayes | Crypto macro | USD liquidity (Fed + TGA + RRP), funding rates, on-chain leverage |
| [raoul-skill](./raoul-skill/) | Raoul Pal | Global macro | Global Liquidity Index (GLI), demographic/debt supercycle |

---

## How to Use

Each skill directory contains a `SKILL.md` file that can be loaded into an AI Agent. Point your agent to the skill file and ask investment research questions.

**Example prompts after loading:**

- `buffett-skill`: "用巴菲特的方式分析 Costco 的护城河"
- `cathie-skill`: "特斯拉在自动驾驶 S 曲线上处于哪个阶段？"
- `arthur-skill`: "当前的美元流动性环境对 BTC 意味着什么？"
- `raoul-skill`: "全球 GLI 现在处于哪个阶段，对资产配置有什么含义？"
- `serenity-skill`: "帮我构建一个跨周期的资产组合"

---

## Skill Structure

Each skill follows the same directory structure:

```
<skill-name>/
├── SKILL.md                    # Core skill definition (load this into your agent)
├── README.md                   # Human-readable overview (Chinese)
├── LICENSE                     # MIT License
├── references/                 # Supporting analytical frameworks
│   ├── <framework>.md
│   └── ...
└── assets/                     # Templates, scorecards, prompt packs
    ├── thesis-template.md
    ├── <scorecard>.json
    └── research-prompt-pack.md
```

---

## Skill Comparison

| Dimension | Serenity | Buffett | Cathie | Arthur | Raoul |
|---|---|---|---|---|---|
| **Time horizon** | Medium-long | Long (years) | Long (5yr+) | Short-medium (weeks-months) | Medium-long (months-years) |
| **Primary focus** | Cross-asset systematic | Individual company fundamentals | Technology disruption | Crypto macro positioning | Global macro cycles |
| **Key signal** | Multi-factor quantitative | Business quality + valuation gap | Innovation S-curve + cost curve | USD net liquidity | GLI phase |
| **Asset universe** | Multi-asset | Global equities | Tech + innovation + crypto | Crypto + crypto proxies | All major asset classes |
| **Data type** | Price + fundamental + macro | Financial filings + business analysis | Patent + adoption + cost data | Fed/Treasury/on-chain data | Central bank + demographic data |

---

## When to Use Which Skill

```
当前市场在交易宏观叙事（跨资产相关性高）
├─→ 判断全球流动性方向       → Raoul.skill
└─→ 判断加密市场具体定位     → Arthur.skill

当前市场回归基本面（跨资产相关性低）
├─→ 成熟行业、护城河分析     → Buffett.skill
└─→ 科技/颠覆性创新机会      → Cathie.skill

需要系统化、量化的跨资产策略
└─→ Serenity.skill
```

---

## Disclaimers

- All skills are based on **publicly available** research, essays, interviews, and presentations.
- **Raoul.skill** specifically: does NOT replicate the paid GMI (Global Macro Investor) service. Outputs are labeled as "framework interpretation" where proprietary data would be needed.
- These skills are for **research and educational purposes only**. Nothing here constitutes investment advice.
- Each skill's LICENSE file contains full disclaimers about methodology sources.

---

## License

MIT License. See individual skill directories for full license text.

---

## Contributing

Skills are community-built methodology tools. Contributions to improve framework accuracy, add new reference documents, or fix errors are welcome via pull request.
