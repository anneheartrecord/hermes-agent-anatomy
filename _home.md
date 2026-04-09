[English](./README_EN.md)

# Hermes Agent 源码解剖

![License](https://img.shields.io/badge/license-MIT-green)
![Docs](https://img.shields.io/badge/docs-8%20articles-blue)
![Language](https://img.shields.io/badge/language-中文-orange)
![Lines](https://img.shields.io/badge/analyzed-334K%20lines-red)
![AI](https://img.shields.io/badge/AI%20Powered-Claude%20Code-purple)

> 33 万行 Python，一个单体仓库的野心 — 从架构到实现逐模块拆解 NousResearch/hermes-agent

[Hermes Agent](https://github.com/NousResearch/hermes-agent) 是 Nous Research 开发的开源 AI Agent 框架。和市面上大部分提供积木块让你自己搭的 Agent 框架不同，它更接近一个**开箱即用的完整产品**：CLI 交互、11 平台消息网关、多 Provider 凭证池化、插件式 Memory 系统、RL 训练数据采集，全部内置。

这个系列对 hermes-agent 的源码做了系统化的技术分析，配有大量手绘风格技术插图。

## 这个系列覆盖了什么

| 篇章 | 内容 | 关键发现 |
|------|------|---------|
| [01-全景图](docs/01-全景图.md) | 架构分层、代码规模、定位分析 | 双入口（CLI + IM 网关）、RL 训练闭环是其他框架没有的 |
| [02-Agent 核心循环](docs/02-Agent核心循环.md) | AIAgent 类生命周期、并行工具执行 | 10,500 行单文件、max 90 次迭代硬上限、ThreadPoolExecutor 并行 |
| [03-Tool Registry](docs/03-Tool-Registry.md) | 工具注册、异步桥接、分发流程 | import 即注册的朴素模式、持久化 event loop 解决 sync/async 阻抗 |
| [04-多 Provider 适配](docs/04-多Provider适配.md) | 统一消息格式、凭证池化、OAuth | 4 种调度策略、429 冷却 1h / 402 冷却 24h 差异化退避 |
| [05-上下文压缩](docs/05-上下文压缩.md) | 头尾保护、LLM 结构化摘要 | 保头保尾压中间、五维度结构化摘要模板、Session 分裂链 |
| [06-消息网关](docs/06-消息网关.md) | 11 平台适配器、SessionStore、Hooks | 一套代码接 Telegram / Discord / Slack / WhatsApp 等 11 个平台 |
| [07-Memory 与 RL 训练](docs/07-Memory与RL训练.md) | 8 种 Memory 后端、轨迹压缩 | 用 Agent 训 Agent 的闭环、Skill 自主创建 + 安全扫描 |
| [08-三方对比](docs/08-三方对比.md) | Hermes vs OpenClaw vs Claude Code | 13 个维度逐项拆解，附选型决策树 |

## 关键数据

| 指标 | 数据 |
|------|------|
| 版本 | v0.8.0 |
| Python 文件 | 744 个 |
| 代码总量 | ~334,661 行 |
| 核心 Agent 循环 | run_agent.py，10,500 行 |
| 内置工具 | ~25 个核心 + MCP / 插件扩展 |
| 消息平台 | 11 个 |
| Memory 后端 | 8 种插件 |
| 凭证池策略 | 4 种（fill_first / round_robin / random / least_used） |
| 压缩阈值 | 50% 上下文窗口 |
| 终端后端 | 6 种（local / Docker / SSH / Modal / Daytona / Singularity） |

## 姊妹篇

这个系列是 [Claude Code 源码解剖](https://anneheartrecord.github.io/claude-code-docs/) 的姊妹篇。一个 TypeScript 工程驱动，一个 Python 研究驱动，放在一起看能看出两种完全不同的 Agent 哲学。

## 目标读者

正在做 Agent 产品的工程师、对 AI Agent 架构感兴趣的开发者、想了解不同 Agent 框架如何做工程取舍的技术人。
