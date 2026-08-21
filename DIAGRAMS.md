<p align="center">
  <img src="assets/macarthur-media-logo.png" width="260" alt="MacArthur Media">
</p>

<p align="center"><b>Built by MacArthur Media for Inlet Recruiting</b></p>

---

# How this works — in plain English

Every example here is an Inlet Recruiting one: you place candidates, and you are
emailing the person who does the hiring.

---

## 1. The whole machine

You give it a sentence. It asks you three questions. Then it writes, edits,
de-robots, and marks its own homework before you ever see the draft.

```mermaid
flowchart TD
    A["You: 'email VPs of Talent at hospital systems'"] --> B{"Do I know the<br/>industry, role, and<br/>business type?"}
    B -- No --> C["Asks you 3 questions<br/>(healthcare / VP of Talent / multi-site)"]
    B -- Yes --> D
    C --> D["<b>Draft</b><br/>Writes the 4-part email"]
    D --> E["<b>Persuade</b><br/>Cuts anything that isn't<br/>a benefit to a VP of Talent"]
    E --> F["<b>Humanize</b><br/>Strips the 53 tells that make<br/>copy smell like ChatGPT"]
    F --> G["<b>Grade</b><br/>Scores itself. Fails = rewrite."]
    G -- Fail --> D
    G -- Pass --> H["Draft lands in your hands"]
```

**Why the loop matters:** a bad cold email doesn't get a "no", it gets silence.
The grader is the only thing standing between a weak draft and 800 sends of it.

---

## 2. Why it asks those three questions

Same product, same sender. Three different emails, because the reader is
different. This is the whole reason the intake exists.

```mermaid
flowchart LR
    subgraph IN["What you tell it"]
        I1["Industry<br/><i>healthcare staffing</i>"]
        I2["Role<br/><i>VP of Talent</i>"]
        I3["Business type<br/><i>12-hospital system</i>"]
    end

    I1 --> O1["Sets the <b>vocabulary</b><br/>'travel nurse fill rate',<br/>not 'talent solutions'"]
    I2 --> O2["Sets the <b>promise</b><br/>VP is measured on time-to-fill,<br/>so promise time-to-fill"]
    I3 --> O3["Sets the <b>size</b> of the promise<br/>'6 RN reqs per site'<br/>not 'hundreds of hires'"]

    O1 --> R["One email that sounds like<br/>it was written by someone<br/>who works in their world"]
    O2 --> R
    O3 --> R
```

**The trap it avoids:** without this, AI writes "I love your passion for talent
acquisition." No VP of Talent has ever loved receiving that sentence.

---

## 3. Same job, three readers

Who you're writing to changes what you promise. The skill picks the row for you.

```mermaid
flowchart TD
    Q["Who is reading this?"]
    Q --> A["<b>Agency owner</b><br/>worries about: revenue"]
    Q --> B["<b>VP of Talent</b><br/>worries about: the number<br/>their CEO asks about"]
    Q --> C["<b>Recruiting coordinator</b><br/>worries about: chaos"]

    A --> A2["Promise: <i>10 new client calls<br/>in 60 days, or you don't pay</i>"]
    B --> B2["Promise: <i>time-to-fill under 21 days<br/>on your hardest reqs</i>"]
    C --> C2["Promise: <i>8 hours a week back<br/>from screening</i>"]
```

---

## 4. What the four parts actually do

A cold email is four jobs in about 90 words. Each part has one job and hands off
to the next.

```mermaid
flowchart LR
    P1["<b>1. Hook</b><br/>'Saw you're hiring 14 RNs<br/>across three sites.'"] --> P2["<b>2. Proof</b><br/>'I fill nursing reqs for<br/>a 9-hospital system in Ohio.'"]
    P2 --> P3["<b>3. Offer</b><br/>'I'll fill 6 of them in 45 days<br/>or you pay nothing.'"]
    P3 --> P4["<b>4. Ask</b><br/>'15 minutes Thursday at 3:30?'"]

    P1 -.->|"buys 3 seconds"| N1["Proves you're a human<br/>who looked"]
    P2 -.->|"buys 5 seconds"| N2["Proves you've done it<br/>for someone like them"]
    P3 -.->|"buys the reply"| N3["Puts the risk on you,<br/>not on them"]
    P4 -.->|"gets the calendar"| N4["One decision,<br/>not a negotiation"]
```

**Rule of thumb:** if you deleted every other email in the sequence, this one
should still do the whole job on its own.

---

## 5. The de-robot pass

This is the step most people skip, and it's the one recruiters notice fastest —
they read hundreds of these a week.

```mermaid
flowchart TD
    D["Draft"] --> S{"Scan for 53<br/>AI fingerprints"}
    S --> X1["Em dashes"]
    S --> X2["'leverage', 'seamless',<br/>'robust', 'delve'"]
    S --> X3["'Not just X — it's Y'"]
    S --> X4["Every sentence<br/>the same length"]
    S --> X5["'I was wondering if<br/>you might possibly...'"]

    X1 & X2 & X3 & X4 & X5 --> F["Rewrite in a casual,<br/>one-person-to-one-person voice"]
    F --> K["<b>Keeps:</b> real names, real numbers,<br/>the short awkward sentence,<br/>the fact you're a human"]
```

**Before:** "I wanted to reach out as I noticed your organization leverages a
robust talent pipeline — not just for volume, but for quality."

**After:** "Saw you're hiring 14 RNs across three sites. That's a lot of screening."

---

## 6. What happens after you send

The skill's job ends at the draft. This is what makes the next draft better.

```mermaid
flowchart LR
    A["Send 500–1000<br/>of one version"] --> B["Change <b>one</b> thing<br/>(subject, or offer,<br/>or CTA — never two)"]
    B --> C["Track the whole funnel:<br/>replies → calls → placements"]
    C --> D{"Did it beat<br/>the old one?"}
    D -- Yes --> E["New champion.<br/>Write variants off it."]
    D -- No --> F["Kill it. Keep the old one."]
    E --> B
    F --> B
```

**Why volume:** at 50 sends, a 2-reply difference is luck. At 800, it's a fact.

---

<p align="center">
  <img src="assets/macarthur-mark.jpg" width="90" alt="MacArthur Media">
</p>
<p align="center"><sub>MacArthur Media · built for Inlet Recruiting</sub></p>
