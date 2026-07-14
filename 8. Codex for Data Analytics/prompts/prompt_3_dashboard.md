# Prompt 3: Branded Charts and Self-Contained Dashboard

Copy and paste the following into Codex:

```
Context: Findings are clear. Turn them into branded charts and one self-contained HTML dashboard Sofia can open by double-clicking. Use the newly created @anthropic-data-analyst skill to guide the analysis and chart decisions.

Instruction:

Use @anthropic-data-analyst to generate five 1600x1000 PNG charts in charts/ from datasets/lumen_clean.csv: revenue_by_class, attendance_trend, churn_heatmap, time_slot_performance, and instructor_leaderboard. Use the Lumen palette and typography from brand/lumen_pilates_brand_bible.md. Add charts/README.md with a one-sentence description per chart.
Build reports/lumen_dashboard.html, a single self-contained file with a header band, four KPI cards for revenue, classes, members, and churn-risk count, the five charts each with a takeaway, and a “What we’re recommending” section with three placeholder bullets. Use inline CSS, fonts loaded from a CDN, and chart paths relative to the HTML file.


Input:
datasets/lumen_clean.csv
reports/eda_findings.md
brand/lumen_pilates_brand_bible.md

Output:
charts/ folder with five PNGs and charts/README.md
reports/lumen_dashboard.html
```
