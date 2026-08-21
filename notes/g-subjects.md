
===== SAMPLE 1/1  (gemini-3.6-flash, 137849+1632+879 tok) =====
### 1. WHAT IS BEING BUILT
An outbound campaign optimization specification for Cold Email, LinkedIn, X, Instagram, and iMessage. It outlines asset metadata requirements, character constraints for message teasers, copywriting formulas for subject lines ("plausible deniability"), short follow-up sequence architecture, and statistical rules for A/B testing and campaign iteration.

---

### 2. STACK AND PREREQUISITES
* **Platforms & Accounts:** LinkedIn (with optional Premium badge), X (Twitter), Instagram, Apple iMessage / SMS, Gmail / Google Workspace.
* **Tools & Apps:** Google Docs, Excalidraw, Claude Code / VS Code CLI (shown briefly for character counting).

---

### 3. COMMANDS AND CONFIG, VERBATIM

#### Document Metadata Specs (Google Docs)
```text
Instagram
1. The profile picture
2. Handle/full name
3. Teaser (30 chars)
4. Body

iMessage
1. The profile picture
2. The teaser (~90 chars or so)
3. Body
```

#### Copywriting & Iteration Rules (Excalidraw)
```text
Subjects = plausible deniability
SLs don't sell
```

**Bad Subjects:**
```text
Quick idea on your daily strategy content
Quick Collab?
Can you double this week?
Interested in ai driven performance optimization
Video Editor
Nick - you scaled to $72K/mo with automation. Here's the next level.
(no subject)
```

**Good Subjects:**
```text
your claude code course and a formatting thought
2026 capital
Been w you from the START
Nick's blind spot.
nick, r u taking coaching clients?
nick, q
nick, are u hiring?
nick, you looked sad in your last vid
nick you're wasting $2,300 per month!
```

**Follow-up Template:**
```text
Hey {X}, checking in on {Y}. TLDR if this is the first time you're seeing this: {email body}. Thanks, Nick
```

**Rules for Iterating:**
```text
1. Always iterate. Always have multiple variants going simultaneously.
2. Stick to a schedule. If you don't, you'll forget.
3. Good rule is 500-1000 per variant.
4. Pick a TAM with a lot of leads (digital agencies in United States).
```

---

### 4. THE BUILD ORDER
1. **Document Messaging Assets:** Define visible metadata for Instagram (~30 char teaser) and iMessage (~90 char teaser).
2. **Define Subject Line Copywriting:** Categorize bad vs. good subject lines based on whether they try to sell versus generating click curiosity via plausible deniability.
3. **Structure Follow-up Architecture:** Map out an initial 2-step sequence (Email 1 -> Email 2) utilizing brief, human pings rather than sales pitches.
4. **Establish Iteration Framework:** Define A/B testing parameters (500–1000 sends per variant, weekly iteration schedule, high-volume TAM target).

---

### 5. GOTCHAS
* **Selling in Subject Lines:** Subject lines that explain the offer reduce open rates. The subject line's only role is to buy the click.
* **Spam Pattern Triggers:** Words like "Quick", capitalized acronyms like "AI", or missing subject lines immediately signal sales bots.
* **Over-sequencing Unproven Copy:** Launching 4+ email sequences on untested copy drastically increases block/spam risks across sending infrastructure.
* **Low Sample Size Testing:** Making campaign decisions on fewer than 500 sends per variant produces statistically irrelevant results.

---

### 6. WHAT THE VIDEO DOES NOT SHOW
* Automated sending logic or software integrations (e.g., Instantly, Smartlead, HeyReach).
* Code implementation for tracking open/reply rates or automating variant rotation.
* Exact statistical formulas for calculating confidence intervals on reply rates.

===== HOW TO READ THESE =====
Keep: tool names, command strings, error messages, and any claim that appears in BOTH samples.
Flag: anything that appears in only one sample. That is where the model is guessing.
Never trust: timestamps, counts, durations, version numbers it did not clearly read on screen.
