---
type: framework
style: notion
aspect: 16:9
output: /Users/annesheartrecord/Desktop/hermes-agent-anatomy/imgs/01-hermes-sqlite-wal.png
---

ZONES:
- A database cylinder icon on the left labeled SQLite
- Three horizontal lanes extending to the right representing concurrent access
- Top two lanes show multiple small eye icons (readers) running in parallel
- Bottom lane shows a single pen icon (writer) with a WAL file buffer between it and the database
- Small dice icons near the writer representing jittered retry (20-150ms)
- A checkpoint marker every few writes

LABELS:
- Database: "SQLite + FTS5"
- Top lanes: "Reader 1", "Reader 2" with text "WAL 并发读"
- Bottom lane: "Writer" with text "抖动退避 20-150ms"
- WAL buffer: "Write-Ahead Log"
- Checkpoint marker: "每 50 次写入 PASSIVE checkpoint"

COLORS:
- Off-white paper background
- Dark gray sketch lines
- Muted umbrella yellow accent on the WAL buffer and checkpoint markers
- No other colors

STYLE:
Minimal hand-drawn illustration with a subtle tech edge. Off-white paper background, dark gray sketch lines, muted umbrella yellow as the only accent color, with occasional thin circuit-trace or node-graph line details. Lots of negative space, Notion-like doodle aesthetic. No realism, no 3D.

ASPECT: 16:9

Add one short Chinese quote in a natural handwritten style near the bottom: "并发不靠锁，靠WAL"
