---
type: framework
style: notion
aspect: 16:9
output: /Users/annesheartrecord/Desktop/hermes-agent-anatomy/imgs/01-hermes-tool-registry.png
---

ZONES:
- Left side: a vertical stack of 6 small module boxes, each with a tiny emoji icon, representing tool modules
- Center: a large rounded rectangle labeled as the Registry singleton, with thin lines connecting from each module on the left
- Right side: a decision tree with 3 branches going to different outputs (execute, error, async bridge)
- Small node-graph dots at each connection point
- A thin circuit-trace line running along the bottom as decoration

LABELS:
- Left modules (top to bottom): "web_tools", "terminal_tool", "file_tools", "browser_tool", "delegate_tool", "memory_tool"
- Center box: "ToolRegistry 单例" with small text "register() → dispatch()"
- Right branch 1: "同步执行"
- Right branch 2: "异步桥接 → event loop"
- Right branch 3: "check_fn → 不可用"
- Arrow from left to center: "import 时注册"
- Arrow from center to right: "运行时分发"

COLORS:
- Off-white paper background
- Dark gray sketch lines for all elements
- Muted umbrella yellow as the only accent color, used on the Registry box border and arrow tips
- No other colors

STYLE:
Minimal hand-drawn illustration with a subtle tech edge. Off-white paper background, dark gray sketch lines, muted umbrella yellow as the only accent color, with occasional thin circuit-trace or node-graph line details woven into the composition. Lots of negative space, Notion-like doodle aesthetic meets minimal blueprint hints. Clean editorial composition, conceptual rather than literal, simple background. No realism, no 3D, no painterly texture, no high saturation, no complex scene, no photographic detail. The overall mood is restrained, lucid, slightly ironic, and emotionally calm.

ASPECT: 16:9

Add one short Chinese quote in a natural handwritten style near the bottom: "import即注册，朴素但有效"
