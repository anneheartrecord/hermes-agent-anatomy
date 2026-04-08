---
type: framework
style: notion
aspect: 16:9
output: /Users/annesheartrecord/Desktop/hermes-agent-anatomy/imgs/06-session-store.png
---

SCENE: A vertical flow diagram showing session lifecycle. At the top, a user message arrives. It flows into a decision diamond "session exists?". Two paths branch: "yes + not expired" leads to "reuse session" box, "yes + expired" leads to a sequence of "flush memories → create new". "No session" leads directly to "create new". Below all paths merge into an active session box. A separate background watcher loop on the right side shows "every 5 min scan → check expiry → flush memories". Session keys shown as small code snippets: "agent:main:telegram:dm:12345".

LABELS:
- Top: "用户消息到达"
- Diamond: "会话存在？"
- Left path: "复用已有会话"
- Middle path: "记忆刷写 → 新建会话"
- Right watcher: "后台 Watcher" with small text "每5分钟扫描"
- Bottom: "活跃会话" with small text "per-user per-platform 隔离"

STYLE:
Minimal hand-drawn illustration with a subtle tech edge. Off-white paper background, dark gray sketch lines, muted umbrella yellow as the only accent color, with occasional thin circuit-trace or node-graph line details woven into the composition. Lots of negative space, Notion-like doodle aesthetic meets minimal blueprint hints. No realism, no 3D, no painterly texture, no high saturation, no complex scene, no photographic detail.

ASPECT: 16:9

Add one short Chinese quote in a natural handwritten style near the bottom: "会话隔离，记忆不丢"
