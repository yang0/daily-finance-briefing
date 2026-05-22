# 📰 小翠时政财经 · 财经简报 Skill

[![GitHub](https://img.shields.io/badge/GitHub-Repositories-blue?logo=github)](https://github.com/yang0/xiaocui-finance-skill)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> 基于 YouTube 频道「小翠时政财经」的分析方法论蒸馏。输入市场数据，输出结构化财经简报。

## 特性

- **结构化简报**：宏观焦点 → 关键人物言论 → 重点公司深度 → 市场全景
- **标签系统**：`[事实]` vs `[判断]` vs `[翻译]` — 事实与观点严格区分
- **推理链**：每个判断配推理过程（A→B→C），可复现
- **比喻记忆点**：复杂概念用通俗比喻化解
- **置信度标注**：不确定的判断标注 `[置信度: X%]`
- **双重模式**：每日简报（全景） & 专题分析（深度）

## 使用方法

### 触发方式

```
用户: "出一份今天的财经简报"
  → AI 按四段式结构输出

用户: "分析一下A股"
  → 聚焦单一市场分析
```

### 前置依赖

本 Skill 不包含实时数据。需要配合以下工具之一：
- `stockquotes` / `yfinance` — 市场行情
- `websearch` + `webfetch` — 新闻公告
- `edgar-mcp` — SEC 文件

## 方法论来源

本 Skill 基于对小翠时政财经频道（YouTube: UCOhck8oLoIwSJzmwYMXsSnQ）4期节目的深度分析，提取其核心分析方法：

| 技术 | 说明 |
|------|------|
| **数据密度** | 每期30-60个事实数据，每个有来源 |
| **个人判断** | 事实后立刻给解读，不装中立 |
| **比喻记忆** | 每个核心论点配一个比喻（"考100分也没用"）|
| **全局关联** | 单点事件→逻辑链条→判断结论 |

蒸馏框架参考自 [nuwa-skill](https://github.com/alchaincyf/nuwa-skill)（女娲·Skill造人术）。

## 文件结构

```
xiaocui-finance-skill/
├── SKILL.md           # 主Skill文件（核心方法论+模板）
├── README.md          # 本文件
├── LICENSE            # MIT协议
├── references/
│   ├── sources/       # 样本节目字幕
│   └── episodes.md    # 样本节目清单
└── scripts/           # 辅助工具（预留）
```

## 许可

MIT License
