# cold-email-copy

A meta-skill for Claude Code that writes cold emails that read like a person wrote them.

It runs four passes, in order:

0. **Intake** — asks for industry, role, and business type before writing a word.
1. **Draft** — the four-part frame: personalization, who am I, offer, CTA.
2. **Persuade** — conversion pass (bundled `copywriting` skill).
3. **Humanize** — 53-pattern AI-tell pass (bundled `humanizer` skill).
4. **Grade** — script grading in-workspace, a manual checklist outside it.

## Install

    git clone <this repo> ~/.claude/skills/cold-email-copy

Then `/cold-email-copy selling X to Y` in Claude Code.

## Layout

- `SKILL.md` — the skill itself
- `reference/humanizer/` — bundled humanizer skill
- `reference/copywriting/` — bundled copywriting skill
- `reference/psychology.md` — the persuasion principles underneath
- `SPEC.md`, `notes/` — source notes with confidence labels
