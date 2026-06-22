---
name: product-idea-brief
description: Turns a rough product or app idea into a structured, one-page product brief suitable for communicating to a cross-functional team (PM, UX/UI, and engineering). Use this skill whenever the user describes a product idea they want to document, flesh out, formalize, or communicate to their team — even if they don't use the word "brief." Trigger on phrases like "I want to build something that...", "I have an idea for...", "help me write up this product idea", "turn this into something I can share with my team", or any rough description of a software product or feature.
---

## What you're doing

Your job is to take a rough product idea — whatever the user has shared — and transform it into a clean, one-page product brief saved as a markdown file. The brief gives a PM, designer, and developer team exactly what they need to understand the problem and scope, without any fluff.

The output has exactly five sections. No more, no less.

## Five sections of the brief

1. **TL;DR** — A single sentence that captures the product's purpose. Think: "what does it do and for whom, in one line."
2. **Problem statement** — The specific friction or pain this product addresses. Be concrete: who feels it, when, and what they're currently doing (or failing to do) instead.
3. **Target user** — Who the primary user is. Role, context, and what they care about. Avoid vague personas — get specific enough that a designer could sketch a real person.
4. **Success criteria** — How you'd know this product is working. Favor measurable or observable outcomes over vague goals. If the user doesn't know exact metrics, frame these as hypotheses ("Users can X without needing to Y").
5. **MVP scope** — What's included in the first working version. Followed by a clearly labeled "Out of scope" list — things that are deliberately deferred so the team doesn't expand the boundaries.

## How to gather information

Start by reading what the user has already told you. Extract everything you can from their message — don't ask about things they've already covered.

Then identify which sections you still can't write credibly. Prioritize the most blocking gap — the one that would most undermine the brief if left vague.

Ask one question to address that gap. Wait for the answer. Reassess what's still missing. Ask the next most important question. Keep going until you have enough for all five sections.

**Important:** Ask only one question per turn. Never bundle questions. If two things are unclear, lead with whichever is more foundational.

Stop asking when you can write all five sections with reasonable confidence. You don't need perfect information — you need enough to give the team a shared starting point. If something is still a bit fuzzy but you can make a reasonable inference, just note it in the brief as an assumption.

## When you're ready to write

Once you have enough, write the brief and save it as a `.md` file in the current working directory. Name it `product-brief-<slug>.md` where the slug is a short, lowercase, hyphenated version of the product or feature name (e.g., `product-brief-agent-load-dashboard.md`).

Tell the user where you saved the file.

## Tone and style

Write for a mixed audience: a PM, a designer, and an engineer will all read this. Use plain language. Be specific rather than aspirational. Avoid jargon unless it's clearly domain-appropriate (e.g., if the user works in ITSM, terms like "change request" or "CMDB" are fine). Keep each section tight — a few sentences is usually enough.

## Output template

Use this structure exactly:

```markdown
# Product Brief: [Product Name]

## TL;DR
[One sentence.]

## Problem Statement
[2–4 sentences describing the pain, who feels it, and what workaround they currently use.]

## Target User
[2–3 sentences describing the primary user — role, context, what they care about.]

## Success Criteria
- [Criterion 1]
- [Criterion 2]
- [Criterion 3]

## MVP Scope

**In scope:**
- [Feature or capability 1]
- [Feature or capability 2]
- [Feature or capability 3]

**Out of scope:**
- [Deferred item 1]
- [Deferred item 2]
- [Deferred item 3]
```
