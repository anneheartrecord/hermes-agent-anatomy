---
type: framework
style: notion
aspect: 16:9
output: /Users/annesheartrecord/Desktop/hermes-agent-anatomy/imgs/07-trajectory-compression.png
---

SCENE: A horizontal before-and-after diagram. Left side "压缩前": a long sequence of message blocks in a row: [system] [human] [gpt] [tool] [gpt] [tool] [gpt] [tool] [gpt] [tool] [gpt] [tool]. The first 4 blocks and last 4 blocks have a subtle yellow shield icon meaning "protected". The middle blocks are in a dashed bracket labeled "可压缩区域". Right side "压缩后": the same first 4 protected blocks, then a single highlighted block labeled "[CONTEXT SUMMARY]", then the last 4 protected blocks. An arrow connects left to right labeled "LLM 摘要替换". Below, small text: "target ≤ 15,250 tokens · 50 并发 · 5min/轨迹超时".

LABELS:
- Left: "原始轨迹"
- Right: "压缩后轨迹"
- Protected zones: "保护区" with small text "首尾保留"
- Middle: "CONTEXT SUMMARY" with small text "~750 tokens"

STYLE:
Minimal hand-drawn illustration with a subtle tech edge. Off-white paper background, dark gray sketch lines, muted umbrella yellow as the only accent color, with occasional thin circuit-trace or node-graph line details woven into the composition. Lots of negative space, Notion-like doodle aesthetic meets minimal blueprint hints. No realism, no 3D, no painterly texture, no high saturation, no complex scene, no photographic detail.

ASPECT: 16:9

Add one short Chinese quote in a natural handwritten style near the bottom: "保护首尾，压缩中间，信号不丢"
