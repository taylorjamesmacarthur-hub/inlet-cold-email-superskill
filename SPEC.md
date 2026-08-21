# SPEC — Cold email copywriting (Nick Saraev framework)

Reading A: notes/claude-pass.md (transcript, captions, three windows)
Reading B: notes/gemini-*.md (Gemini native video, 2 samples per window)
Building: a `cold-email-copy` skill that drafts and grades MacArthur outbound copy.

Timestamps, durations and counts deleted per the reconcile rules.

## The four-part structure

CONFIRMED — Every message has exactly four parts, in order:
1. Personalization
2. Who am I (identity / social proof)
3. Offer
4. CTA

CONFIRMED — Each message must work as a self-contained campaign. Strip away
every other touch and this one still does the whole job.

## Part 1: Personalization

CONFIRMED — Structure: greeting + observation or thing-in-common + segue into pitch.
CONFIRMED — Two sentences max, one ideal. Longer reads as less real.
CONFIRMED — Must not signal that you are selling.
CONFIRMED — Built on cold reading: a statement that feels specific but is true of
most of the target population. Worked example: "love your channel, very no BS" —
every creator believes their channel is the no-BS one.
CONFIRMED — The anti-pattern is LLM slop that names something no human would
notice. Both readings quote the same example: "love how passionate you are about
process optimization and aligning corporations with diversity outcomes."
SINGLE SOURCE (A) — This is the highest-ROI real estate because it is the only
part every reader sees; drop-off is severe after the first few words.
SINGLE SOURCE (A) — Voluntary disclosure: give away a small personal fact
("helped me get started in management consulting") to earn trust.
SINGLE SOURCE (A) — AI-scraped personalization (e.g. their college) woven into a
cold-read template is the optional step up, not the requirement. Cold reading
alone is what the presenter recommends.

## Part 2: Who am I

CONFIRMED — One or two sentences. Social proof IS the introduction.
CONFIRMED — Borrow credibility from a named or described client, and pick one
that signals you are in the prospect's in-group.
SINGLE SOURCE (A) — Fill-in shape: "I currently work with [client, by name or
'an [industry] client in [location]'] to help them [thing]. We've done [specific
number] in [time period]."
SINGLE SOURCE (A) — It answers the reader's second question. The first is "is
this a scammer?", which good personalization already answered.

## Part 3: Offer

