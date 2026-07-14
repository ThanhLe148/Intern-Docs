# Prompt 1: Explore the Data

> **Instructor note:** Read the file, write a short briefing, drop charts into Excel as embedded images. Works on the retail workbook (3 stores × 5 categories, 104 weeks).

## Paste this into Claude Code (venv active)

```
Context: I have an Excel workbook in the dataset/ folder with weekly sales history across multiple stores and categories. I want to understand it before forecasting.

Instruction: Read the workbook in dataset/. Use the Data Dictionary sheet to understand each column. Write a short briefing on what the data shows. Then add a Charts sheet with embedded images so the picture is visible inside Excel.

Input:
- The Excel file in dataset/ (e.g. dataset/retail_sales.xlsx)
- Use the Data Dictionary sheet to interpret columns

Output:
- briefing.md with: one-paragraph summary, per-category read, three things worth investigating, holiday and stockout effects.
- A new Charts sheet inside the workbook with embedded images:
  - per-category trend (one line per category)
  - small-multiples grid: one panel per store/category, holiday weeks marked
  - discount sensitivity scatter per category
- Keep the briefing direct. No filler.
```

> **Instructor note:** Walk the class through `briefing.md` and the Charts sheet. Point out the holiday lifts (Seasonal +120%, HomeCare +35%), the discount sensitivity (Snacks and Essentials respond strongly), and the stockout impact (~22% units lost).
