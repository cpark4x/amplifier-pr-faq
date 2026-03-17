---
name: writing-pr-faq
description: Use when creating a PR/FAQ, pitch document, or Working Backwards press release for a product, bundle, tool, or project
---

# Writing a PR/FAQ

A PR/FAQ is a thinking tool, not a document format. The press release forces you to reason from the customer's perspective — if you can't write a clear one, you don't understand the product well enough.

**Before writing, answer these five questions** (Bryar framework):

1. Who is the customer?
2. What is their problem?
3. What is the solution, in their language?
4. Would they change behavior to adopt it?
5. Is it worth doing?

If you can't answer all five, the PR/FAQ isn't ready to write.

## Structure

```
# [product name] — PR/FAQ

## Press Release                    (one page max)
## What the output looks like       (concrete before/after)
## Frequently Asked Questions       (6-10 questions)
```

## Press Release

**One page max.** Two tight paragraphs is ideal for developer tools.

**Paragraph 1 — Problem and solution.** Bolded opening sentence with the value prop. What's broken, what this does, who it's for. End with audience signal — name the situations where this matters.

**Paragraph 2 — How it works.** One operational detail that makes the product concrete. Speed, modes, key mechanic. No feature lists.

**Exclude:** datelines, fake quotes, feature rosters, corporate framing ("we are excited to announce"), superlatives.

## Concrete Example

**Show real output immediately after the press release.** Before/after if the product transforms something. This is the most persuasive element — never skip it, never substitute an abstract description.

## FAQs

**6-10 questions. Single list. Include hard questions about viability.**

**Required:**

1. **What does it do?** — one paragraph, concrete
2. **How do I install it?** — exact commands, copy-pasteable
3. **Can I try it in 5 minutes?** — smallest test, what to type, what to expect
4. **How is this different from [existing approach]?** — honest comparison
5. **What are the limitations?** — name them honestly
6. **At least one hard question** — what would cause this to fail? What's the biggest risk?

**Anti-patterns:** more than 10 FAQs, only easy questions, limitations buried last.

## Writing Sharp FAQs

Structure gets you to 7/10. These rules get you to 9.

**Limitations as scannable lists, not paragraphs.** One bullet per limitation.

**Viability risks as concrete scenarios, not abstract categories.**

```
# Bad:  Output formatting may cause friction for users.
# Good: You generate a brief in 15 minutes, then spend 10 minutes
#        stripping trace references before you can paste it into Slack.
```

**Features as outcomes, not capabilities.**

```
# Bad:  | storyteller | Turns structured findings into narrative |
# Good: | storyteller | Board decks that tell a story instead of dumping data |
```

## Checklist

- [ ] Five questions answered
- [ ] Press release fits one page
- [ ] No fake quotes, datelines, or corporate framing
- [ ] Concrete example shows real output
- [ ] Install command is copy-pasteable
- [ ] "Try it in 5 minutes" FAQ exists
- [ ] At least one hard viability question
- [ ] Limitations stated honestly as scannable list
- [ ] 6-10 FAQs total
- [ ] Reads in under 3 minutes
