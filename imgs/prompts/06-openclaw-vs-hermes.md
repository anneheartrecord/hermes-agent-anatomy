---
type: framework
style: notion
aspect: 16:9
output: /Users/annesheartrecord/Desktop/hermes-agent-anatomy/imgs/06-openclaw-vs-hermes.png
---

SCENE: A side-by-side comparison layout. Left side shows Hermes Gateway: a single process box containing multiple adapter blocks stacked inside, sharing one SessionStore and one HookSystem, with label "单进程多适配器". Right side shows OpenClaw Extensions: multiple separate container boxes (each with its own icon), connected via HTTP/gRPC arrows to a central orchestrator, with label "独立容器/进程". A dotted line divides the two sides. Below each, key traits listed: Hermes = "轻量 · 一致性 · 个人/小团队", OpenClaw = "隔离 · 可扩展 · 企业级多租户".

LABELS:
- Left title: "Hermes Gateway"
- Right title: "OpenClaw Extensions"
- Left trait: "单进程 · in-process 调用"
- Right trait: "多进程 · 跨进程通信"

STYLE:
Minimal hand-drawn illustration with a subtle tech edge. Off-white paper background, dark gray sketch lines, muted umbrella yellow as the only accent color, with occasional thin circuit-trace or node-graph line details woven into the composition. Lots of negative space, Notion-like doodle aesthetic meets minimal blueprint hints. No realism, no 3D, no painterly texture, no high saturation, no complex scene, no photographic detail.

ASPECT: 16:9

Add one short Chinese quote in a natural handwritten style near the bottom: "同一个问题，两种哲学"
