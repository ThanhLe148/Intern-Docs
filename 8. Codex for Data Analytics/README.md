# Project 07: Data EDA with the Anthropic Plugin

You are the analyst at Lumen Pilates. Sofia handed you 18 months of messy transaction data. Codex does not ship with a built-in data analysis skill, so you point it at the Anthropic skills repo on GitHub, read the data skills, build your own local skill scoped to Lumen, and run a full clean-and-EDA pass.

The lesson behind this project: skills are not magic. They are markdown files that other people wrote first. You will adapt them 90 percent of the time, not write them from scratch.

## Setup (3 minutes)

1. Copy this folder anywhere you like.
2. Set up a Python environment. Python 3.10 or newer.
   ```bash
   cd 07_data_eda_anthropic_plugin
   python3 -m venv .venv
   source .venv/bin/activate
   pip install pandas matplotlib seaborn jinja2
   ```
3. Confirm Codex CLI is installed and signed in. Codex auto-discovers project skills at `.agents/skills/<name>/SKILL.md` only at launch, so you must restart Codex after prompt 1 finishes.
4. Confirm Codex can fetch from GitHub. The reference repo lives at **https://github.com/anthropics/skills**. The data skills sit under `data/`. If your network blocks `raw.githubusercontent.com`, clone the repo into a `_reference/skills/` folder and have Codex read from disk.
5. Launch Codex from this folder.
6. Paste prompts in order from `prompts/`. Four files total. Restart Codex once after prompt 1 so the newly installed data skill is registered before prompts 2 through 4 reference it.

## What's in this folder

| Path | What it is |
|---|---|
| `brand/lumen_pilates_brand_bible.md` | Lumen brand reference for chart styling and the executive summary voice |
| `datasets/lumen_messy_18months.csv` | 18 months of transactions, around 2,800 rows. Intentionally messy. |
| `prompts/` | Four step-by-step prompts |

The prompts will create `reports/`, `charts/`, and the skill folder `.agents/skills/<name>/` (with `SKILL.md` inside) at the project root.

## What you'll build

- A local Codex skill at `.agents/skills/<name>/SKILL.md`, installed via `@skill-creator` from the Anthropic skills repo, with YAML frontmatter so Codex auto-discovers it
- `datasets/lumen_clean.csv` plus a data quality report covering every fix applied
- `reports/eda_findings.md` with revenue by class, attendance trend, churn risk, and time slot performance
- Five branded charts in `charts/`
- A self-contained dashboard at `reports/lumen_dashboard.html`
- A one-page executive summary at `reports/sofia_summary.md` that Sofia could read on her phone

## If something breaks

- Skill not auto-discovered after prompt 1: skills are folders, not flat files. Confirm the file lives at `.agents/skills/<name>/SKILL.md` (not a flat file at the root) and that `SKILL.md` starts with YAML frontmatter (`name`, `description`). Restart Codex.
- GitHub fetch blocked: clone the Anthropic skills repo into `_reference/skills/` and tell Codex to read from disk.
- Charts look generic: the most common cause is matplotlib defaulting to its own font. Set `rcParams` explicitly in the script.
- Wrong numbers in EDA: skipping the cleaning step. Run prompt 2 fully before any chart prompt.
- Dashboard image paths broken: Codex sometimes outputs absolute paths. Force relative paths from `charts/`.
- Canela not on your machine: Cormorant Garamond from Google Fonts is the free fallback. Söhne falls back to Inter.
