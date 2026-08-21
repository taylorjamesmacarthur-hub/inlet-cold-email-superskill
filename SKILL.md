---
name: inlet-cold-email-superskill
description: Meta-skill for cold email. Interviews you for industry, role, and business type, writes the four-part outbound email (personalization, who am I, offer, CTA), runs a persuasion pass and a humanizer pass so it does not read like AI, then grades it. Use when asked to write a cold email, draft outreach, personalize a sequence, fix a cold email that is not getting replies, grade or critique outbound copy, or build a new template for the cold rotation.
argument-hint: "<what you're selling and to whom> | <path to an email to grade>"
allowed-tools: Bash, Read, Write, Edit, Grep, AskUserQuestion
user-invocable: true
---

# inlet-cold-email-superskill

<img src="assets/macarthur-mark.jpg" width="80" align="right" alt="MacArthur Media">

*Built by MacArthur Media for Inlet Recruiting.*

**The writing framework is Nick Saraev's four-part cold email formula.** Do not
substitute another structure, another order, or another CTA style. The formula,
its confirmed rules, and its reference templates are recorded in
[`SPEC.md`](SPEC.md) with confidence labels — CONFIRMED lines are verified by two
independent readings of the source course, SINGLE SOURCE lines are not. When a
draft and this skill disagree, `SPEC.md` wins.

One skill, four moves, in order. Do not skip a move.

    0. Intake      — industry, role, business type. Never guess these.
    1. Draft       — the four-part frame (below).
    2. Persuade    — conversion pass (reference/copywriting).
    3. Humanize    — AI-tell pass (reference/humanizer).
    4. Grade       — saraev_grade.py + copy_lint.py, or the manual checklist.

**New here, or explaining this to someone who isn't technical?** Read
[DIAGRAMS.md](DIAGRAMS.md) — six diagrams, recruiting examples, no jargon.

Before writing, answer in one sentence: what is the ONE thing they should do
after reading? Reply, view an asset, or book a call. If you cannot say it in one
sentence, you are not ready to write.

---

## Step 0 — Intake (mandatory)

**Never write a cold email without knowing industry, role, and business type.**
Personalization that is not anchored to those three is the AI slop this whole
framework exists to prevent.

If any of the three is missing from the request, ask with `AskUserQuestion` —
one question per missing field, options drawn from what you already know about
the request, and always leave room for "Other".

| Field | What you need | Why it changes the copy |
|---|---|---|
| **Industry** | gym / agency / SaaS / clinic / trades / e-comm… | Sets the vocabulary and the cold-read that lands |
| **Role** | owner / VP / ops manager / marketing lead… | Sets what they are measured on, which becomes the offer |
| **Business type** | single location, multi-location, franchise, solo, PE-backed | Sets the scale of the claim so it stays credible |

Also confirm, if not already given: what you sell, your proof (a named client or
a number), and the one action you want.

### Role → what they are measured on

Write the offer against the metric the role owns, not the one the company owns.

| Role | Owns | Offer against |
|---|---|---|
| Founder / owner | Revenue, survival | New booked calls, hours back |
| VP / director | The number their boss watches | Throughput, retention, cost per outcome |
| Ops / GM | Process, staffing, chaos | Hours back, fewer escalations |
| Marketing lead | Pipeline, CAC | Qualified replies, show rate |
| Office / clinic manager | Schedule density, no-shows | Filled slots, fewer no-shows |

### Business type → claim ceiling

- **Solo / single location** — small absolute numbers, high relative lift. "8 more consults a month."
- **Multi-location** — per-location numbers, then multiply. Never quote a total that sounds fake.
- **Franchise** — they cannot change brand assets. Offer must live inside their constraints.
- **PE-backed / enterprise** — they buy repeatability, not heroics. Lead with process and proof.

---

## Step 1 — Draft: the four parts

Each message must stand alone — strip away every other touch and this one still
does the whole job.

### Part 1 — Personalization

Greeting, then an observation or thing-in-common, then a segue into the pitch.

- Two sentences max. One is ideal.
- Must not signal that you are selling. No money, no pitch language.
- Use cold reading: something that feels specific but is true of most of the
  target list. "Love your channel, very no BS" works because every creator
  believes theirs is the no-BS one.
- Anchor the cold read to the **industry** from Step 0. A gym owner and a SaaS
  VP do not believe the same flattering thing about themselves.
- Give away one small real fact about yourself. It buys trust cheaply.
- The failure mode is AI slop that names something no human would notice —
  "love how passionate you are about process optimization." If a real person
  would not write it, cut it.

### Part 2 — Who am I

One or two sentences. Social proof IS the introduction.

    I currently work with [client by name, or "a [industry] business in [location]"]
    to help them [thing]. We've done [specific number] in [time period].

Pick the client that puts you in the prospect's in-group — same **industry**,
same **business type** where possible. "we" is allowed here and only here — it
means you and your client.

### Part 3 — Offer

An observation about their situation, then an offer with the risk on you.

- The observation is cold-readable too: "you're leaving money on the table with
  your intake process" is true of nearly everyone.
