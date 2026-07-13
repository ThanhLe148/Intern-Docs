# Project 02: Lumen Spring Class Launch Campaign

You'll turn a single Google Sheet into a complete six-week launch campaign for three new Lumen Pilates classes. Codex pulls the launch plan, generates three on-brand hero images, builds three Canva carousels, schedules nine calendar events across the campaign, then sends a real launch email to your own inbox so you can preview exactly what members will see. Four prompts, four plugins, one image generation step.

## Setup (10 minutes)
1. Copy this folder anywhere you like
2. Open Google Sheets, create a new spreadsheet titled exactly **Lumen Spring Launch Plan**, and paste in the contents of `datasets/lumen_class_launches.csv` (header row first)
3. Confirm four Codex plugins are connected and pointing at the same Google account: Sheets, Canva, Calendar, and Gmail
4. Launch Codex from this folder
5. Paste prompts in order from `prompts/`. Prompt 1 will have Codex write its own AGENTS.md before anything else

## What's in this folder
| Path | What it is |
|---|---|
| `brand/` | Brand bible for Lumen Pilates |
| `datasets/lumen_class_launches.csv` | Three rows of launch plan data, paste into your Google Sheet |
| `prompts/` | Four prompts to paste, in order |

Codex writes its own `AGENTS.md` at the project root during prompt 1, so you do not need to create one ahead of time.

## What you'll build
- An AGENTS.md written by Codex itself in prompt 1
- Three on-brand hero images in `assets/heroes/`
- Three Canva carousels (four slides each) in your Canva account
- Nine Google Calendar events covering the full six-week campaign
- One real launch email sent to your own Gmail to preview the send

## If something breaks
- Codex says it cannot find the Sheet: the Sheet title is wrong or the Sheets plugin is on a different Google account. Fix the title to exactly "Lumen Spring Launch Plan" and confirm the plugin account
- Canva carousel captions sound like a fitness influencer: paste the Sample Voice section from the brand bible directly into prompt 2 and re-run
- Calendar events land on the wrong calendar: the Calendar plugin defaulted to the wrong calendar. Delete the events and re-run, telling Codex which calendar to use by name
- Calendar event dates look off: the +5 and -10 day math slipped. Cross-check `output/campaign_timeline.md` against the launch dates in `output/launch_plan.md`
- Launch email sounds like Mailchimp: paste the Sample Voice section into prompt 4 and re-run with stronger voice instructions
