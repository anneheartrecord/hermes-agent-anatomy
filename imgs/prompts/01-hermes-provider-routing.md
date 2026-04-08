---
type: framework
style: notion
aspect: 16:9
output: /Users/annesheartrecord/Desktop/hermes-agent-anatomy/imgs/01-hermes-provider-routing.png
---

ZONES:
- A decision tree flowing left to right. Starting node on the left labeled as "请求", branching into 5 paths going right
- Each path leads to a different provider box
- Below the tree, a horizontal bar showing credential pool with 4 small key icons, some marked with checkmarks, one marked with an X (exhausted)
- Small cooldown timer icons next to the exhausted key

LABELS:
- Starting node: "LLM 请求"
- Branch 1: "Nous Portal"
- Branch 2: "OpenRouter"
- Branch 3: "Anthropic"
- Branch 4: "OpenAI"
- Branch 5: "自定义端点"
- Bottom bar: "凭证池: fill_first / round_robin / random / least_used"
- Exhausted key label: "429 → 1h 冷却"
- Another exhausted key: "402 → 24h 冷却"

COLORS:
- Off-white paper background
- Dark gray sketch lines
- Muted umbrella yellow accent on active paths and checkmark keys
- No other colors

STYLE:
Minimal hand-drawn illustration with a subtle tech edge. Off-white paper background, dark gray sketch lines, muted umbrella yellow as the only accent color, with occasional thin circuit-trace or node-graph line details. Lots of negative space, Notion-like doodle aesthetic. No realism, no 3D.

ASPECT: 16:9

Add one short Chinese quote in a natural handwritten style near the bottom: "Key挂了不要紧，池子里还有"