- Quantified, specific, time-bound.
- **Never a range.** "20 meetings in 60 days", never "10 to 20".
- Risk reversal is not optional. The prospect risks nothing.

      I will [X] in [Y time] or [Z — you don't pay / I keep working free / full refund].

- Size the claim against their revenue and their **business type**. The same
  number is a 16% lift for one business and 2% for another. Only the second one
  is credible.

**MacArthur note:** quantify in outcomes, not dollars — booked calls, hours back,
replies handled. `copy_lint.py` bans dollar figures in cold copy, and a revenue
promise is one we would have to keep. Outcome guarantees pass both bars.

### Part 4 — CTA

One specific ask, with a specific time.

- Banned: "would you be interested?", "let me know your thoughts."
- Give slots, not a negotiation. Every extra step leaks prospects.
- Say how little of their time it takes, and offer the one-click path.

      Would you be open to a 15-min call? How's 3:30pm tomorrow?

### Frame rules (whole message)

- One person to one person. "I", never "we" (outside Part 2).
- No "hope this finds you well." No signature block beyond your name.
- Short, casual, slightly imperfect. A small typo or a "sent from my iPhone"
  reads more human than clean copy.

### The conversion model (Saraev, CONFIRMED)

    conversion  ∝  (perceived ROI × trust) / friction

A way to think, not arithmetic to perform. Use it to diagnose a dead draft:

- **ROI too low or too vague?** → Part 3. Quantify it, time-bound it, size it to
  their business type.
- **Trust too low?** → Part 2. Better client name, tighter in-group match, a real
  number instead of an adjective.
- **Friction too high?** → Part 4. Fewer steps, a named time, a one-click path,
  and the risk moved onto you.

Every fix lives in one of the four parts. If a change does not raise ROI, raise
trust, or cut friction, do not make it.

### Reference templates

Three verbatim Saraev templates are in [`SPEC.md`](SPEC.md) under "Reference
templates" — the landing-page offer, the retail acquisition offer, and the
20-meetings offer. Read them before writing a new template for the rotation. Copy
their *shape*, never their words; the wording is tied to that sender and that list.

---

## Step 2 — Persuasion pass

Run the draft against `reference/copywriting/SKILL.md`. In a cold email only
these five carry weight — check each, fix in place:

1. **Benefits over features** — they do not care what you do, only what changes.
2. **Specificity over vagueness** — a number, a name, or a date in every part.
3. **Customer language over company language** — write the words the *role*
   uses, not the words your deck uses.
4. **One idea per email** — if the message argues two things, cut one.
5. **Clarity over cleverness** — a clever line that costs a beat of confusion
   loses to a plain one.

Deeper frameworks (PAS, hooks, transitions) are in
`reference/copywriting/references/`. Load only if the draft is failing.

**This pass edits inside the four parts. It never restructures them.** The
copywriting skill is written for landing pages; where it conflicts with Saraev —
page-length copy, multiple CTAs, feature sections, "we" voice — Saraev wins.

---

## Step 3 — Humanizer pass (mandatory)

Cold email is where AI tells cost money. Run the draft through
`reference/humanizer/SKILL.md`, `--voice casual --purpose email`.

Non-negotiable for outbound, from that skill's pattern catalog:

- **P13 em dashes** — zero. Commas or a period.
- **P7 AI vocabulary** — no delve, leverage, robust, seamless, foster, notably,
  moreover, "in today's landscape".
- **P9 negative parallelism** — no "not just X, it's Y".
- **P10 rule of three** — no forced triads.
- **P17 curly quotes** — straight quotes only; curly quotes read as pasted.
- **P22–P30 hedging** — no "perhaps", "might be able to", "I was wondering if".
- **Burstiness** — vary sentence length hard. Four sentences of the same length
  is the loudest tell in a short email.

Preserve, do not sand off: real names, real numbers, the small self-deprecating
fact, the deliberate fragment. Those are the human signal.

Full 53-pattern catalog: `reference/humanizer/references/patterns.md`.

---

## Step 4 — Grade it

    .venv/bin/python execution/saraev_grade.py <file>                    # the four parts
    .venv/bin/python execution/saraev_grade.py --subject "nick?" <file>  # + subject line
    .venv/bin/python execution/copy_lint.py                              # length, banned words, pricing

Both must pass before anything goes in the rotation. `saraev_grade.py` expects
the four parts as blank-line separated blocks.

**Outside this workspace** (no scripts): grade manually, all six must be yes.

1. Are all four parts present, in order?
2. Is there a number, name, or date in Part 2 and Part 3?
3. Is the risk on the sender, not the prospect?
4. Is the CTA one ask with one specific time?
5. Zero em dashes, zero AI vocabulary, zero hedging?
6. **Text message test** — would a friend seeing you type this think it was
   personal, or a blast?
7. **Read it back** — if this landed in your inbox, would you think it was
   written for you?

---

## After sending

- One variable at a time, enough volume for a real signal (500–1000 sends).
- Track the whole funnel, not one number: replies, opt-ins, calls, closed.
- Cut the bottom performers fast, write new variants off the winner, repeat.
- Data over gut. Copy you expect to flop routinely wins.
- Watch what prospects do, not what they say.

## Related

- `reference/humanizer/` — bundled. 53 AI patterns, five voice profiles.
- `reference/copywriting/` — bundled. Conversion copy principles and frameworks.
- `reference/psychology.md` — the seven principles under all of this. Use it to
  diagnose *why* a draft isn't landing.
- `outbound-surface` — sender name, subject line, teaser, profile: everything
  judged before the body. If opens are bad, the problem is there, not here.
- `outbound-sequence` — how many follow-ups, and how to iterate on evidence.
- `execution/casualize.py` — turns "Pacific Creative Group LLC" into "PCG" and
  "Vancouver, British Columbia" into "East Van". This is the only job AI should
  do in your copy: small templated variables inside a template that already
  works. Never let it write the whole email — that is what produces the slop
  opener the framework exists to avoid.

## Provenance

The four-part frame, the conversion model, the frame rules, and the iteration
rules are Nick Saraev's, from "Cold Email Copywriting & Outreach Full Course
2026", extracted via the youtube-to-agent pipeline. `SPEC.md` and `notes/` carry the
confidence labels — CONFIRMED lines are verified by two independent readings,
SINGLE SOURCE lines are not. Humanizer and copywriting passes are bundled from
their standalone skills under `reference/`.
