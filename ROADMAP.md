# Roadmap — PRJ-002 process and tools

Ideas and planned work for how this project runs: onboarding, automation, notifications and community.
This is not the bill's schedule (see [CALENDAR.md](CALENDAR.md)) and it authorizes nothing.
Items move to the [work board](https://github.com/orgs/RuntimeRepublic/projects/1) when the Human Engineer
schedules them. Contributors may suggest additions by issue (Level 2 and up).

Last updated: 2026-11-03

## Next up

1. **Level 2 bar.** Define "useful, sourced review comments" in [ONBOARDING.md](ONBOARDING.md)
   (for example: two comments on different clauses; factual or legal claims cite a source; opinions are labeled "Opinion:").
2. **Docs catch-up.** ONBOARDING and SPEC-003 §18.1 still say ZIP code and districts are asked at Level 2;
   they are now collected privately in the Readiness Check form.

## Onboarding automation

3. **Welcome bot.** When an onboarding issue opens: a welcome comment with the quiz link and next steps.
4. **Private details form.** Contact details go to the Human Engineer's private records, never to GitHub;
   the issue's Step 4 box is checked automatically.
5. **Roster file.** A public `members/ROSTER.md` (GitHub username, level, steps done, next step) updated automatically,
   so each member's AI assistant can read their status from a synced file.
6. **Quiz helper prompts.** "Need help? Paste this into Claude" text under each quiz question, linking the exact lesson.
   The prompts explain the lesson; they never give the answer.
7. **Branch protection on `main`**, and Level 3 by pull request from a fork (only the Human Engineer merges).
8. **Label guard.** Level labels can only be added by the Human Engineer.
9. **Stale reminders and a weekly roster report.**
10. **A RuntimeRepublic bot account (GitHub App)** for automated comments.

## Notifications and dashboard

11. **Daily check-in** for the Human Engineer: what needs a decision, merges waiting, days to the November 30 draft freeze.
12. **Project dashboard (web page):** countdown, current phase and gate, Phase 1 task status, members per level
    (usernames only), latest press releases. Public information only.

## Guided checklists

13. **Step-by-step checklists**, checked off one box at a time:
    - Set up your AI assistant project (Claude, ChatGPT or Grok) for PRJ-002
    - Get the most from Facebook and Runtime Republic
    - X, GETTR, Discord and other channels

## Community

14. **Discord proposal** (to be opened by a Level 2 contributor). GitHub activity can post to a Discord channel
    automatically. Proposed standard: Discord is for conversation and GitHub is the record; no votes or decisions
    in Discord; officeholders follow the Kansas Open Meetings Act caution (SPEC-003 §18.3(1)); no personal details;
    Level 1 and up.

## Bill tracking and review (after the November 30 draft)

15. **Bill Watch for the 2027 Kansas session (Level 1).** Members follow their own legislators, record when each
    version of a bill's text was posted and when it was voted on, flag gut-and-go replacements, cover one committee,
    and send a short weekly note. Every entry has a source link. Track the process, not the politics.
16. **Nonpartisan bill review standard.** One checklist applied the same way to any bill in any state or Congress:
    clarity, single subject, definitions, text posted in time, fiscal note, enforceability, constitutional questions,
    unintended effects. Reviews suggest improvements clause by clause and never support or oppose a bill.
17. **Bill tracker templates.** A Google Sheet anyone can copy: enter bill numbers, and a daily script records each new
    version with its time stamp, status changes and votes, and sends an email when the text changes.

## Later

18. **Website:** Join and Press pages on RuntimeRepublic.com.
19. **Video:** a short walkthrough of setting up an AI assistant project.
20. **Podcast:** narrated essays (Republic Radio).
21. **"My Runtime Republic" web app:** members see their level and next step, and get notices when a watched bill
    changes. Its own project and specification, after the November 30 draft freeze.
