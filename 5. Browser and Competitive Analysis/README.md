# Project 04: Casa Verde Competitive Intelligence

You are running competitive intelligence for Casa Verde Studio, a sustainable interior design firm in Austin. Codex researches 5 Austin firms live, synthesizes the landscape, then produces three Casa Verde branded deliverables: an internal positioning PPT, a client-facing white paper PDF, and a shareable infographic. Four prompts.

## Setup (5 minutes)
1. Copy this folder anywhere you like
2. Confirm the casa-verde skill is sitting at `.agents/skills/casa-verde/SKILL.md`. The kit ships with it pre-installed. If you completed Project 03, you already have a working version. Either path is fine because Codex auto-loads anything under `.agents/skills/` when you launch it from this folder
3. Confirm browser automation is connected (Playwright MCP, Chrome MCP plugin, or computer use, whichever you use)
4. Confirm image generation is available for the infographic, or HTML/CSS render to PNG works on your setup
5. Install the pptx skill or have python-pptx available for the deck
6. Launch Codex from this folder so the casa-verde skill auto-loads
7. Paste prompts in order from `prompts/`. Prompt 1 has Codex write its own AGENTS.md before defining the research framework

## How the five firms get picked
You do not start with a list. In Phase 2a of prompt 2, Codex discovers 5 Austin-area firms that match Casa Verde's competitive set (sustainable residential interior design, honest materials, comparable budget range, Austin or nearby Hill Country). Codex writes the shortlist with rationale to `output/competitor_shortlist.md`. Then Phase 2b does the deep dive on those 5. Some sites or Instagram pages may be offline, slow, or private. Document what you cannot reach rather than guessing.

## What's in this folder
| Path | What it is |
|---|---|
| `.agents/skills/casa-verde/` | The Casa Verde brand skill, pre-installed. Codex auto-loads this |
| `brand/casa_verde_brand_bible.md` | Full Casa Verde brand bible for reference |
| `templates/competitor_research_schema.md` | Starting schema for the research framework |
| `prompts/` | Four prompts to paste, in order |

## What you'll build
- An AGENTS.md written by Codex itself in prompt 1
- `output/research_framework.md`, the explicit research contract, with Competitor Discovery criteria up front
- `output/competitor_shortlist.md`, the 5 firms Codex discovered with a one-line rationale per firm and the candidates it rejected
- `output/competitors/<slug>.md`, one file per firm, website plus Instagram data
- Screenshots in `assets/screenshots/websites/` and `assets/screenshots/instagram/`
- `output/comparison.md`, the side-by-side synthesis with a positioning map
- `output/casa_verde_positioning_deck.pptx`, the internal branded deck for Elena's team
- `output/deck_summary.md`, slide titles and key takeaways
- `output/austin_sustainable_design_2026.pdf`, a 4 to 6 page Casa Verde branded white paper
- `output/austin_sustainable_design_infographic.png`, a single-page shareable visual
- `output/sharing_blurbs.md`, Instagram, email, and LinkedIn copy to share the white paper

## Output format requirements
- Every cell in the comparison is real data or "unknown" with the source you tried. Never guess
- Every customer-facing output (deck copy, PDF body, infographic copy, sharing blurbs) applies the casa-verde skill
- No em-dashes anywhere
- No exclamation marks anywhere
- No banned vocabulary (luxury, premium, elevated, curated, bespoke, transform, stunning, gorgeous, wow factor, dream home)
- "Design that breathes." appears at most once per piece

## If something breaks
- A firm site is offline: Codex captures the failure, notes it, continues with what is available
- Instagram is private: capture the wall, note it, do not log in
- Screenshot tool returns blank: retry once, then move on with a note
- Branded outputs sound generic: re-read the casa-verde skill at `.agents/skills/casa-verde/SKILL.md` and ask Codex to grep the avoid-word list against the deck or PDF, then rewrite any hits
- Brand colors look like generic gray: regenerate using the exact hex codes from `brand/casa_verde_brand_bible.md`
- "Design that breathes." appears in every section: the skill says once per piece. Tell Codex to grep and remove duplicates
