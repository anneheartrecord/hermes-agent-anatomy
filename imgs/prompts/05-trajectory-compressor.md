---
type: framework
style: notion
aspect: 16:9
output: /Users/annesheartrecord/Desktop/hermes-agent-anatomy/imgs/05-trajectory-compressor.png
---

SCENE: 左右对比两个压缩器。左侧"context_compressor.py(在线)"：一个Agent循环图标连着一个小压缩器，标注"单次同步·粗估token·200K窗口"。右侧"trajectory_compressor.py(离线)"：一堆ShareGPT格式的训练数据文件流入一个大压缩器，标注"50并发·精确tokenizer·15K目标"。两者之间用虚线分隔，顶部标签分别是"对话进行中"和"训练前批处理"。底部右侧有一个小的HuggingFace logo轮廓。

STYLE:
Minimal hand-drawn illustration with a subtle tech edge. Off-white paper background, dark gray sketch lines, muted umbrella yellow as the only accent color, with occasional thin circuit-trace or node-graph line details woven into the composition. Lots of negative space, Notion-like doodle aesthetic meets minimal blueprint hints. No realism, no 3D, no painterly texture, no high saturation, no complex scene, no photographic detail.

ASPECT: 16:9

Add one short Chinese quote in a natural handwritten style near the bottom: "在线求快，离线求准"
