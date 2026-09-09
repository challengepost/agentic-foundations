---
name: 2-plan
description: Plan the project before any code — find the idea, define the product, choose the simplest architecture. Three reviewed documents in one skill.
---

# 2-plan — Plan the Whole Thing First

## Where Are We

Before anything else, look at `docs/`. Never infer state from conversation memory — the files are the truth.

1. List which of these exist: `learner-profile.md`, `scope.md`, `prd.md`, `spec.md`, `checklist.md`. Read the `status:` line in each one's frontmatter.
2. Say back where the learner is, in one sentence.
3. Route:
   - No `learner-profile.md` → tell them to run `1-start`, stop.
   - Otherwise resume at the **first document that is not `status: approved`**, in order scope → prd → spec:
     - missing → begin that phase fresh
     - `status: draft` → read it back, summarize in a few sentences, ask "pick up here or redo this one?"
     - `status: approved` → skip it
   - All three approved → say so, point to `3-build`, stop — unless they say they want to reopen one.

Save every document as soon as its first draft exists, with `status: draft`. Flip to `approved` only on an explicit yes. A draft that lives only in the conversation dies with it.


<!-- TODO: merge prototype 2-scope, 3-prd, 4-spec. Decisions (9/9):
- This is the meat of the curriculum. Linger. No time budget stated anywhere.
- Three phases, three docs, review after each:
  Scope  → docs/scope.md  (idea discovery or shaping, brain dump, stress-test, protect the POC)
  Product → docs/prd.md   (reconstruct core journey first, sort undefined, states, guard POC boundary) — read references/prd-guide.md
  Technical → docs/spec.md (calibrate to profile, derive architecture from product, complexity budget, one concrete recommendation) — read references/spec-patterns.md
- Learner may finish all three in one conversation or start fresh between phases; docs carry context.
- Honor the review-format preference from learner-profile.md (Markdown in terminal, or a simple self-contained HTML render). No project-companion.
- Hand off to 3-build.
-->
