---
type: framework
style: notion
aspect: 16:9
output: /Users/annesheartrecord/Desktop/hermes-agent-anatomy/imgs/03-tool-dispatch-flow.png
---

SCENE: Tool 分发流程: 左侧 LLM 返回 tool_use block, 箭头进入中间 dispatcher 方块(内含 name→handler map 查找), 右侧分叉到三条路径: 同步执行/异步执行/权限拦截, 每条路径末端汇回 result collector

STYLE:
Minimal hand-drawn illustration with a subtle tech edge. Off-white paper background, dark gray sketch lines, muted umbrella yellow as the only accent color, with occasional thin circuit-trace or node-graph line details woven into the composition. Lots of negative space, Notion-like doodle aesthetic meets minimal blueprint hints. No realism, no 3D, no painterly texture, no high saturation, no complex scene, no photographic detail.

ASPECT: 16:9

Add one short Chinese quote in a natural handwritten style near the bottom: "分发的本质是名字到函数的映射"
