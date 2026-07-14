# Prompt 0: Project Setup

> **Instructor note:** One-time. Codex installs Python if missing, builds a venv, registers a Jupyter kernel. Kick this off during the opening so it finishes in the background.

## Step 1: Make a Project Folder

Drop the dataset titled "retail_sales.xlsx" into a new folder
```


## Step 2: Paste This Prompt

```
Context: I'm starting a forecasting project. I may or may not have Python installed. I want a clean working environment in this folder.

Instruction: Set up everything I need. If Python is missing, install it. Create a venv in this folder, install the packages below, register a Jupyter kernel, point VS Code at the venv, and write a short AGENTS.md. Self-heal on install failures.

Input:
- venv name: venv (project root)
- packages: pandas, numpy, openpyxl, matplotlib, statsmodels, pmdarima, prophet, jupyter, ipykernel
- kernel display name: "Python (venv)"

Output: working venv, kernel registered. Print one line per package with its version when done.
```
