# founder-accountability-coach

> the only four words you need to say to your AI at the end of the day: "log my day number." everything else here — the morning brief, the coaching, the pattern-reading — builds from that one honest habit.

---

## what this is

two things, one record.

**every night**, you say four words to Claude — "log my day number" — and it gathers what actually happened today (from your conversation, or by asking one sharp question if it needs more), drafts an honest log in your voice, shows it to you, and posts it to dayNumber_ once you confirm. no blank field, no second app.

**every morning**, before you do anything else, Claude reads that record — plus your inbox and calendar if you connect them — and tells you the single most important thing to do today. not a to-do list. a brief built from what's actually alive.

between the two, you get a coach: something that's read your actual logs, tracks your patterns, and asks the question you've been avoiding instead of the one that's easy to answer.

this repo contains everything you need to run all three inside a Claude project.

---

## what it looks like

saying the four words, 11pm:

```
you: log my day number

claude: here's the draft —

"spent most of today debugging the payment webhook, no luck. did get
a reply from the accelerator, call's booked for thursday. also just
tired today, wanted to quit around 4pm, didn't."

want to add or change anything before I post it?

you: post it

claude: logged. day #327, streak's at 40.
```

the next morning:

```
day #326 — june 18, 2026
streak: 39 days — green
logged today: yes

the number that matters most right now: 1 daily logger
target: 50 — 49 to go — not moving.

what's alive from yesterday
— Jordan Baker, Athenaeum VC — call confirmed Tuesday June 23, 8:30am PST
— Shannon Graszat, Innovation Factory — sprint conversation open, no confirmation yet
— Michael Cardamone, Forum Ventures — email delivery failing, 20 hours left before bounce

overnight replies
inbox is clear.

calls and reminders today
— follow-up due: Jyoti Bansal, Unusual Ventures (sent June 11, 7 days)
— follow-up due: Nakul Mandan, Audacious Ventures (sent June 11, 7 days)

the single most important thing today
fix the Michael Cardamone email before the delivery fails permanently.

one reminder from the canon
Ford: the assembly line only works if every station is moving.
1 daily logger means the line has stopped. get the sprint partner confirmed today.

| target                      | current | needed | days left |
|-----------------------------|---------|--------|-----------|
| daily loggers for $10M close| 1       | 50     | 87        |
| sprint partner confirmed    | 0       | 1      | —         |
```

both pulled from live data. zero fabrication, either direction.

---

## how it works

three layers, one record:

**the log** — four words, end of day. Claude drafts from your actual conversation, you confirm, it posts to dayNumber_. this is the one non-negotiable habit everything else depends on.

**dayNumber_** — your proof-of-work layer. every day you log publicly, your day # goes up. the AI reads your streak, your consistency signal, your total logs, and how many other founders are active on the platform. longer log history = smarter brief, smarter coaching.

**Gmail + Google Calendar** — optional. sharpens the morning brief with overnight replies and today's calls and follow-ups. the brief and the log both work without these; dayNumber_ is the one required connection.

**the coach** — reads your logs, tracks your patterns, and pushes back. not a mentor, not a hype machine. the thing that asks the question you've been avoiding.

---

## setup

### step 1 — create a claude project

go to [claude.ai](https://claude.ai) and create a new Project. projects give Claude persistent instructions and memory across conversations.

### step 2 — connect your tools

in the project settings, connect:

- **dayNumber_** — connect at [daynumber.io/connect](https://daynumber.io/connect). required. this is what makes the log real and the brief specific to you.
- **Gmail** and **Google Calendar** — optional, connect via the Google MCP integration in Claude settings, for a sharper morning brief.

### step 3 — add the project instructions

paste the full contents of both [`LOG_MY_DAY.md`](./LOG_MY_DAY.md) and [`MORNING_BRIEF.md`](./MORNING_BRIEF.md) into your project's **Project Instructions**. these define what Claude does automatically, every session: the four-word logging trigger and the morning brief.

### step 4 — add the coach

upload [`coach.md`](./coach.md), [`identity.md`](./identity.md), [`rules.md`](./rules.md), [`examples.md`](./examples.md), [`mcp.md`](./mcp.md), and the [`reference/`](./reference) folder to your project's **Project Knowledge**. this is what turns "logs your day and briefs you" into "coaches you" — the Three Windows, the consistency signals, the quit signal, the weekly review.

### step 5 — customize your goal

edit the `## your goal` block at the top of `MORNING_BRIEF.md`:

```
FOUNDER NAME: [your name]
CURRENT GOAL: [what you're working toward — e.g. "close $500K pre-seed by September 1"]
GOAL DEADLINE: [date]
THE METRIC THAT MATTERS MOST: [the single number that tells you if you're on track]
CURRENT COUNT: [where you are right now]
TARGET COUNT: [where you need to be]
DAYS REMAINING: [calculate from today to deadline]
WARMEST OPEN THREAD: [the one relationship or conversation you're trying to close]
CALL PIPELINE: [calls or meetings booked this week]
```

everything else adapts automatically.

---

## the record gets smarter the more you log

when you log once a week, the AI knows roughly what you're working on.

when you log every day for 90 days, it knows your patterns — what you keep saying you'll do but don't, where your momentum actually lives, what you're avoiding. the brief and the coaching stop being a summary of external data and start being a mirror of how you actually build.

start with the four words tonight. everything else compounds from there.

---

## files in this repo

```
LOG_MY_DAY.md                      — the four-word logging trigger. paste into Project Instructions.
MORNING_BRIEF.md                   — the morning brief trigger. paste into Project Instructions.
coach.md                           — the full coaching system prompt. upload as Project Knowledge.
identity.md                        — who the coach is. upload as Project Knowledge.
rules.md                           — the ten coaching rules. upload as Project Knowledge.
examples.md                        — coaching vs. knowledge-base responses, side by side. upload as Project Knowledge.
mcp.md                             — how to connect the dayNumber_ MCP server.
reference/day-number-framework.md  — the day # system explained.
reference/coaching-drills.md       — specific techniques for common founder moments.
```

---

## built on dayNumber_

this tool is built on top of [dayNumber_](https://daynumber.io) — the proof-of-work layer for founders. every day you log publicly on dayNumber_, your day # goes up. the record is permanent, public, and machine-readable.

**what's your day #?**

[daynumber.io](https://daynumber.io)

---

## contributing

this is an open template. if you adapt it for a specific use case — a 30-day sprint, a sales pipeline, a product launch countdown — open a PR with your version and a description of what you changed and why.

---

*built by [jordan ovejas](https://daynumber.io) — see the current day # on [my public profile](https://daynumber.io/jordan)*
