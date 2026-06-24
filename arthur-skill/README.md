# Arthur.skill

> 加密宏观流动性猎手 — 受 Arthur Hayes 公开方法论启发

---

## 这个 Skill 做什么

Arthur.skill 将你的 AI Agent 变成一个专注**美元流动性周期**和**加密宏观定位**的研究伙伴。

核心逻辑来自 Hayes 在 Maelstrom Fund Substack 和 BitMEX Research 的公开文章：**比特币是全球美元流动性的高 Beta 看涨期权**。当美元净流动性扩张时，加密上涨；当净流动性收缩时，加密下跌。其他一切都是噪音。

---

## 分析路径

```
美元净流动性方向
  → 美联储资产负债表 + TGA 余额变化 + RRP 动态
  → 加密市场 Beta 环境判断（周期阶段）
  → 永续合约资金费率 + OI 结构
  → 链上杠杆密度（DeFi 借贷利率 + 清算密集区）
  → 宏观/监管事件风险
  → 综合风险姿态
  → 什么情况说明这个判断错了
```

---

## 核心概念

### 美元净流动性 = 美联储表 + TGA 消耗 − 逆回购（RRP）

| 组成部分 | 看多信号 | 看空信号 |
|---|---|---|
| 美联储资产负债表 | QE 或 QT 暂停 | 主动 QT 进行中 |
| TGA 余额 | 下降（财政支出/债务上限约束） | 上升（国债发行重建） |
| 隔夜逆回购 RRP | 下降（闲置资金回流系统） | 上升（资金被吸收） |

### 资金费率 = 实时仓位温度计

- 正向费率（多头支付空头）→ 市场净多，可能过度拥挤
- 负向费率（空头支付多头）→ 空头主导，轧空可能性上升
- 结合 OI 趋势，判断行情可持续性

### 链上杠杆 = 级联清算风险评估

- DeFi 稳定币借贷利率 → 链上加杠杆的需求强度
- 清算密集区距当前价格 → 价格下跌多少触发踩踏式清算
- 综合评级：低 / 适度 / 高 / 危险

---

## 触发场景

- "用 Arthur Hayes 的方式看当前 BTC 走势"
- "现在的美元流动性是正的还是负的？"
- "资金费率极端了吗？"
- "链上杠杆有没有踩踏风险？"
- "下次 FOMC 前后怎么布局？"
- "为什么 BTC 在流动性正向时还在跌？"
- "hayes framework", "USD liquidity", "funding rates", "on-chain leverage"

---

## 输出样例

```
流动性方向：正向
- 美联储：QT 暂停（表 +200亿/周）
- TGA：下降（近4周 -1500亿）
- RRP：下降（近4周 -3000亿）
→ 综合：三项全部正向，强力流动性顺风

资金费率（BTC 年化）：18%
- 历史分位：过去 12 个月 55% 分位
- OI：上升 + 价格上升 → 新多单主导，可持续
→ 信号：多头略微偏高但不极端

链上杠杆：适度
- AAVE 稳定币借贷年化：7.2%
- 最近清算密集区：$78,000（距当前 -9%）
→ 风险：适度，安全距离尚可

综合风险姿态：积极持仓
降级信号：如果 RRP 开始上升 + 资金费率 > 50%，减仓
```

---

## 与其他 Skill 的关系

| Skill | 核心框架 | 最适用场景 |
|---|---|---|
| **Arthur.skill** | 美元流动性 + 资金费率 + 链上杠杆 | 加密宏观定位、短中期 Beta 判断 |
| **Raoul.skill** | 全球 GLI + 人口债务长周期 | 全球宏观资产配置、长期结构性判断 |
| **Cathie.skill** | 颠覆性创新 + S 曲线 + Wright's Law | 技术叙事驱动的加密上涨阶段 |
| **Buffett.skill** | 护城河 + 价值投资 | 加密股权代理（Coinbase 等）基本面 |
| **Serenity.skill** | 量化/跨周期 | 系统化多资产策略 |

---

## 局限性

- 仅用 Hayes 的**公开**研究（Substack、BitMEX Research、公开采访），不是 Maelstrom 基金的内部策略。
- 实时链上数据（资金费率、清算墙）需要用户自行通过 Coinglass / Glassnode / DefiLlama 确认最新读数。
- 宏观数据有发布滞后：美联储表每周更新，TGA 和 RRP 每天更新，M2 每月更新。

---

## 数据来源

- 美联储 H.4.1 (federalreserve.gov)
- 纽约联储 RRP (newyorkfed.org)
- 美国财政部 TGA (fiscaldata.treasury.gov)
- Coinglass (funding rates, OI)
- Glassnode (on-chain analytics)
- CryptoQuant (leverage ratio, exchange flows)
- DefiLlama (DeFi lending, liquidations)

---

## 免责声明

本 Skill 为公开方法论推演工具，不构成投资建议。基于 Arthur Hayes 公开发表的研究，与 Maelstrom Fund 无关联。买卖决策由用户自行负责。

---

## 许可证

MIT License. 详见 LICENSE 文件。
