# Week 3 — What You Need

This folder has the one file you'll work with all session: **`retail_sales.xlsx`**.

## Before the Session

1. Make sure you have Claude Code installed.
2. Make a folder on your Desktop: `~/Desktop/forecasting_project`
3. Move `retail_sales.xlsx` into that folder.

Don't open the workbook yet — Prompt 1 walks you through it.

## What's in the Workbook

| Sheet | What's there |
|---|---|
| **Overview** | Plain-English narrative — what the file is and how to forecast it |
| **History** | 1,560 weekly rows: 3 stores × 5 categories × 104 weeks |
| **Future Calendar** | 8 weeks ahead with known driver values (price, marketing, holidays) |
| **Data Dictionary** | Every column explained in plain English |

## During the Session

Your instructor shares the prompts. Paste each into Claude Code in order:

1. **Prompt 0 — Setup** (creates a Python venv and installs packages)
2. **Prompt 1 — Explore** (writes a briefing and adds a Charts sheet)
3. **Prompt 2 — Forecast with Backtest** (ARIMA + SARIMA + Prophet, picks the winner per series, writes the 8-week forecast back to Excel)

You end the session with:
- `retail_sales.xlsx` — now with new sheets: Charts, Backtest Results, Forecast, Forecast vs Actuals, Forward Forecast
- `briefing.md` — your written read on the data
- A working venv and a notebook in your folder

Nothing else. No loose Python files. Everything's inside Excel.

## If You Don't Have Python

That's fine. Prompt 0 checks for Python and installs it for you (Homebrew on macOS, or it points you to python.org on Windows). You don't need to do anything ahead of time.
