# Onboarding — Join PRJ-002, the Kansas One-Hour Posting Rule

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
| 2 | Read the two courses | — | — |
| 3 | Open your onboarding issue | The issue (public) | — |
| 4 | Send private details to the Human Engineer | A "received" note on your issue (no details) | Human Engineer |
| 5 | Pass the lesson quizzes | A "quizzes passed" note on your issue | Human Engineer (by hand for now) |
| 6 | Pass "Explain it back" | A "Part B passed" note on your issue | Human Engineer |
| 7 | Set up your AI assistant (recommended) | A checked box on your issue | You (self-reported) |
| 8 | Receive Level 1 | A `level-1` label and a recorded grant | Human Engineer |

Then you move up to Level 2 and Level 3 by doing useful work (SPEC-003 §18.2).

---

## Step 1 — GitHub account

Create a free account at [github.com](https://github.com). That is the only account required to start.

## Step 2 — Learn the goal

Read these free courses in the Runtime-Republic Training repository:

- [*The One-Hour Rule*](https://github.com/RuntimeRepublic/Runtime-Republic-Training/tree/main/Courses/one-hour-rule), Lessons 01–05
- [*Reading the Draft*](https://github.com/RuntimeRepublic/Runtime-Republic-Training/tree/main/Courses/reading-the-draft), Lessons 01–02

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

Later, at Level 2, you will also be asked for your ZIP code and your districts. To find your
districts, enter your own address in the U.S. Census Bureau's
[Census Geocoder](https://geocoding.geo.census.gov/geocoder/geographies/address?form)
and report only your ZIP code, U.S. House district, Kansas Senate district and Kansas House
district. Never send or post your street address.

The Human Engineer will comment "Private details received" on your issue. Nothing more.

## Step 5 — Lesson quizzes (SPEC-003 §18.1, Part A)

Ask for the quiz form on your issue. You need at least 3 of 4 correct on each lesson
(*The One-Hour Rule* 01–05 and *Reading the Draft* 01–02). Answer keys are never posted
in GitHub.

For now the Human Engineer scores quizzes by hand and comments "Quizzes passed (date)" on
your issue. Signed completion codes, checked automatically, will replace this later.

## Step 6 — Explain it back (SPEC-003 §18.1, Part B)

Answer three questions in your own words and send them privately:

1. The problem PRJ-002 solves, and why a joint rule alone cannot fix it
2. The four safe-harbor conditions, and why votes stay out of the repository
3. One real weakness in the draft, and a proposed fix

Part B rewards understanding, not agreement. You may disagree with the draft and still pass.

## Step 7 — Set up your AI assistant (recommended, not required)

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

## Step 8 — Level 1 (Reviewer)

When Steps 4–6 are complete, the Human Engineer adds the `level-1` label, records the grant
(name, level, date; SPEC-003 §18.3(4)) and shares the model language document for review.

---

## Moving up

| Level | You may | How you get there |
|---|---|---|
| 1. Reviewer | Comment on the model language document | Steps 1–8 |
| 2. Contributor | Open Review Comment and Proposed Change issues here | Useful, sourced review comments at Level 1; ZIP code and districts sent privately |
| 3. Proposer | Open pull requests | Useful issues at Level 2 |

At every level you propose and the Human Engineer decides. See [CONTRIBUTING.md](CONTRIBUTING.md)
for the ground rules and [CALENDAR.md](CALENDAR.md) for dates.

## If you hold public office

Before Level 1 you will be told that your comments about official business may be public
records under the Kansas Open Records Act, and that discussion among members of your public
body belongs in a noticed meeting, not here (Kansas Open Meetings Act; SPEC-003 §18.3(1)).
