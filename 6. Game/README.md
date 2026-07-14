# Project: Bean Theory Arcade

You'll build a branded Phaser arcade game starring Bruno the Bean for Bean Theory Coffee's Junction location, then embed it in a launch landing page with leaderboard and email capture.

## Setup (2 minutes)
1. Copy this folder anywhere you like
2. Install the Codex CLI and ensure image generation is enabled. Make sure the Game Studio plugin is installed and active
3. Launch Codex from this folder
4. Paste prompts in order from `prompts/`. Prompt 1 will have Codex write its own AGENTS.md before producing the reference pack and design doc

## What's in this folder
| Path | What it is |
|---|---|
| `brand/` | Brand bible for Bean Theory Coffee |
| `assets/` | Empty starter folders for references, sprites, backgrounds, and UI |
| `prompts/` | Four prompts to paste, in order |

## What you'll build
- An AGENTS.md written by Codex itself in prompt 1
- A reference asset pack in `assets/reference/` and `game/DESIGN.md`
- A full sprite roster anchored on Bruno, plus three parallax cafe backgrounds
- A working Phaser, TypeScript, and Vite game in `game/`, with leaderboard via localStorage
- A landing page in `landing/` with the game embedded and an email capture form

## If something breaks
- Style drift across sprites: regenerate the off sprite while explicitly referencing `assets/sprites/bruno_run_1.png` as the style anchor
- Parallax seams visible: regenerate that background with the phrase "horizontally tileable, left edge matches right edge"
- Jumping feels floaty: adjust gravity or jump velocity in `game/src/systems/playerSystem.ts` and re-test
- Hero copy reads like Mailchimp: rewrite with the Sample Voice section of the brand bible pasted directly into the prompt
