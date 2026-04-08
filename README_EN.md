[中文](./README.md)

# Hermes Agent Source Code Anatomy

![License](https://img.shields.io/badge/license-MIT-green)
![Docs](https://img.shields.io/badge/docs-8%20articles-blue)
![Language](https://img.shields.io/badge/language-Chinese-orange)
![Lines](https://img.shields.io/badge/analyzed-334K%20lines-red)
![AI](https://img.shields.io/badge/AI%20Powered-Claude%20Code-purple)

NousResearch/hermes-agent is an open-source AI Agent framework with 334K lines of Python. It includes everything from CLI interaction to an 11-platform messaging gateway to RL training data collection, all in a single monorepo.

This repository is a systematic technical analysis of hermes-agent's source code, with module-by-module breakdowns and hand-drawn technical illustrations. The final article compares Hermes Agent, OpenClaw, and Claude Code across 13 dimensions.

Sister project: [Claude Code Source Code Anatomy](https://github.com/anneheartrecord/claude-code-docs)

## Table of Contents

| # | Article | Topics |
|---|---------|--------|
| 01 | Panoramic Overview | Architecture, code scale, positioning |
| 02 | Agent Core Loop | AIAgent lifecycle, IterationBudget, parallel tool execution |
| 03 | Tool Registry | ToolEntry metadata, singleton pattern, async bridging |
| 04 | Multi-Provider Adaptation | Unified message format, credential pooling, OAuth |
| 05 | Context Compression | Head-tail protection, LLM summarization, session splitting |
| 06 | Message Gateway | GatewayRunner, 11 platform adapters, hooks system |
| 07 | Memory & RL Training | 8 memory backends, SQLite FTS5, trajectory compression |
| 08 | Three-Way Comparison | Hermes Agent vs OpenClaw vs Claude Code |

## License

MIT
