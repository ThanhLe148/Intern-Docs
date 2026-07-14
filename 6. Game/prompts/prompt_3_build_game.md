# Prompt 3: Build the Playable Phaser Game

Copy and paste the following into Codex:

```
Context: We have the design doc at game/DESIGN.md, sprites in assets/sprites/, and parallax backgrounds in assets/backgrounds/. Build Bean Run as a real browser game that loads quickly on a cafe landing page and works on desktop and mobile.

Instruction: Build the playable game in a game/ directory using Phaser, TypeScript, and Vite. Wire up the run cycle, parallax (using the speeds in PARALLAX.md), jump, collisions, scoring with a localStorage leaderboard, the difficulty curve from the design doc, and mobile touch controls.

Input:
- Design doc: game/DESIGN.md
- Sprite manifest: assets/sprites/sprite_manifest.json
- Background manifest and parallax speeds: assets/backgrounds/background_manifest.json, assets/backgrounds/PARALLAX.md
- Leaderboard storage: localStorage key beanRunLeaderboard

Output:
- A working game in game/ with dev, build, and preview scripts
- All UI copy in Bean Theory voice (e.g. "Best run today: 1,240" not "HUGE SCORE")
- A short game/README.md with how to run it locally
```
