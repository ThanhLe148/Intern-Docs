# Prompt 1: Setup and Build the Casa Verde Brand Skill

Copy and paste the following into Codex:

```
Context: Elena Reyes runs Casa Verde, a sustainable interior design studio in Austin. Her brand bible already exists. I want to turn it into a Codex skill so anyone on her team or any freelancer with Codex access can produce on-brand work without re-asking what Casa Verde sounds like.

Instruction: First, read brand/casa_verde_brand_bible.md and README.md, then write AGENTS.md in this folder capturing the project goal, Casa Verde's voice rules, the signature phrase "Design that breathes." (used once per piece), avoid vocabulary, conventions (no em-dashes, sign-off "Elena"), and the workflow (we will paste prompts 1 through 4). Then build a working skill at .agents/skills/casa-verde/SKILL.md. Write YAML frontmatter at the top of SKILL.md with two keys: name (casa-verde) and description. The description should explain when Codex should reach for this skill (writing emails, proposals, captions, landing pages for Casa Verde) and when it should NOT (any non-Casa-Verde content). Make it specific enough to apply to emails, proposals, captions, and landing pages.

Input:
- Brand bible: brand/casa_verde_brand_bible.md
- Pre-generated brand assets in assets/ (hero living room, three material textures, Elena portrait, logo concept). Reference them in the skill, do not regenerate them.

Output:
- AGENTS.md at the project root
- A complete .agents/skills/casa-verde/SKILL.md that reads like a working contract, not an internal style guide
- Include voice rules, do and don't vocabulary, palette, type, materials, sign-off conventions, sample voice (3 from the bible plus 3 new ones), and notes on when to reference each pre-generated asset
- Keep the skill under 350 lines, cut anything that's filler
```

After this prompt finishes, restart Codex once so the new skill is auto-discovered before you paste prompt 2.
