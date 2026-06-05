# Hexagon

A memory + mental-arithmetic puzzle inspired by *The Devil's Plan*. Memorize a honeycomb of 19 numbers, then — once they vanish — find **three touching tiles that add up to the target**. Score as many combos as you can before the clock runs out.

**[Play now](https://shrihari1999.github.io/hexagon/)**

## How to play

1. Pick a difficulty and hit **Play**.
2. **Memorize** the numbers on the 19-tile hexagonal board (or tap *I'm ready* to start early).
3. The numbers vanish. Tap **three tiles in a straight line** (along any hex axis) whose hidden values sum to the **target**.
4. Correct **new** combo → **+1** (with a streak bonus); wrong → **−1**; repeating a combo you already found also costs **−1**. Find them all!

## Features

- 19-tile hexagonal board with straight-line selection along the three hex axes (built on axial coordinates, rendered as crisp scalable SVG)
- **Memorize → Solve** two-phase rounds with live countdown bars
- Three difficulties (Easy / Medium / Hard) — each tunes memorize time, solve time, target range, and peeks
- **Streak bonuses** — every third consecutive correct combo is worth extra points
- Limited **Peeks** — briefly flash the numbers back when your memory fails you
- Guaranteed-solvable boards (every board has at least one valid combo)
- Found-combo tracker, duplicate combos penalized (−1, like the original), and an end-of-round summary
- Per-difficulty **best score**, saved locally
- Fully responsive, touch-friendly, and installable as a **PWA** — no build step, no backend, single-player only

## Tech

Plain HTML/CSS/vanilla JS in a single file — no framework, no build. Served as a static site from the `docs/` folder for GitHub Pages.

## Local development

```bash
cd docs
python3 -m http.server 8000
# open http://localhost:8000
```
