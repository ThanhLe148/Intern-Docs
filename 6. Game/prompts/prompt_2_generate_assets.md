# Prompt 2: Generate All Sprites and Parallax Backgrounds

Copy and paste the following into Codex:

```
Context: We have game/DESIGN.md and the reference pack in assets/reference/. Now generate every sprite for Bruno and the enemy and power-up roster, then the three parallax cafe backgrounds. Everything must look like one illustrator drew it.

Instruction: Generate Bruno's sprites first using the reference pack as the locked style anchor. Then generate every enemy and power-up from the design doc in the same style. Anchor each sprite at bottom-center on transparent background. After sprites, generate three horizontally tileable cafe backgrounds (far, mid, near). The mid layer should show a Bean Theory chalkboard with drink names from the brand bible.

Input:
- Reference pack: assets/reference/bruno_reference.png, bruno_pose_sheet.png, cafe_environment_reference.png, ASSET_BRIEF.md
- Game roster: assets/reference/ASSET_BRIEF.md and game/DESIGN.md
- Brand bible: brand/bean_theory_brand_bible.md

Output:
- assets/sprites/ with the full Bruno run cycle, idle, jump, stumble, plus enemies and power-ups
- assets/sprites/sprite_manifest.json mapping stable Phaser asset keys to file paths
- assets/sprites/STYLE.md capturing locked palette, line weight, and shading for future sprite additions
- assets/backgrounds/ with three horizontally tileable PNGs (far, mid, near)
- assets/backgrounds/background_manifest.json with stable Phaser asset keys
- assets/backgrounds/PARALLAX.md noting recommended scroll speeds per layer
```
