---
type: framework
style: notion
aspect: 16:9
output: /Users/annesheartrecord/Desktop/hermes-agent-anatomy/imgs/07-lifecycle-hooks.png
---

SCENE: A vertical timeline/pipeline diagram showing the MemoryProvider lifecycle from top to bottom. Nodes along the timeline: "initialize" → "system_prompt_block" → a repeating loop section containing "on_turn_start → prefetch → Model推理 → sync_turn → queue_prefetch", the loop has a circular arrow. After the loop: "on_pre_compress" (highlighted with yellow accent, with a small note "抢救即将丢弃的记忆") → "on_session_end" → "shutdown". Side branches show "on_memory_write" and "on_delegation" connecting into the loop from the side.

LABELS:
- Top: "Session Start"
- Loop section: "Turn Loop" with small text "每轮对话"
- Highlighted node: "on_pre_compress" with small text "压缩前提取洞察"
- Bottom: "shutdown" with small text "反序关闭"

STYLE:
Minimal hand-drawn illustration with a subtle tech edge. Off-white paper background, dark gray sketch lines, muted umbrella yellow as the only accent color, with occasional thin circuit-trace or node-graph line details woven into the composition. Lots of negative space, Notion-like doodle aesthetic meets minimal blueprint hints. No realism, no 3D, no painterly texture, no high saturation, no complex scene, no photographic detail.

ASPECT: 16:9

Add one short Chinese quote in a natural handwritten style near the bottom: "每个钩子都有try-except，一个崩溃不拖垮全局"
