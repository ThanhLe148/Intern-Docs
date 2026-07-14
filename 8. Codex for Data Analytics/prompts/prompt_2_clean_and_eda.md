# Prompt 2: Clean Sofia's Data and Run EDA

Copy and paste the following into Codex:

```
Context: Sofia handed me 18 months of messy transaction data. Use the newly created @anthropic-data-analyst skill. Sofia wants three answers: which classes drive revenue, which members are at churn risk, and which time slots underperform.

Instruction:

Use @anthropic-data-analyst to clean datasets/lumen_messy_18months.csv. Output datasets/lumen_clean.csv and reports/data_quality_report.md listing every fix made.
Use @anthropic-data-analyst to run EDA on datasets/lumen_clean.csv covering revenue by class, attendance trend by month, churn risk segmentation, and time slot performance. Output reports/eda_findings.md with a Headlines section at the top and one section per analysis with a small table and a 2-3 sentence takeaway.
Input:

datasets/lumen_messy_18months.csv


Output:
datasets/lumen_clean.csv
reports/data_quality_report.md
reports/eda_findings.md
```
