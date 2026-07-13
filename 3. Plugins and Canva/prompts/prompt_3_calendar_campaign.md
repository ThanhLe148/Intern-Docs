# Prompt 3: Schedule the Campaign in Google Calendar

Copy and paste the following into Codex:

```
Context: The three launches in output/launch_plan.md need a campaign timeline I can actually see on a calendar. Each launch needs an announcement post 10 days before the launch date, a launch day reminder on the launch date itself, and a follow-up testimonial post 5 days after launch. That is three events per launch, nine events total.

Instruction: Read output/launch_plan.md. For each of the three classes, create three Google Calendar events on my primary calendar (or on a calendar named "Lumen Marketing" if I created one). Use clear titles like "Slow Wake announcement post" and "Slow Wake launch day" and "Slow Wake follow-up testimonial." Set each event to 9:00 AM Central Time, 30 minutes long. In each event description, write a one-paragraph reminder of what I should do that day in Sofia's voice. After all nine events are created, write a single timeline doc that shows the full six-week campaign with every date and event title in chronological order. Use @google calendar to create the events.

Input:
- output/launch_plan.md
- output/canva_summary.md (so the announcement reminder can reference the carousel)

Output:
- Nine Google Calendar events created across the three launches
- output/campaign_timeline.md showing the full six-week campaign in chronological order with date, event title, and the one-line reminder for each
```
