---
name: writing-pr-faq
description: Use when creating a PR/FAQ, pitch document, or Working Backwards press release for a product, bundle, tool, or project
---

# Writing a PR/FAQ

## Overview

A PR/FAQ is Amazon's Working Backwards format: a press release followed by FAQs. But the document is not the point — the **thinking** is. The press release format forces you to reason from the customer's perspective and makes half-baked thinking impossible to hide. If you can't write a clear press release, you don't understand the product well enough.

Before writing anything, answer these five questions (from Colin Bryar, ex-Amazon VP):

1. **Who is the customer?**
2. **What is their problem?**
3. **What is the solution, in their language?**
4. **Would they change behavior to adopt it?**
5. **Is it worth doing?**

If you can't answer all five, the PR/FAQ isn't ready to write.

## Structure

```
# [product name] — PR/FAQ

## Press Release          (one page max — keep it tight)
## What the output looks like   (concrete before/after example)
## Frequently Asked Questions   (6-10 questions)
```

## Press Release Rules

**One page max.** Keep it as short as possible — two tight paragraphs is ideal for developer tools. The constraint is the point: if you can't explain it in a page, you haven't clarified your thinking enough.

**Paragraph 1 — The problem and solution.** One bolded opening sentence that states the value prop. Then: what's broken today, what this does differently, who it's for. End with the audience signal — name the specific situations where this matters (board briefs, vendor evaluations, CI pipelines — whatever applies).

**Paragraph 2 — How it works at the user level.** One operational detail that makes the product concrete. Speed, modes, key mechanic. No feature lists — pick the single most important thing a user would want to know before trying it.

**What does NOT belong in the press release:**
- Datelines ("Seattle, WA — Today, we are announcing...")
- Fake customer quotes (never fabricate testimonials)
- Feature rosters (that's what FAQs are for)
- Internal/corporate framing ("we are excited to announce")
- Superlatives ("revolutionary", "game-changing", "seamless")

## The Concrete Example Section

**Immediately after the press release, show what the product actually produces.**

This is the single most persuasive element in the document. Show a before/after, a sample output, a screenshot — whatever makes the value tangible. The reader should see the difference, not be told about it.

If the product transforms input to output, show both. If it produces artifacts, show a real one. If it's a workflow, show the result.

**Never skip this section.** Abstract descriptions of output are not substitutes.

## FAQ Rules

**6-10 questions. Single list, but include hard questions about viability.**

Amazon's original format splits FAQs into external (customer) and internal (stakeholder). For open-source and developer tools, the audience is usually the same — but the *function* of the internal FAQ matters: it forces you to confront feasibility, risks, and reasons the product might fail. Keep that rigor even without the formal split.

**Required FAQs (always include these):**

1. **What does it do?** — One paragraph, concrete
2. **How do I install it?** — Exact commands, copy-pasteable
3. **Can I try it in 5 minutes?** — The smallest possible test. What to type, what to expect, how long it takes
4. **How is this different from [existing approach]?** — Honest comparison, not marketing
5. **What are the limitations?** — Honest. Name them. This builds credibility

**Hard questions (include at least one):**

These replace the function of Amazon's internal FAQ — they force you to address viability, not just desirability:

- What would cause this to fail?
- What's the biggest risk or tradeoff?
- What can't it do that users will expect it to?
- Is it slow? Does it cost more? Why is that worth it?

**Optional FAQs (include when relevant):**

- Can I use parts independently? (if it's composable)
- What happens when it fails? (if failure modes matter)

**FAQ anti-patterns:**
- More than 10 FAQs (trim or merge — the reader won't finish)
- FAQs that repeat press release content verbatim
- Rhetorical questions nobody would actually ask
- Only easy questions — no hard ones about viability or risks
- Hiding limitations in the last FAQ hoping nobody reads that far

## Tone

**Direct, honest, conversational.** Write like you're explaining to a colleague, not announcing to shareholders.

- State tradeoffs plainly: "Yes, it's slower. Here's why and when that's worth it."
- Acknowledge limitations early, not buried at the end
- No fake excitement ("we're thrilled to announce")
- Use the product's actual name as users will encounter it (CLI name, package name — not a title-cased marketing name unless that's the real name)

## Checklist

Before calling the PR/FAQ done:

- [ ] Five questions answered (customer, problem, solution, behavior change, worth doing)
- [ ] Press release fits on one page
- [ ] No fake quotes or testimonials
- [ ] No dateline or corporate framing
- [ ] Concrete example section shows real output
- [ ] Install command is copy-pasteable
- [ ] "Try it in 5 minutes" FAQ exists
- [ ] At least one hard question about viability/risks
- [ ] Limitations are stated honestly, not buried
- [ ] Total FAQs between 6 and 10
- [ ] Document reads in under 3 minutes
