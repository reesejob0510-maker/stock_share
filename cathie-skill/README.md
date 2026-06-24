# Cathie.skill

### 让 AI 用 ARK S 曲线框架，判断颠覆性技术的渗透位置与成本拐点

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Agent Skill](https://img.shields.io/badge/Agent%20Skill-SKILL.md-black)](SKILL.md)
[![中文优先](https://img.shields.io/badge/README-%E4%B8%AD%E6%96%87%E4%BC%98%E5%85%88-red)](README.md)

---

看到 AI、新能源、机器人、基因组学这些方向，很多人能感受到热度，却很难判断：这个技术处于 S 曲线哪个阶段？成本还需要下降多远才能触发主流采用？5 年以后市场有多大？现在的估值合不合理？

Cathie.skill 把凯西·伍德（Cathie Wood）和 ARK Invest 公开研究报告、Big Ideas 年报和访谈中可观察到的分析框架做成 Agent Skill。它会从颠覆性技术出发，判断 S 曲线位置，用 Wright's Law 量化成本轨迹，估算融合后的 TAM，最后整理成一份有数据支撑的研究优先清单。

它的工作方式：先搞清楚这个技术在替代什么、替代的价格拐点在哪，再看渗透率数据支不支持当前叙事，最后判断现在的估值对应的增长假设是否合理。

> Research support only. Cathie.skill 负责研究、排序和推理；最终买卖决策由你自己决定。

---

## 为什么是 Cathie Wood 式方法

凯西·伍德在 ARK Invest 年度 Big Ideas 报告（公开发布）和公开访谈中长期输出一套可观察的颠覆性创新分析框架。核心逻辑很清楚：**成本曲线驱动 S 曲线，S 曲线驱动 TAM 扩张**。

Cathie.skill 复用的是这套公开方法论中的研究路径：

- 从五大颠覆性创新平台出发：AI、自动驾驶、机器人、能源存储、多组学/基因组学。
- 判断每项技术在 S 曲线上的精确位置——是"跨越鸿沟"还是"早期多数"，有本质区别。
- 用 Wright's Law 量化成本下降路径：每累计产量翻倍，成本下降多少？
- 识别关键成本阈值：越过这个点之后，什么新用例被解锁？
- 估算收敛 TAM：不是今天的市场，而是成本下降后被创造出来的未来市场。
- 发现平台融合：AI × 机器人、AI × 基因组学——两个平台交叉时颠覆面乘数级扩大。

这个仓库做的是公开资料研究工具。数据依托 BNEF、IRENA、IEA、NIH、IFR 等独立基准数据，以及公司年报和专利文件。

---

## 它能帮你做什么

| 你现在遇到的问题 | 可以这样问 AI | Cathie.skill 会帮你看什么 |
|---|---|---|
| 看好新能源/AI/机器人，不知道技术处于 S 曲线哪个阶段 | `用 cathie-skill 判断 [技术] 在 S 曲线的位置` | 用渗透率数据和成本基准定位，不只看故事 |
| 想知道电池/太阳能成本还需要多久下降到经济拐点 | `用 cathie-skill 分析电池成本曲线` | Wright's Law 学习率 + 关键阈值时间线 |
| 看到一家公司讲「AI 颠覆」故事，担心只是蹭热点 | `用 cathie-skill 挑战 [公司] 的颠覆叙事` | 渗透率数据支不支持，独立成本数据有没有，估值隐含了什么 |
| 想知道 5 年后市场有多大，但担心 TAM 被夸大 | `用 cathie-skill 计算 [赛道] 的收敛 TAM` | 从可观测的采用人口 × 收敛定价 × 渗透率倒推，不用今天的市场规模 |
| 手上有几只 AI/新能源候选股，想排研究优先级 | `用 cathie-skill 比较 A、B、C 三家公司` | S 曲线位置 + 成本曲线优势 + 5年 TAM 暴露度综合排序 |
| 想学 ARK 的分析框架，不知道从哪里开始 | `带我用 cathie-skill 学 S 曲线分析，每次只问我一个问题` | 从颠覆逻辑拆到成本曲线，再到 TAM 和估值 |

---

## 直接复制这个 Prompt

```text
用 cathie-skill 深度分析 [AI/新能源/机器人/基因组学] 赛道。
判断这个技术处于 S 曲线哪个阶段，成本曲线还需要走多远，
5 年 TAM 的基准情景是多少，找出 5 个最值得优先研究的标的，
说明 S 曲线位置、成本曲线优势、5年情景价值和主要降级条件。
```

```text
用 cathie-skill 分析 [电池/太阳能/DNA测序/激光雷达] 成本曲线。
用 Wright's Law 估算什么时候越过下一个关键阈值，
这个阈值会解锁什么新用例，以及有哪些约束可能打断曲线。
```

```text
用 cathie-skill 挑战 [公司] 的颠覆叙事。
S 曲线位置有渗透率数据支撑吗？成本学习率有独立数据吗？
当前股价隐含了什么增长率？什么情况说明采用会大幅慢于预期？
```

更多可复制模板见 [assets/research-prompt-pack.md](assets/research-prompt-pack.md)。

---

## 输出长什么样

```text
先判断 S 曲线位置和成本曲线进度：

• AI 赛道（LLM/推理）：已过鸿沟，进入早期多数。API 成本已越过 $1/百万 token 阈值，
  企业采用明显加速。→ 最高优先级

• 固态电池：仍在早期采用者阶段，渗透率 < 2%，量产成本比液态电池高 3–5 倍。
  成本曲线还需要 2–3 次产量翻倍。→ 降优先级，等 2026–2027 成本数据

• 人形机器人：创新/实验室阶段，尚无大规模商业部署，成本基准不确定。
  叙事领先于数据 2–3 年。→ 观察名单

如果你想找具体标的，我会优先研究：

1. [公司 A]：拥有 AI 推理成本曲线最快学习率，平台效应随应用层扩张而增强。
   5 年基准 TAM $X B，市场份额预期 Y%，当前估值隐含 Z% 年增长——略偏保守。

2. [公司 B]：处于电池成本曲线最前端，累计产量领先同类 3 倍，学习率 ~18%（BNEF 数据支撑）。
   主要风险：锂原料价格反弹可能压缩学习率。

下一步先查三件事：
1. 最新 BNEF 电池价格调查——确认学习率是否持续。
2. [公司 A] Q2 财报——推理成本指引是否支持学习率故事。
3. IEA Global EV Outlook 最新版——中国渗透率加速或放缓。
```

---

## 安装

### Claude Code

用户级安装：

```bash
SKILL_DIR="$HOME/.claude/skills/cathie-skill"
mkdir -p "$SKILL_DIR"
cp -R SKILL.md LICENSE references assets examples evals "$SKILL_DIR"/
```

项目级安装：

```bash
SKILL_DIR=".claude/skills/cathie-skill"
mkdir -p "$SKILL_DIR"
cp -R SKILL.md LICENSE references assets examples evals "$SKILL_DIR"/
```

### Codex / OpenAI Agent Skills

```bash
SKILL_DIR="$HOME/.agents/skills/cathie-skill"
mkdir -p "$SKILL_DIR"
cp -R SKILL.md LICENSE references assets examples evals "$SKILL_DIR"/
```

---

## 仓库结构

```text
cathie-skill/
├── SKILL.md                                  ← 核心 Skill 定义（11步研究工作流）
├── README.md
├── LICENSE
├── references/
│   ├── innovation-platform-framework.md      ← 五大颠覆平台 + 融合乘数逻辑
│   ├── wrights-law-and-cost-curves.md        ← Wright's Law 机制 + 各技术学习率 + 阈值识别
│   ├── scurve-adoption-analysis.md           ← S 曲线六阶段 + 跨越鸿沟框架
│   ├── valuation-methods.md                  ← 5年 TAM 情景 + 反向 DCF + 成本阈值估值
│   ├── evidence-ladder.md                    ← 证据分级（强/中/弱）
│   ├── market-source-playbook.md             ← 各市场数据来源（全球/美股/A股/清洁能源/基因组）
│   ├── cathie-dialogue-protocol.md           ← 研究伙伴对话和学习模式协议
│   ├── output-style-and-language.md          ← 输出风格和语言规范
│   └── risk-and-compliance.md                ← 研究边界和高风险情况处理
├── assets/
│   ├── thesis-template.md                    ← 颠覆性创新投资备忘录模板
│   ├── innovation-scorecard.json             ← 创新打分 JSON 模板
│   └── research-prompt-pack.md               ← 可复制的 Prompt 模板集
├── examples/
│   ├── ev-battery-cost-curve-demo.md         ← EV 电池 Wright's Law 示例（待补充）
│   └── ai-platform-scurve-demo.md            ← AI 平台 S 曲线示例（待补充）
└── evals/
    └── test-cases.md                         ← 触发和行为测试用例（待补充）
```

---

## 关键数据资源

| 技术 | 成本数据来源 | 采用率数据来源 |
|---|---|---|
| 电池/新能源汽车 | BloombergNEF 电池价格调查 | IEA Global EV Outlook / 乘联会 |
| 太阳能/风电 | IRENA 可再生能源发电成本 | IRENA 装机容量统计 |
| DNA 测序 | NIH/NHGRI 基因组测序成本 | Illumina IR / 学术文献 |
| AI 推理 | 公司 API 定价历史 | McKinsey/Gartner 企业采用调查 |
| 激光雷达/自动驾驶 | 公司披露 / 行业报告 | NHTSA AV 数据 / CARB |
| 机器人 | IFR 世界机器人报告 | IFR 年度出货量统计 |

---

## 与 Serenity.skill 和 Buffett.skill 的关系

| | Serenity.skill | Buffett.skill | Cathie.skill |
|---|---|---|---|
| 核心问题 | 谁控制供应链卡点？ | 护城河够不够宽？ | S 曲线在哪，成本何时到拐点？ |
| 分析起点 | 热点 → 产业链拆解 | 商业模式 → 护城河 | 技术平台 → S 曲线 + 成本曲线 |
| 时间框架 | 3–12 个月 | 5–10 年 | 5 年（到收敛） |
| 估值方法 | 产业链卡点定性 + 排序 | DCF + 历史估值 | TAM 情景 + 反向 DCF |
| 最适合 | 科技/制造/产业链 | 消费/金融/医疗 | 颠覆性技术/平台/新能源 |

三个 Skill 可以组合使用：Serenity 帮你找产业链机会，Cathie 帮你判断技术采用拐点，Buffett 帮你验证长期护城河和估值安全边际。

## License

MIT
