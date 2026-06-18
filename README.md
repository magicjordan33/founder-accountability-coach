# founder-accountability-coach

> an AI-powered morning brief that tells you the single most important thing to do today — built from your actual data, not templates.

---

## what this is

every morning, before you do anything else, an AI reads your dayNumber_ logs, your inbox, and your calendar — then tells you exactly what to do today to hit your goal.

not a to-do list. not a generic productivity prompt. a brief built from your actual situation: what conversations are open, what follow-ups are due, what your consistency signal looks like, how many days you have left to hit your target.

it takes 60 seconds to read. it tells you the one thing that moves the needle most today.

this repo contains the prompt template, setup instructions, and the MORNING_BRIEF.md file you need to run this inside a Claude project.

---

## what it looks like

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

this is a real brief. pulled from live data. zero fabrication.

---

## how it works

the brief pulls from three sources simultaneously:

**dayNumber_** — your proof-of-work layer. every day you log publicly, your day # goes up. the AI reads your streak, your consistency signal, your total logs, and how many other founders are active on the platform. the more you log, the more context the AI has about what you're actually building. longer log history = smarter brief.

**Gmail** — your inbox. the AI scans for unread replies from anyone in your target audience overnight. VC replies, founder responses, accelerator confirmations. it surfaces what needs a response before anything else.

**Google Calendar** — your follow-up queue. every reminder, call, and follow-up due today shows up in the brief. nothing falls through.

the AI then synthesizes these three streams into one output: the single most important thing to do today, followed by a prioritized focus list for the rest of the day.

---

## setup

### step 1 — create a claude project

go to [claude.ai](https://claude.ai) and create a new Project. projects give Claude persistent instructions and memory across conversations.

### step 2 — connect your tools

in the project settings, connect the following MCP integrations:

- **dayNumber_** — connect at [daynumber.io/connect](https://daynumber.io/connect). this is the core data layer. your daily logs are what make the brief specific to you.
- **Gmail** — connect via the Google MCP integration in Claude settings
- **Google Calendar** — connect via the Google MCP integration in Claude settings

the brief works without Gmail and Calendar but it will be less specific. dayNumber_ is the minimum required connection.

### step 3 — add the morning brief instructions

copy the contents of [`MORNING_BRIEF.md`](./MORNING_BRIEF.md) from this repo into your Claude project's **Project Instructions** (the system prompt for the project).

customize the following fields for your situation:

```
## your goal
[what you are working toward and in what timeframe — e.g. "close $500K pre-seed by September 1"]

## the metric that matters most
[the single number that tells you if you're on track — e.g. "10 paying customers"]

## the warmest open thread
[the single most important relationship or conversation you are trying to close right now]

## the call pipeline
[any calls or meetings booked this week]
```

### step 4 — start every session with anything

the brief triggers automatically at the start of every new conversation in the project. you don't have to ask for it. just open Claude and say good morning. the brief runs before anything else.

---

## the brief gets smarter the more you log

the dayNumber_ connection is what separates this from any other productivity prompt.

when you log once a week, the AI knows roughly what you're working on.

when you log every day for 90 days, the AI knows your patterns — what you keep saying you'll do but don't, where your momentum actually lives, what you're avoiding. the brief stops being a summary of external data and starts being a mirror of how you actually build.

the AI has read a founder's 300 days of honest logs and told them: *"you're not inconsistent about building. you're inconsistent about talking to customers. that's the difference between a tool no one uses and something that matters."*

that kind of insight only exists after 300 days of honest logs. start logging now.

---

## customizing for your goal

the template ships configured for a founder raising a fund with a 90-day target. it works equally well for:

- **pre-seed fundraising** — track warm investor threads, follow-up cadence, and call pipeline
- **first 10 customers** — track outreach, demo bookings, and conversion pipeline
- **product launch** — track build milestones, beta user count, and launch checklist
- **30-day sprint** — set a specific 30-day goal and track daily progress against it

change the goal section in `MORNING_BRIEF.md` to match your situation. everything else adapts automatically.

---

## files in this repo

```
MORNING_BRIEF.md        — the full prompt template. paste this into your Claude project instructions.
EXAMPLE_BRIEF.md        — a real example brief with annotations explaining each section.
CUSTOMIZATION_GUIDE.md  — how to adapt the template for different founder goals.
```

---

## built on dayNumber_

this tool is built on top of [dayNumber_](https://daynumber.io) — the proof-of-work layer for founders. every day you log publicly on dayNumber_, your day # goes up. the record is permanent, public, and machine-readable.

the morning brief is what happens when your proof-of-work record meets your live inbox and calendar. the combination gives the AI enough context to tell you something true and specific about today — not something generic about productivity.

**what's your day #?**

[daynumber.io](https://daynumber.io)

---

## contributing

this is an open template. if you adapt it for a specific use case — a 30-day sprint, a sales pipeline, a product launch countdown — open a PR with your version and a description of what you changed and why.

---

*built by [jordan ovejas](https://daynumber.io/jordan) — day #326*
