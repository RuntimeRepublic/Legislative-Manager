# Onboarding — Join PRJ-002, the Kansas One-Hour Posting Rule
Work board: https://github.com/orgs/RuntimeRepublic/projects/1

**Status:** v0 (bootstrap). Some steps are checked by hand until automation is built.
**Governed by:** SPEC-003 §18 (Contributor Readiness and Access). If this page and SPEC-003 conflict, SPEC-003 wins.

This page is the single path for new collaborators **and their AI assistants**.
If you are an AI assistant helping someone join, read this whole page, then help them
find the first unchecked box on their onboarding issue (Step 3).

---

## The path at a glance

| Step | What you do | Evidence left behind | Who checks it |
|---|---|---|---|
| 1 | Create a GitHub account | Your GitHub username | — |
| 2 | Read the course | — | — |
| 3 | Open your onboarding issue | The issue (public) | — |
| 4 | Send private details to the Human Engineer | A "received" note on your issue (no details) | Human Engineer |
| 5 | Take the Readiness Check | A "Readiness Check passed" note on your issue | Human Engineer |
| 6 | Set up your AI assistant (recommended) | A checked box on your issue | You (self-reported) |
| 7 | Receive Level 1 | A `level-1` label and a recorded grant | Human Engineer |

Then you move up to Level 2 and Level 3 by doing useful work (SPEC-003 §18.2).

---

## Step 1 — GitHub account

Create a free account at [github.com](https://github.com). That is the only account required to start.

## Step 2 — Learn the goal

Read this free course in the Runtime-Republic Training repository. Each lesson takes about three minutes:

- [*The One-Hour Rule*](https://github.com/RuntimeRepublic/Runtime-Republic-Training/tree/main/Courses/one-hour-rule), Lessons 01–05

Recommended, not required: [*Reading the Draft*](https://github.com/RuntimeRepublic/Runtime-Republic-Training/tree/main/Courses/reading-the-draft), Lessons 01–02.

## Step 3 — Open your onboarding issue

[Open an issue using the **Onboarding** template](https://github.com/RuntimeRepublic/Legislative-Manager/issues/new?template=onboarding.md).
Title it `Onboarding: <your GitHub username>`. This issue is your public record. Every
later step leaves a note or label on it, so anyone (including your AI assistant) can see
where you are.

## Step 4 — Private details (never in GitHub)

**Do not post any of the following in an issue, comment or file.** This repository is public
and permanent. Send them privately to the Human Engineer using the method he gives you on
your onboarding issue:

| Required | Optional |
|---|---|
| Your name | Phone number |
| Email address | |
| Preferred way to be contacted | |
| Whether you are a **private citizen** or an **officeholder** (and which public body) | |

Your state and U.S. congressional district are asked on the Readiness Check form (Step 5).
Later, at Level 2, you will also be asked for your ZIP code and your districts. To find your
districts, enter your own address in the U.S. Census Bureau's
[Census Geocoder](https://geocoding.geo.census.gov/geocoder/geographies/address?form)
and report only your ZIP code, U.S. House district, Kansas Senate district and Kansas House
district. Never send or post your street address.

At Level 2 you may also share two **optional** details. Skipping them never affects your access.

| Optional | Why we ask |
|---|---|
| Your voting precinct, as shown on your own voter registration (Kansas VoterView, linked from your county election office) | To organize local outreach. Precincts change, so report what your registration says today. |
| Political party: Republican, Democrat, Libertarian, Unaffiliated, Other, or "prefer not to say" | PRJ-002 is nonpartisan. Party is used only in totals (for example, "reviewers are 40% R, 35% D, 25% unaffiliated") to show balance. It is never used for access, and it is never shown in GitHub as a team, label or note about you. |

The Human Engineer will comment "Private details received" on your issue. Nothing more.

## Step 5 — Readiness Check (SPEC-003 §18.1)

The Human Engineer posts the link to a short Google Form on your onboarding issue. It takes
about five minutes:

- **Three questions** about the *gut and go* and why the One-Hour Rule ends secret action.
  You need all three right. You may retake it.
- **Your view:** do you support the goal? There is no wrong answer.
- **About you:** your GitHub username, state and U.S. congressional district. These stay with
  the Human Engineer and are never posted in GitHub.

The form never asks for your name, email, phone or address. Answer keys are never posted
in GitHub. When you pass, the Human Engineer comments "Readiness Check passed (date)" on your issue.

## Step 6 — Set up your AI assistant (recommended, not required)

AI assistants follow the same rule you do: they may draft and review, never approve
(SPEC-003 §18.3(3)). To set up Claude the way the Human Engineer's is set up:

1. In Claude, create a Project named `PRJ-002 One-Hour Rule — <your name>`.
2. **Instructions:** paste the **Contributor** block from
   [`prompts/PRJ-002-Claude-Project-Instructions.md`](prompts/PRJ-002-Claude-Project-Instructions.md).
   Paste only the text inside the block.
3. **Context:** add two GitHub sources:
   - `RuntimeRepublic/Legislative-Manager`: `CLAUDE.md`, `ONBOARDING.md`, `CALENDAR.md`,
     `prompts/LegislativeManager.md`, `projects/PRJ-002-Kansas-Legislative-Text-Posting/`, `kansas-standards/`
   - `RuntimeRepublic/Runtime-Republic-Training`: `Courses/one-hour-rule/`, `Courses/reading-the-draft/`
4. **First message:** "Read ONBOARDING.md and my onboarding issue (#__). Where am I, and what is my next step?"

Cursor or another editor is useful at Level 3, when you edit files. It is not required before then.

## Step 7 — Level 1 (Reviewer)

When Steps 4 and 5 are complete, the Human Engineer adds the `level-1` label, records the grant
(name, level, date; SPEC-003 §18.3(4)) and shares the model language document for review.

---

## Moving up

| Level | You may | How you get there |
|---|---|---|
| 1. Reviewer | Comment on the model language document | Steps 1–7 |
| 2. Contributor | Open Review Comment and Proposed Change issues here | Useful, sourced review comments at Level 1; ZIP code and districts sent privately (precinct and party optional) |
| 3. Proposer | Open pull requests | Useful issues at Level 2 |

At every level you propose and the Human Engineer decides. See [CONTRIBUTING.md](CONTRIBUTING.md)
for the ground rules and [CALENDAR.md](CALENDAR.md) for dates.

## If you hold public office

Before Level 1 you will be told that your comments about official business may be public
records under the Kansas Open Records Act, and that discussion among members of your public
body belongs in a noticed meeting, not here (Kansas Open Meetings Act; SPEC-003 §18.3(1)).
