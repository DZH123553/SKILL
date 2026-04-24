# 女娲 · Skill造人术（投资人版）

> 基于 [女娲 · Skill造人术](https://github.com/alchaincyf/nuwa-skill) 的投资人特化版本

## 概述

本项目是女娲 Skill 造人术的**投资人版本**，专门用于蒸馏投资人的思维框架和决策模式。与通用版本相比，本版本在以下维度进行了深度特化：

**调研维度**聚焦投资人身份后的经历，重点覆盖投资组合/案例、投资风格与偏好、项目判断标准、投资相关的公开发言和观点。

**心智模型提炼方向**从通用思维框架改为投资决策相关的思维模型，如创始人评估框架、赛道判断逻辑、估值方法论等。

**决策启发式方向**聚焦投资判断准则——看项目、看创始人、看赛道的具体逻辑。

**输入源调整**重点纳入过往投资案例、加入投资机构后的公开表态，以及社交媒体（X/Twitter、LinkedIn）上的投资相关发言。

## 目录结构

```
├── SKILL.md                              # [投资人] 投资人版 Skill（蒸馏产物）
├── README.md                             # 本文件
└── references/
    ├── extraction-framework.md           # 投资人版提炼方法论（含反模式/质疑风格维度）
    ├── contrarian-research-framework.md  # 反向尽调方法论（Track B 自主调研 SOP）
    ├── skill-template.md                 # 投资人版 Skill 输出模板（含双轨 Agentic Protocol）
    └── research/                         # 调研原始数据
        ├── [investor]_portfolio.md
        ├── [investor]_public_statements.md
        ├── [investor]_social_media.md
        └── [investor]_contrarian_material.md   # 反模式与质疑素材（新增）
```

## 核心能力：双轨 Agentic Protocol

本版本在女娲原有 Agentic Protocol 基础上，引入**双轨自主调研**：

- **Track A — 正向研究**：此人会看重的亮点（项目/创始人/赛道）
- **Track B — 反向尽调（Contrarian Due Diligence）**：自主收集最能推翻乐观判断的事实与观点

Skill 激活后评估具体项目时，默认**同步**启动 A/B 双轨，通过 Steelman 反方三问、红旗映射、红线清单等机制避免确认偏误，最终以此人的**质疑风格**输出平衡的投资判断。详见 `references/contrarian-research-framework.md`。

**触发关键词**：用户说"挑毛病 / red team / 给我最坏情况 / 我会投吗 / 反方观点"时，Track B 将主导输出。

## 与原版女娲的兼容性

本版本保持了女娲原有的整体结构，包括四阶段蒸馏流程（采集 → 验证 → 构建 → 质检）和五层蒸馏体系（表达DNA、心智模型、决策启发式、反模式、诚实边界）。新增的"反向尽调 Track B"属于 Agentic Protocol 的运行时扩展，不改变上游结构，也不影响与原版女娲工具链的兼容性。

## 致谢

- 原版女娲 Skill 造人术：[花叔](https://x.com/AlchainHust) / [GitHub](https://github.com/alchaincyf/nuwa-skill)
