# LOG_MY_DAY.md

## The four-word trigger

The only thing dayNumber_ requires is that you log, honestly, every day. Most founders miss a day not because nothing happened, but because logging meant stopping, opening another app, and starting from a blank field.

If you're already talking to Claude, the log should come from that conversation. Four words, end of day:

**"log my day number"**

Any close variant works too — "log my day," "post this to dayNumber_," "help me log today," "day number log." This file tells Claude what to do when it hears any of them.

---

## What Claude does

### 1. Gather what actually happened

Pull first from this conversation's own context — what got built, what broke, what got decided, what got dropped today. If there isn't enough here to work with, ask one sharp question, not a form: "what actually happened today?" If the answer is vague or future tense ("going to," "planning to"), push once: "what's one specific thing you did, not planned?" A plan is not a log entry.

### 2. Draft it in your voice, not a recap voice

- Never open with the day number — the platform stamps it automatically. Restating it reads wrong.
- Never close with a sign-off or a motivational tag. Not "showing up," not "one day at a time." The entry ends when the thought ends.
- First person, plain, specific, honest about what didn't work, not just the wins.
- No buzzwords, nothing that reads like a LinkedIn post.

### 3. Show the draft. Always.

Claude shows the full draft and lets you edit it freely before anything posts — even if you said "just post it for me." This step is not optional. It's what makes the record honest: an AI-assisted draft is fine, an AI-published log you never read is not.

### 4. Post it

Claude calls `post_log` with your confirmed text and your actual timezone (asks if genuinely unknown — a wrong timezone can push a log across a day boundary and misalign the day #).

### 5. Close the loop

One or two lines back, using `get_morning_brief` or `read_logs`: "logged. day #[X], streak's at [N]." The same small hit of watching the number move, without opening the app.

---

## What this never does

- Never invents details you didn't say or confirm.
- Never posts without you seeing and confirming the final text first.
- Never turns a plan or intention into past-tense log language.
- Never adds hype, a sign-off, or a closing line you didn't write yourself.
- Never silently guesses your timezone when it would change which day the log lands on.

This is the same rule that governs everything else on dayNumber_: the record is only worth anything if nothing on it was invented.
