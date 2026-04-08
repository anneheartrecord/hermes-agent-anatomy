---
type: framework
style: notion
aspect: 16:9
output: /Users/annesheartrecord/Desktop/hermes-agent-anatomy/imgs/06-adapter-hierarchy.png
---

SCENE: A class hierarchy diagram. At the top, a base class box "BasePlatformAdapter" with 4 abstract methods listed (connect, disconnect, send, get_chat_info) and 6 optional methods. Below it, 5-6 concrete adapter boxes arranged in a row, connected by inheritance arrows: TelegramAdapter (2718行), DiscordAdapter (2827行), FeishuAdapter (3589行), SlackAdapter (1361行), WeCom (1342行), and a "..." box for others. Each adapter box has a small icon representing its connection method (long polling, WebSocket, Socket Mode). Shared base capabilities listed at the bottom: retry, typing indicator, media extraction, message truncation.

LABELS:
- Top: "BasePlatformAdapter" with small text "4 abstract + 6 optional"
- Each adapter with line count
- Bottom shared: "共享能力" with small text "重试 · typing · 媒体提取 · 智能分片"

STYLE:
Minimal hand-drawn illustration with a subtle tech edge. Off-white paper background, dark gray sketch lines, muted umbrella yellow as the only accent color, with occasional thin circuit-trace or node-graph line details woven into the composition. Lots of negative space, Notion-like doodle aesthetic meets minimal blueprint hints. No realism, no 3D, no painterly texture, no high saturation, no complex scene, no photographic detail.

ASPECT: 16:9

Add one short Chinese quote in a natural handwritten style near the bottom: "最小契约，最大自由"
