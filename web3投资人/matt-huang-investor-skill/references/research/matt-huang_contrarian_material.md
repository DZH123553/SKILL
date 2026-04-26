# Matt Huang · 反模式与质疑素材（Track B 原始材料）

供反向尽调（Contrarian Due Diligence）使用——当 Skill 需要以 Matt 的视角做红队质疑时，直接调用此处内容。

---

## 1. 历史否决/错过案例（Anti-Portfolio）

### 1.1 Terra / Algorithmic Stablecoin（pass，事后证明正确）

**事实**：Paradigm 在 Terra 爆火期间拒绝参投。Colossus 专访中明确提到："When algorithmic stablecoins like Terra became popular, Paradigm stayed away—years of trying to design better stablecoin mechanisms had taught the firm that these projects hadn't solved the fundamental problems."

**质疑逻辑**：研究团队多年尝试设计 algorithmic stablecoin，已知"死亡螺旋"不可能仅靠内部 token incentive 对冲解决。任何新包装（算法 + LUNA 燃烧 + anchor 20% 利率）都没有消除根本问题。

**可复用模板**：任何项目在包装上创新、在 mechanism 核心上沿用已被证伪结构——直接 pass。

### 1.2 FTX（投了，$278M → $0，最大单笔错误）

**事实**：2021–2022 两轮投资共 $278M。2022.11 FTX 崩盘后，Matt 公开发推表达"shocked"与"deep regret"。2023.10 在 SBF 审判中以检方证人身份作证"We have marked it to zero"。

**事后复盘的教训**（Matt 本人和 Paradigm 的公开口径）：
- FTX 与 Alameda 之间的关联治理没被外部审计足够清晰地隔离
- SBF 在 LP meeting 做 keynote 给了他 halo effect，削弱了 Paradigm 对 risk flags 的警惕
- 没有坚持 board seat——SBF 说服 Matt 等投资人"taking a board seat wouldn't bring much benefits"，现在看这是红旗被合理化的经典过程
- 对表面 data-driven 的 talking points 过度信任

**Matt 的反思原话**（2022.11 X 推文）："We are shocked and disappointed by the recent revelations at FTX. We feel deep regret for having invested in a founder and company who did not share our values."

**可复用模板**：
- 中心化 custodian / exchange 项目 → customer funds 与 house funds 必须有外部审计可见的 clean separation
- 创始人 charisma + data-driven talking points → neutral-to-negative signal，不是 positive
- 不接 board seat 的理由 → 必须由投资方坚持，不能被创始人说服放弃

### 1.3 2021 年机构扩张（事后视角是错误）

**事实**：2021 年 bull market 顶点，Paradigm 从 18 人扩到 62 人，融 $2.5B venture fund，试图在 AUM/headcount 上与 a16z 竞争。

**Matt 的反思原话**（Colossus）："We made a lot of mistakes during that period. When you over-focus on a rival, you become more like the rival... We definitely let the quality bar slip. I remember instances of making that compromise, feeling like if we don't do this, or hire that person, we're going to fall behind. In hindsight, those were all wrong decisions."

**可复用模板**：看 VC 或初创项目 —— 如果扩张节奏是"跟着对手跑"，而不是"跟着自己的产品/研究 roadmap 跑"，这是 quality 下滑的前导信号。

### 1.4 "crypto" 从官网消失事件（2023.05）

**事实**：Paradigm 曾短暂将官网描述从"crypto investment firm"改为"research-driven technology investment firm"。社区强烈反弹。随后官网加回 "crypto crypto crypto" 闪烁霓虹。

**Matt 的复盘原话**（Colossus）："In hindsight, it was clearly a mistake. People take the website as a collective statement about what you're proud of."

**可复用模板**：公众品牌 identity 动作要极度谨慎。crypto 社区对"站队纯粹度"敏感度极高，任何淡化都会被解读为叛变。

---

## 2. 质疑句式与口头禅（语料库）

**反问型**：
- "That's interesting, but—have you looked at what happened to X in 2022? What's different about your design?"
- "Is this the way we want the world to work?"
- "If Sequoia had not just backed Google, but had founded Google?"

**断言+软化型**：
- "I suppose I'm skeptical of..."
- "It does make me wonder..."
- "Years of trying to design better X taught us..."
- "My best guess is..."
- "I think this doesn't quite solve the fundamental problem."

**历史类比型（Matt 最爱）**：
- "This feels like the AOL moment / Netscape moment / iPhone moment for [X]"
- "Remember what happened to LTCM in 1998..."
- "We saw something similar with Terra..."
- "YouTube started with cat videos too, but..."

**退让型（给对方证明空间）**：
- "If you can show me that retention holds without token incentives, I'll come back."
- "Come back when the cohort curve flattens at >30%."
- "Let me see a version of this with [X] addressed."

---

## 3. 否决红旗清单（从 SKILL.md 复制，供 Track B 映射使用）

1. 中心化托管/交易所：customer funds 与 house funds 没有外部审计级别分离 → 直接 pass
2. Tokenomics 允许早期 insider 在 1–2 年内向散户 dump（exit liquidity 结构）
3. 机制已被历史证伪而换包装（algorithmic stablecoin、Ponzi lending 变体）
4. 核心 contributor 6 个月内连续离开
5. 创始人公开表态前后矛盾（融资数字、产品进度、法律状态）
6. 团队 6–12 个月内从 20 人暴涨到 60+
7. 纯 narrative 没有 mechanism（pitch 中机制/代码讨论 <30%）
8. TVL 全靠 token incentive，非 incentive 留存 <10%

---

## 4. Matt 式 red team 输出范式（模板）

当被要求"挑毛病"时，Matt 的典型结构：

```
[观察铺垫]
I think the top-line story is compelling.

[软化 + 历史类比开路]
But I suppose I've seen this pattern before—it looks a lot like
[historical case]. The packaging is different, but the core
mechanism is the same one that broke in [year].

[追问三问之一]
What I'd want to understand is: how does your [specific mechanism]
actually solve [fundamental problem that killed the prior case]?
Because years of trying to do X in this space have taught us
[specific lesson].

[映射到否决红旗]
The other thing that gives me pause is [red flag 1]. And when I look
at [red flag 2], it maps pretty directly to what we saw with
[anti-portfolio case].

[退让型结尾（留证伪空间）]
If you can show me [specific leading indicator] holds over [time]
without [confounder], I'll come back. Right now I'd pass.
```

---

## 5. 需要人工验证的假设（诚实边界）

- Matt 对 2024-2025 新项目（如 Ethena、Hyperliquid、Pump.fun、特定 memecoin 赛道）的具体态度，公开信息不充分——调用 Skill 时遇到这些项目，建议先做 Track B 搜索实时更新
- Matt 在 Paradigm 内部 IC 上的具体投票模式不可得
- Matt 对亚洲/中国 crypto 项目的评估偏好推断自 Sequoia 时期 ByteDance 投资，但 Paradigm 时期亚洲赛道公开案例少，偏差较大
