[English](./README_EN.md)

# Hermes Agent 源码解剖

![License](https://img.shields.io/badge/license-MIT-green)
![Docs](https://img.shields.io/badge/docs-8%20articles-blue)
![Language](https://img.shields.io/badge/language-中文-orange)
![Lines](https://img.shields.io/badge/analyzed-334K%20lines-red)
![AI](https://img.shields.io/badge/AI%20Powered-Claude%20Code-purple)

NousResearch/hermes-agent 是一个 33 万行 Python 代码的开源 AI Agent 框架。从 CLI 交互到 11 平台消息网关到 RL 训练数据采集，全部内置在一个单体仓库里。

这个仓库是对 hermes-agent 源码的系统化技术分析，逐模块拆解，配有大量手绘风格技术插图。最后一篇将 Hermes Agent、OpenClaw、Claude Code 三个框架放在一起做了 13 个维度的对比。

姊妹篇：[Claude Code 源码解剖](https://github.com/anneheartrecord/claude-code-docs)

## 文档目录

### 全景篇

| 文档 | 内容 |
|------|------|
| [01-全景图](./docs/01-全景图.md) | Nous Research 背景、整体架构、代码规模、定位分析 |

### 核心模块篇

| 文档 | 内容 |
|------|------|
| [02-Agent 核心循环](./docs/02-Agent核心循环.md) | AIAgent 类生命周期、IterationBudget、并行工具执行、消息清洗 |
| [03-Tool Registry](./docs/03-Tool-Registry.md) | ToolEntry 元数据、单例注册、异步桥接、handle_function_call 分发 |
| [04-多 Provider 适配](./docs/04-多Provider适配.md) | 统一消息格式、Anthropic 适配器、凭证池化、OAuth 认证 |
| [05-上下文压缩](./docs/05-上下文压缩.md) | 头尾保护、LLM 结构化摘要、Session 分裂、轨迹压缩 |
| [06-消息网关](./docs/06-消息网关.md) | GatewayRunner、SessionStore、11 平台适配器、Hooks 系统 |
| [07-Memory 与 RL 训练](./docs/07-Memory与RL训练.md) | 8 种 Memory 后端、SQLite FTS5、批量轨迹生成、Skill 安全扫描 |

### 对比篇

| 文档 | 内容 |
|------|------|
| [08-三方对比](./docs/08-三方对比.md) | Hermes Agent vs OpenClaw vs Claude Code，13 个维度逐项拆解 |

## 关键数据

| 指标 | 数据 |
|------|------|
| 版本 | v0.8.0 |
| Python 文件 | 744 个 |
| 代码总量 | ~334,661 行 |
| 核心依赖 | openai / anthropic / httpx / rich / prompt_toolkit |
| Agent 循环上限 | 90 次迭代 |
| 内置工具 | ~25 个核心 + MCP/插件扩展 |
| 消息平台 | 11 个 |
| Memory 后端 | 8 种插件 |
| 凭证池策略 | 4 种 |

## License

本仓库为技术分析文档，不包含 hermes-agent 源码本身。

MIT
