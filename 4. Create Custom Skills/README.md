# Project: Casa Verde Brand Skill

You'll turn Casa Verde Studio's brand bible into a working Codex skill, test it on three real-world outputs (welcome email, proposal cover, Instagram caption), refine the skill based on what drifted, and apply it to a one-page landing page. Four prompts.

## Setup (2 minutes)
1. Copy this folder anywhere you like
2. Install the Codex CLI
3. Confirm the 6 pre-generated brand images are inside `assets/` (your instructor generated them before class and shipped them with this kit)
4. Launch Codex from this folder
5. Paste prompts in order from `prompts/`. Prompt 1 will have Codex write its own AGENTS.md before producing the skill
6. After prompt 1 finishes, restart Codex once. Codex auto-discovers project skills in `.agents/skills/<name>/SKILL.md` on launch, so the casa-verde skill becomes available for prompts 2 through 4 only after a restart

## What's in this folder
| Path | What it is |
|---|---|
| `brand/` | Brand bible for Casa Verde Studio |
| `assets/` | Six pre-generated Casa Verde brand images, do not regenerate |
| `prompts/` | Four prompts to paste, in order |

The brand assets are pre-generated. You do not generate new images in this project. You build a brand skill that knows when and how to reach for these visuals. Project 09 is where you do your own image generation work.

## What you'll build
- An AGENTS.md written by Codex itself in prompt 1
- `.agents/skills/casa-verde/SKILL.md`, the working brand skill, with YAML frontmatter (name, description) so Codex knows when to apply it
- `outputs/welcome_email_acharyas.md`, a client welcome email
- `outputs/proposal_cover_acharyas.md`, a one-page proposal cover
- `outputs/instagram_beck_residence.md`, an Instagram caption with hashtags and alt text
- `outputs/skill_review.md` and `.agents/skills/casa-verde/CHANGELOG.md`, the iteration log
- A refined `.agents/skills/casa-verde/SKILL.md` (overwritten in prompt 3)
- A one-page landing site at `landing/index.html`

## If something breaks
- Outputs use "luxury," "transform," or "stunning": the skill's Avoid list is not strict enough. Re-run prompt 3 and tell Codex to harden it
- Signature phrase appears twice on one page: add an explicit "use only once per piece" line to the skill
- Hashtags drift to #luxuryhome: hashtag rules were missing from skill v1. Surface this in prompt 3
- Caption sounds like a brand account, not Elena: paste the Sample Voice section directly into the prompt