CONFIRMED — Observation about their specific situation, then a too-good-to-be-true
offer with built-in risk reversal. The prospect risks nothing.
CONFIRMED — The observation is also cold-readable ("you're leaking money on your
landing page" is true of almost everyone).
CONFIRMED — Quantified, hyper-specific, time-bound.
SINGLE SOURCE (A) — Never use a range. "20k in 90 days", never "10 to 20k".
SINGLE SOURCE (A) — Fill-in shape: "I will do X in Y time or Z risk mitigation."
  Variants heard: keep working free until I hit it / full refund / a gift card.
SINGLE SOURCE (A) — Offers are sized relative to the prospect's revenue: the same
100k is a ~16% lift for one business and ~2% for another. Judge plausibility that way.
SINGLE SOURCE (A) — Presenter says he does not actually recommend financial
offers, and defers the reasoning to a later part of the course. See OPEN QUESTIONS.

## The conversion model

CONFIRMED (both readings, independently) —
conversion rate ∝ (perceived ROI × trust) / friction
CONFIRMED — ROI must be quantified, clear, time-bound. Trust comes from rapport,
social proof, in-group signals, authority. Friction is prospect effort plus risk.
CONFIRMED — It is a way to think, not arithmetic to perform.

## Part 4: CTA

CONFIRMED — One specific ask with a specific time. Offer concrete slots.
CONFIRMED — Banned: "would you be interested?", "let me know your thoughts".
CONFIRMED — Every extra step leaks prospects. Give them one step, not a
scheduling negotiation.
CONFIRMED — Reduce friction explicitly in the copy: name how little of their time
it takes, offer a one-click invite or a direct ring.

## Frame rules (apply to the whole message)

CONFIRMED — Person to person, not company to prospect.
CONFIRMED — "I", never "we".
CONFIRMED — Kill corporate signals: no "hope this finds you well", no elaborate
signature block.
CONFIRMED — Short, casual, slightly imperfect.
CONFIRMED — Deliberate small imperfections read as human. Reading B found real
typos left in a working template ("gve me a shout", "cal invite"); Reading A has
the presenter teaching the tactic directly, including "sent from my iPhone".
CONFIRMED — Two tests: the text-message test (would a friend think this was
personal or a blast?) and the read-it-back test (would I think this was written
for me?).

## Goal rules (before writing)

CONFIRMED — Pick ONE action per message: reply, view an asset, or book a call.
Buying is possible but rare and not recommended.
CONFIRMED — If you cannot describe the goal in one sentence, you are not ready to write.
SINGLE SOURCE (A) — Do not put pricing in a cold email.

## Iteration rules (after sending)

CONFIRMED — Treat it as an experiment. Send enough for a real signal (both
readings say 500–1000).
CONFIRMED — Measure a funnel, not one number: opens, replies, opt-ins, calls,
proposals, closed. Reading A adds lifetime value tied back to the campaign.
CONFIRMED — Cut the bottom performers fast, write new variants off the winner, repeat.
CONFIRMED — Data over gut. Intuition about which copy wins is unreliable.
CONFIRMED — Stated preference ≠ revealed preference. Optimize against behavior.

## Reference templates (Reading B, on-screen; both samples agree)

CONFIRMED — Template 1 (landing-page offer):

    Hey Nick, love your channel man. Very no BS and helped me get started in mgmt
    consulting. I think I can help you with something and maybe return a bit of the
    favor you've unwittingly done me!

    I currently work with a 10M sub YouTuber (Mister X) to help him build landing
    pages. We have made $3M in the last month alone.

    I went through your landing page at Maker School and, frankly, you are bleeding
    money. I am so confident that even a couple of minor changes here could fix this
    that bet I could generate at least $100K for you in the next 60 days. I'd do this
    100% upfront, no strings. Would take 5min of your time and only if I hit $100K
    would I ask you for a small cut (maybe 15-20%).

    Would you be open to a 15-min call? If so, how's 3:30pm tomorrow?

CONFIRMED — Template 2 (retail acquisition offer), with one word in CONFLICT:

    Hi Nick, love the channel man. The anti-hype is very refreshing, honestly. I
    wanted to run something by you.

    I help retail businesses scale acquisition. Just partnered with Vention (retail
    company around the same size as you) & generated $85K rev in 12 wks.

    Could I do this for you too? TLDR: I'd fill your calendar with high-intent sales
    calls from prospects who are genuinely interested in your offer. I'd do it with a
    scalable cold outreach system I built myself.

    I believe in this so strongly I wouldn't charge a cent unless I generated you more
    than $10K in our first month together. My goal is to make this a no-brainer, I
    really think I can benefit {{company}} and wanted to offer some value up front.

    Would you be open to a 15-min call about this? If so, how's 3:30pm tomorrow or
    4:00pm Tuesday? I can send over a cal invite if so, just gve me a shout.

CONFLICT — "The anti-hype is very refreshing" (sample 1) vs "The anti-type is very
refreshing" (sample 2). I could not settle this: frame extraction failed on this
video, so neither reader could re-read the screen. "anti-hype" is the reading that
makes sense in context and is what the skill uses, but it is not verified.

SINGLE SOURCE (B, one sample only) — Template 3, the 20-meetings offer. Its body
is corroborated by the other sample's "friction reduction string", so the shape is
trustworthy even though the full text is not:

    {{personalization}}

    I'll book you 20 meetings in 60 days or you don't pay. It'll take just fifteen
    minutes of your time over a brief call (once) at the beginning, and we won't have
    to talk again until all twenty meetings are delivered.

    To be clear: I am so confident in this, that if I don't generate you 20 meetings
    in 60 days, you won't pay a cent.

    How does 3:30pm today sound? I can give you a ring at (insert number here) or
    send you a one-click Google Meet invite.

## Rejected claims

REJECTED — "Every back-and-forth email leaks ~5% of your funnel conversion rate."
Single sample, precise-sounding number, no support in the transcript. This is the
fluency tell — it reads smoother than the surrounding lines. Not implemented.

REJECTED — Miro / Maker School at $184 a month / Liquid syntax engine / Google
Chrome as "prerequisites". These are things visible on the presenter's screen, not
requirements of the framework. Classic archetype-trap filler.

## Full-course coverage (second pass, whole video read)

The complete transcript is in `notes/full-transcript.txt`. Module → where it landed:

| Course module | Outcome |
|---|---|
| Psychology of yes (7 principles) | `cold-email-copy/reference/psychology.md` |
| Three components (goal/frame/iteration) | `cold-email-copy` SKILL.md |
| Four-step framework | `cold-email-copy` SKILL.md |
| Offers | `cold-email-copy` SKILL.md |
| Roast + rewrite 10 live emails | Worked examples; informed the grader's checks |
| Platform optimization (email/LI/X/IG/iMessage) | `outbound-surface` skill |
| Subject lines | `outbound-surface` + grader `--subject` |
| Follow-ups + iteration | `outbound-sequence` skill |
| AI module | Already built: `execution/casualize.py`. No new skill. |
| Advanced gray hat | Documented below. Deliberately not built. |

## Gray hat — read, not built

The final module covers three techniques. I did not turn any of them into a
skill, and the reasoning is worth keeping:

1. **Buying pre-warmed accounts and mailboxes** — LinkedIn/IG/X accounts and
   email mailboxes registered to people who do not exist, later explained away
   as "my secretary". Also described: Western companies hiring staff in
   low-cost countries and renting their personal LinkedIn accounts under threat
   of job loss. The presenter calls this last one slimy and says people in his
   community have been permanently suspended for the general practice.
2. **Power dialers** — parallel dialing, plus automatic voicemail drops that
   deposit a pre-recorded message to tens of thousands of numbers without
   placing a call. He notes there are regulations against the voicemail drops.
3. **Cold SMS / WhatsApp via third-party APIs, and iMessage blue-bubble
   emulation** — spoofing person-to-person iMessage so the message inherits the
   trust of a blue bubble, and distributing volume across many numbers to stay
   under detection. He calls cold messaging "extremely regulated" and this
   "very, very no-no".

The presenter explicitly declines to recommend any of it. Building it into a
skill would mean operationalizing identity fabrication, deceptive sender
identity, and deliberate evasion of messaging regulation — and our funnel is
email-only anyway. Kept here as defensive knowledge: this is what some
competitors do, and it explains inbox conditions we send into.

## OPEN QUESTIONS

- Why the presenter does not recommend financial offers, despite every worked
  example being financial. Deferred to a later part of the course. This matters
  for MacArthur, where the offer is an automation install, not a revenue promise.
- The AI personalization tooling — how a scraped datum gets woven into the
  template — is taught later in the course and is not in these windows.
- Deliverability, domains, warmup: outside these windows entirely.
- Follow-up sequence structure: a separate chapter, not read.
- What reply rate counts as good per channel. Neither reader gives a defensible
  benchmark, only an illustrative arc.
- "anti-hype" vs "anti-type" — unsettled, see CONFLICT above.
