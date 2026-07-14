# Prompt 1: Install the Anthropic Data Skill as a Codex Skill

Copy and paste the following into Codex:

```
Context: Codex does not ship with a built-in data analysis skill. Anthropic publishes a Data plugin on GitHub, and inside that plugin is an analyze skill. Use Codex’s @skill-creator skill to adapt that Anthropic analyze skill into a local Codex skill named anthropic-data-analyst.

Instruction:
Use @skill-creator to create a local Codex skill named anthropic-data-analyst at .agents/skills/anthropic-data-analyst/SKILL.md. Adapt the content from the analyze skill inside Anthropic’s Data plugin on GitHub. The installed skill must include YAML frontmatter with name: anthropic-data-analyst and a clear description so Codex auto-discovers it on launch.

Input:

https://github.com/anthropics/knowledge-work-plugins/tree/main/data
Output:

.agents/skills/anthropic-data-analyst/SKILL.md

```



After this prompt finishes, restart Codex once so the new skill is auto-discovered before prompt 2.
