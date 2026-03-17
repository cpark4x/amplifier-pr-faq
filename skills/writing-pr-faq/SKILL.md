---
name: writing-pr-faq
description: Use when creating a PR/FAQ, pitch document, or Working Backwards press release for a product, bundle, tool, or project
---

# Writing a PR/FAQ

## Overview

A PR/FAQ is a one-document pitch: a press release followed by FAQs. Amazon's Working Backwards format adapted for open-source and developer tools. The goal is a document a prospective user reads and knows whether this is for them — in under 3 minutes.

## Structure

```
# [product name] — PR/FAQ

## Press Release          (2 paragraphs only)
## What the output looks like   (concrete before/after example)
## Frequently Asked Questions   (6-10 questions)
```

## Press Release Rules

**Exactly 2 paragraphs.** No more.

**Paragraph 1 — The problem and solution.** One bolded opening sentence that states the value prop. Then: what's broken today, what this does differently, who it's for. End with the audience signal — name the specific situations where this matters (board briefs, vendor evaluations, CI pipelines — whatever applies).

**Paragraph 2 — How it works at the user level.** One operational detail that makes the product concrete. Speed, modes, key mechanic. No feature lists — pick the single most important thing a user would want to know before trying it.

**What does NOT belong in the press release:**
- Datelines ("Seattle, WA — Today, we are announcing...")
- Fake customer quotes (never fabricate testimonials)
- Feature rosters (that's what FAQs are for)
- Internal/corporate framing ("we are excited to announce")
- More than 2 paragraphs

## The Concrete Example Section

**Immediately after the press release, show what the product actually produces.**

This is the single most persuasive element in the document. Show a before/after, a sample output, a screenshot — whatever makes the value tangible. The reader should see the difference, not be told about it.

If the product transforms input to output, show both. If it produces artifacts, show a real one. If it's a workflow, show the result.

**Never skip this section.** Abstract descriptions of output are not substitutes.

## FAQ Rules

**6-10 questions. No internal/external split.**

The internal/external FAQ split is for corporate Amazon documents where stakeholders and customers are different audiences. For open-source, developer tools, and bundles, there's one audience: prospective users. One flat FAQ list.

**Required FAQs (always include these):**

1. **What does it do?** — One paragraph, concrete
2. **How do I install it?** — Exact commands, copy-pasteable
3. **Can I try it in 5 minutes?** — The smallest possible test. What to type, what to expect, how long it takes
4. **How is this different from [existing approach]?** — Honest comparison, not marketing
5. **What are the limitations?** — Honest. Name them. This builds credibility

**Optional FAQs (include when relevant):**

- Is it slow? (if it's not instant)
- Does it cost more? (if it consumes paid resources)
- Can I use parts independently? (if it's composable)
- What happens when it fails? (if failure modes matter)

**FAQ anti-patterns:**
- More than 10 FAQs (trim or merge — the reader won't finish)
- FAQs that repeat press release content verbatim
- Rhetorical questions nobody would actually ask
- Hiding limitations in the last FAQ hoping nobody reads that far

## Tone

**Direct, honest, conversational.** Write like you're explaining to a colleague, not announcing to shareholders.

- State tradeoffs plainly: "Yes, it's slower. Here's why and when that's worth it."
- Acknowledge limitations early, not buried at the end
- No superlatives ("revolutionary", "game-changing", "seamless")
- No fake excitement ("we're thrilled to announce")
- Use the product's actual name as users will encounter it (CLI name, package name — not a title-cased marketing name unless that's the real name)

## Checklist

Before calling the PR/FAQ done:

- [ ] Press release is exactly 2 paragraphs
- [ ] No fake quotes or testimonials
- [ ] No dateline or corporate framing
- [ ] Concrete example section shows real output
- [ ] Install command is copy-pasteable
- [ ] "Try it in 5 minutes" FAQ exists
- [ ] Limitations are stated honestly, not buried
- [ ] Total FAQs between 6 and 10
- [ ] No internal/external FAQ split
- [ ] Document reads in under 3 minutes
