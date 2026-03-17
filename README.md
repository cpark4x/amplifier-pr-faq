# amplifier-pr-faq

You ask an AI to write a PR/FAQ. It produces a 23-question corporate press release with a fake customer quote, a dateline from Seattle, and an internal/external FAQ split nobody asked for. The actual product is invisible under five paragraphs of filler.

This is an [Amplifier skill](https://github.com/microsoft/amplifier) that teaches AI agents how to write Working Backwards PR/FAQ documents that are tight, honest, and concrete. It was built with TDD — baseline-tested against real failure patterns, then revised with sourced research on Amazon's original format.

What changes: press releases stay under a page, every PR/FAQ includes a concrete before/after example of what the product produces, FAQs include hard questions about viability (not just softball features), and limitations are stated honestly instead of buried.

---

## What a skill-guided PR/FAQ looks like

Without the skill, an AI writes this press release:

> **Seattle, WA** — Today, we are announcing **MyTool**, a powerful framework for automated research. "We had 40,000 lines of code with inconsistent documentation," said Dana Reeves, a senior engineer at a mid-stage startup...

With the skill:

> **mytool turns your Python codebase into clean API documentation in seconds, without configuration files or markup boilerplate.** Most Python projects have incomplete or outdated docs because maintaining them by hand is boring...

No dateline. No fake quote. Problem first. Product name as users encounter it.

---

## Quick start

**Use on demand in any Amplifier session:**

```
load_skill(source="git+https://github.com/cpark4x/amplifier-pr-faq@main#subdirectory=skills")
load_skill(skill_name="writing-pr-faq")
```

Then ask: "Write a PR/FAQ for [your project]."

**Or install locally for instant access:**

```bash
mkdir -p ~/.amplifier/skills/writing-pr-faq
cp skills/writing-pr-faq/SKILL.md ~/.amplifier/skills/writing-pr-faq/SKILL.md
```

Then `load_skill(skill_name="writing-pr-faq")` works in any session without the git fetch.

---

## What the skill teaches

- Answer five prerequisite questions before writing (Bryar framework)
- Press release: one page max, problem-first, no corporate filler
- Concrete example section immediately after the press release
- 6-10 FAQs including at least one hard question about viability/risks
- Required FAQs: what it does, install, try-in-5-minutes, comparison, limitations
- Direct tone — tradeoffs stated plainly, no superlatives

---

## Built by

[Chris Park](https://www.linkedin.com/in/chrispark) — Microsoft Office of the CTO, AI Incubation.
