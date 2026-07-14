## Step 1: Paste This Prompt into Codex

```
@OpenAI Developers 

Context: I'm starting a new Python project using the OpenAI Agents SDK. I need an isolated environment set up before writing any code. I use VS Code (or Cursor/Windsurf) to open notebooks.

Instruction: Create a Python virtual environment in the project folder, install the required packages, register it as a Jupyter kernel, configure VS Code to use it as the default Python interpreter, and create a .env file for API keys.

Input:
- Virtual environment name: venv (must be in the project root so VS Code auto-discovers it)
- Packages: openai-agents, python-dotenv, ipykernel
- Register kernel: python -m ipykernel install --user --name=venv --display-name="Python (venv)"
- Create .vscode/settings.json with "python.defaultInterpreterPath" pointing to venv/bin/python
- .env file with placeholder: OPENAI_API_KEY=your-openai-api-key-here

Output: A ready-to-use project environment with venv created in the project folder, packages installed, Jupyter kernel registered, VS Code configured to auto-select the venv, and .env file created.
```

---

## Step 2: Add Your API Key

Open the `.env` file Claude Code created and replace the placeholder with your real key:

```
OPENAI_API_KEY=sk-your-actual-key-here
```

> Get an API key from [platform.openai.com](https://platform.openai.com/).

