# Buffett.skill

### 让 AI 用巴菲特护城河框架，筛出内在价值被低估的高质量资产

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Agent Skill](https://img.shields.io/badge/Agent%20Skill-SKILL.md-black)](SKILL.md)
[![中文优先](https://img.shields.io/badge/README-%E4%B8%AD%E6%96%87%E4%BC%98%E5%85%88-red)](README.md)

---

看到消费、金融、医疗这些行业里一堆标的，很多人能感受到某家公司"挺好的"，却很难判断：护城河到底够不够宽？财务质量是真实的还是靠杠杆堆出来的？现在的价格有没有安全边际？

Buffett.skill 把沃伦·巴菲特公开信、年报及访谈中可观察到的投研路径做成 Agent Skill。它会从商业模式出发，判断竞争优势来源，验证财务质量，估算内在价值，最后整理成一份有逻辑、有证据、有安全边际的研究优先清单。

它的工作方式：先搞清楚这家公司靠什么赚钱、为什么客户不换，再看数字是否支撑这个故事，最后判断现在的价格有没有给足折扣。

> Research support only. Buffett.skill 负责研究、排序和推理；最终买卖决策由你自己决定。

---

## 为什么是巴菲特式方法

沃伦·巴菲特在伯克希尔股东信（1977 年至今）和公开访谈中长期输出一套可观察、可验证的投资框架。核心逻辑很清楚：**好公司 × 合理价格**。

Buffett.skill 复用的是这套公开方法论中的研究路径：

- 从商业模式开始，先看客户为什么付钱、付多少年了。
- 把竞争优势拆成五类来源：品牌定价权、网络效应、切换成本、成本优势、监管护城河。
- 用财务数据检验：ROE、所有者收益（Owner Earnings）、FCF 转化率、资本配置记录。
- 用 DCF + 历史估值区间双重锚定内在价值，留足安全边际。
- 最后找到最容易让判断出错的条件，给出可观测的降级信号。

这个仓库做的是公开资料研究工具。它吸收巴菲特式研究的结构化思路，同时要求所有公司判断回到年报、财报、管理层信件、交易所公告等一手资料。

---

## 它能帮你做什么

| 你现在遇到的问题 | 可以这样问 AI | Buffett.skill 会帮你看什么 |
|---|---|---|
| 看好某家消费或医疗公司，不知道护城河够不够宽 | `用 buffett-skill 分析 [公司] 的护城河来源和宽度` | 拆五类护城河来源，找财报层面的定价权和毛利率证据 |
| ROE 很高，担心是杠杆堆出来的而不是真实竞争力 | `帮我 Du Pont 分解 [公司] 的 ROE，判断质量` | 净利润率 × 资产周转率 × 财务杠杆，分清真实盈利能力 |
| 股价下跌想抄底，但不确定有没有安全边际 | `用 buffett-skill 计算 [公司] 的内在价值区间` | 所有者收益 DCF + 历史估值区间双锚，给出买入价参考 |
| 手上有几只候选股，想让 AI 帮排研究优先级 | `用 buffett-skill 比较 A、B、C 三家公司` | 按护城河宽度、财务质量、估值安全边际综合排序 |
| 看到市场热捧一只股票，想知道它有没有真实护城河 | `用 buffett-skill 挑战 [公司]，护城河证据够不够` | 查它的毛利率历史、定价行为、客户切换成本证据 |
| 想学巴菲特框架，不知道从哪里开始 | `带我用 buffett-skill 学护城河分析，每次只问我一个问题` | 从商业模式拆到竞争优势，再到财务验证和估值 |

---

## 直接复制这个 Prompt

```text
用 buffett-skill 深度分析 [公司/股票代码]。
联网查年报、财报、历史 ROE、FCF 转化率和管理层资本配置记录，
判断护城河来源和宽度，估算所有者收益和内在价值区间，
说明安全边际、排序理由和主要降级条件。
```

```text
用 buffett-skill 扫描 A 股消费/医疗/金融板块。
找出护城河最宽、ROE 最稳定、估值给了足够安全边际的 5 家公司，
说明每家的护城河来源、财务质量和主要风险。
```

```text
用 buffett-skill 挑战 [公司]。
护城河来源是什么？证据够不够？
FCF 和净利润是否匹配？管理层资本配置记录怎么样？
以现在的价格，市场在假设什么增长？什么情况说明这个判断错了？
```

更多可复制模板见 [assets/research-prompt-pack.md](assets/research-prompt-pack.md)。

---

## 输出长什么样

```text
先排护城河层级：宽护城河（ROE 稳定 > 20%，有定价权证据）→ 窄护城河（有竞争优势但面临压力）→ 不确定（故事多于证据）。

如果你想找具体标的，我会优先研究这几家：

1. [公司 A]：品牌护城河，近 5 年毛利率比行业均值高 15pp，ROE 均值 23%，FCF 转化率 0.9×。
   以现在的价格，所有者收益 DCF 给出安全边际约 30%。
   主要风险：私域流量冲击传统渠道，需要跟踪年度渠道数据。

2. [公司 B]：切换成本护城河，合同负债持续增长，ROE 18%，但负债率偏高（净债/EBITDA 2.5×）。
   估值在历史区间中位数，安全边际有限。

3. [公司 C]：护城河来源不清晰，毛利率在下降，FCF 持续低于净利润。
   降级至「观察」，等下一份年报核实。

下一步先查三件事：
1. [公司 A] 年报里的分渠道毛利率和定价政策说明。
2. [公司 B] 最新季报里的合同负债和现金流。
3. [公司 C] 毛利率下降的原因解释（财报电话会纪要）。
```

---

## 安装

### Claude Code

用户级安装：

```bash
SKILL_DIR="$HOME/.claude/skills/buffett-skill"
mkdir -p "$SKILL_DIR"
cp -R SKILL.md LICENSE references assets examples evals "$SKILL_DIR"/
```

项目级安装：

```bash
SKILL_DIR=".claude/skills/buffett-skill"
mkdir -p "$SKILL_DIR"
cp -R SKILL.md LICENSE references assets examples evals "$SKILL_DIR"/
```

### Codex / OpenAI Agent Skills

用户级安装：

```bash
SKILL_DIR="$HOME/.agents/skills/buffett-skill"
mkdir -p "$SKILL_DIR"
cp -R SKILL.md LICENSE references assets examples evals "$SKILL_DIR"/
```

### 其他 AgentSkills-compatible 客户端

把 `SKILL.md`、`LICENSE`、`references/`、`assets/`、`examples/`、`evals/` 放进对应客户端的 `buffett-skill/` 目录即可。

---

## 仓库结构

```text
buffett-skill/
├── SKILL.md                              ← 核心 Skill 定义（入口文件）
├── README.md
├── LICENSE
├── references/
│   ├── moat-framework.md                 ← 五类护城河来源、宽度评级、降级信号
│   ├── financial-quality-checklist.md    ← ROE/所有者收益/FCF/资本配置核查清单
│   ├── valuation-methods.md              ← DCF/历史估值/收益率法三种估值方法
│   ├── evidence-ladder.md                ← 证据分级标准（强/中/弱）
│   ├── market-source-playbook.md         ← 各市场数据来源（美股/港股/A股/日本）
│   ├── buffett-dialogue-protocol.md      ← 研究伙伴对话和学习模式协议
│   ├── output-style-and-language.md      ← 输出风格和语言规范
│   └── risk-and-compliance.md            ← 研究边界和高风险情况处理
├── assets/
│   ├── thesis-template.md                ← 巴菲特式投资备忘录模板
│   ├── moat-scorecard.json               ← 护城河打分 JSON 模板
│   └── research-prompt-pack.md           ← 可复制的 Prompt 模板集
├── examples/
│   ├── consumer-brand-moat-demo.md       ← 消费品牌护城河分析示例（待补充）
│   └── financial-compounder-demo.md      ← 金融复利机器分析示例（待补充）
└── evals/
    └── test-cases.md                     ← 触发和行为测试用例（待补充）
```

---

## 研究边界

Buffett.skill 是独立的公开方法论项目，灵感来自沃伦·巴菲特（Warren Buffett）公开信、访谈和伯克希尔年报中可观察到的研究范式。功能范围限于研究辅助。

它提供研究优先级、护城河判断、财务质量核查、估值区间参考和下一步核验清单。交易执行、账户操作、收益承诺和最终买卖判断始终由用户自己控制。

强结论应以年报、财报、管理层信件、交易所公告、可信媒体和行业数据为依据。社交媒体内容适合作为线索来源，最终判断要回到更强证据。

---

## 与 Serenity.skill 的关系

| | Serenity.skill | Buffett.skill |
|---|---|---|
| 核心问题 | 谁控制了供应链卡点？ | 这家公司有没有持久竞争优势？ |
| 分析起点 | 宏观热点 → 产业链拆解 | 商业模式 → 护城河来源 |
| 判断维度 | 供应商数量、验证周期、扩产难度 | 定价权、ROE、FCF、资本配置 |
| 时间框架 | 3–12 个月（供需周期） | 5–10 年（复利积累） |
| 最适合 | 科技/制造/产业链主题 | 消费/金融/医疗/平台型企业 |

两个 Skill 可以互补：Serenity 帮你找产业链机会，Buffett 帮你判断找到的公司是否值得长期持有。

## License

MIT
