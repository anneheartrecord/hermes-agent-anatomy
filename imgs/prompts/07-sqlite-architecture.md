---
type: framework
style: notion
aspect: 16:9
output: /Users/annesheartrecord/Desktop/hermes-agent-anatomy/imgs/07-sqlite-architecture.png
---

SCENE: A diagram showing SQLite storage architecture. Center: a cylindrical database icon labeled "state.db" with "WAL 模式" annotation. Multiple arrows coming in from the left represent concurrent readers/writers: "CLI 会话", "Telegram Bot", "Discord Bot", "Worktree Agent". On the right side, two key mechanisms illustrated: top-right shows "抖动重试" with a small zigzag line and text "20ms~150ms random jitter" to break convoy effect; bottom-right shows "被动 Checkpoint" with a small arrow labeled "PASSIVE" and text "每50次写入". Below the database, a virtual table icon labeled "FTS5 全文搜索" with trigger arrows connecting it to the main messages table.

LABELS:
- Center: "state.db" with small text "WAL · 多读单写并发"
- Top-right: "抖动重试" with small text "打破护航效应"
- Bottom-right: "被动 Checkpoint" with small text "永不阻塞"
- Bottom: "messages_fts" with small text "FTS5 · 触发器自动同步"

STYLE:
Minimal hand-drawn illustration with a subtle tech edge. Off-white paper background, dark gray sketch lines, muted umbrella yellow as the only accent color, with occasional thin circuit-trace or node-graph line details woven into the composition. Lots of negative space, Notion-like doodle aesthetic meets minimal blueprint hints. No realism, no 3D, no painterly texture, no high saturation, no complex scene, no photographic detail.

ASPECT: 16:9

Add one short Chinese quote in a natural handwritten style near the bottom: "随机抖动，优雅并发"
