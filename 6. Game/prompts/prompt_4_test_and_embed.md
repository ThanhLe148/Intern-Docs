# Prompt 4: Test, Fix, and Embed in the Launch Landing Page

Copy and paste the following into Codex:

```
Context: Bean Run runs in game/ but I want a real browser QA pass before we put it on the landing page, then I need a launch page Maya can use for the Junction opening. The page should introduce the cafe, embed the game, show a top-10 leaderboard, and capture an email for a weekly free-latte draw.

Instruction: First, start the dev server and play three full runs. For each issue (collisions, jump arc, sprite alignment, parallax timing, mobile input, leaderboard, restart, console errors), find the root cause and fix it. Then build a landing/ page that embeds the built game, reads the leaderboard from localStorage, and validates a small email signup form. Store demo signups in localStorage too.

Input:
- The game in game/ and design doc game/DESIGN.md
- Brand bible: brand/bean_theory_brand_bible.md
- Junction address: 2856 Dundas Street West, Toronto
- Leaderboard storage: localStorage key beanRunLeaderboard
- Signup demo storage: localStorage key beanTheorySignupDemo

Output:
- A bug log at game/BUGFIXES.md with each issue, its root cause, and the fix
- Updated game files with the fixes applied, three clean runs with no console errors
- A landing page in landing/ with the game embedded, a top-10 leaderboard, and a working email capture
- Hero copy in Bean Theory voice (no exclamation marks, no "passionate")
- A short landing/README.md noting students should run npm run build in game/ first
```
