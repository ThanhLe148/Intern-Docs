# Prompt 2: Test the Skill on a Welcome Email and Proposal Cover

Make sure you restarted Codex after prompt 1 so the casa-verde skill is auto-discovered. Then copy and paste the following into Codex:


Note to use a skill in Codex you use "@" followed by the name of the skill. Claude supports "/" instead. 
```
Context: We just built .agents/skills/casa-verde/SKILL.md. Now I want to test it on two real Casa Verde scenarios. Daniel and Priya Acharya signed for a $185k renovation of their 1920s Hyde Park bungalow in Austin (living room, dining, primary bedroom). They're first-time renovation clients and a bit nervous. After the welcome email, Elena needs a one-page cover for the proposal PDF that goes before the budget table.

Instruction: Apply the casa-verde skill at .agents/skills/casa-verde/SKILL.md and write both pieces. The welcome email should set the tone for the next six months without pitching services, and reference something specific about a 1920s bungalow. The proposal cover lives in a 30-second-read format with one tangible material reference and one closing line.

Input:
- /casa verde
- Client and project: Daniel and Priya Acharya, 1920s Hyde Park bungalow, $185k
- Available assets: assets/

Output:
- outputs/welcome_email_acharyas.html, around 200 words, with subject line, body, and a short PS that references something tangible from a previous bungalow project. Generate a stunning branded HTML page. 
- outputs/proposal_cover_acharyas.html, body 180 to 230 words, headline under 8 words, one closing line using the signature phrase per the skill, plus a recommended hero image path from assets/ with a one-line caption. Generate a stunning branded HTML page. 



```
