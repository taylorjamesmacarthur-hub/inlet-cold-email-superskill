<p align="center">
  <img src="assets/macarthur-media-logo.png" width="300" alt="MacArthur Media">
</p>

# inlet-cold-email-superskill

**Built by MacArthur Media for Inlet Recruiting.**

A meta-skill for Claude Code that writes cold emails that read like a person wrote them.
Built on **Nick Saraev's four-part cold email formula**, wrapped in an intake interview,
two editing passes, and a self-grader.

It runs four passes, in order:

0. **Intake** — asks for industry, role, and business type before writing a word.
1. **Draft** — the four-part frame: personalization, who am I, offer, CTA.
2. **Persuade** — conversion pass (bundled `copywriting` skill).
3. **Humanize** — 53-pattern AI-tell pass (bundled `humanizer` skill).
4. **Grade** — script grading in-workspace, a manual checklist outside it.

**New here?** [DIAGRAMS.md](DIAGRAMS.md) explains the whole thing in six diagrams,
with recruiting examples and no jargon.

<p align="center">
  <img src="assets/diagrams/01-pipeline.svg" width="880" alt="The pipeline">
</p>

## Install

    git clone <this repo> ~/.claude/skills/inlet-cold-email-superskill

Then `/inlet-cold-email-superskill selling X to Y` in Claude Code.

## Layout

- `SKILL.md` — the skill itself
- `DIAGRAMS.md` — six plain-English diagrams, recruiting examples
- `assets/` — MacArthur Media brand marks
- `reference/humanizer/` — bundled humanizer skill
- `reference/copywriting/` — bundled copywriting skill
- `reference/psychology.md` — the persuasion principles underneath
- `SPEC.md`, `notes/` — source notes with confidence labels

---

<p align="center"><sub>MacArthur Media · built for Inlet Recruiting</sub></p>
