---
doc: learner-profile
---
<!-- This template captures the few things about the learner that later phases actually use.
     Every downstream skill reads this document to calibrate depth, tone, and how much of a
     decision to hand back to the learner. Keep it scannable and short.

     Two rules for filling it in:
     1. Record what the learner demonstrated, with a short quote or paraphrase as evidence.
     2. Do not infer beyond the evidence, and do not assign fixed or confident labels.
        "Not established" is an acceptable and useful value. -->

# Learner Profile

## Demonstrated Technical and Agent Experience
What they have actually built or attempted, and what they did versus what the AI did.
Which tools, languages, or agents came up — and which they used fluently versus named vaguely.
Evidence: quote or paraphrase the part of their story this is based on.
> Used by `2-plan` (what they can realistically get built) and `2-plan` (never ask them to choose between options they can't evaluate).

## Desired Learning Outcome
The capability they want by the end — usually distinct from the app itself.
Evidence: their own words.
> Used by `2-plan` to decide how deep to go and where to invest explanation, and by `2-plan` as an angle to open the learner up when answers get short.

## Vocabulary and Concepts Likely to Need Explanation
Terms that will come up in planning or build that they did not use or seemed unsure about.
Terms they clearly already own, so we don't over-explain them.
> Used by `2-plan`, `2-plan`, `3-build`, and `3-build` to pitch explanations at the right level.

## Collaboration and Communication Preferences
How they like an agent to communicate, how much initiative they welcome, and what makes collaboration feel useful rather than intrusive.
Evidence: their own words.
> Used by `2-plan` through `3-build` to calibrate tone, proactivity, challenge, and how much narration to provide.

## Areas Where the Learner Wants Ownership
Decisions they said they want to make themselves.
Evidence: their own words.
> Used by `2-plan`, `2-plan`, and `2-plan`: recommend here, but let them decide.

## Likely Support Needs
Where they asked to slow down, and where the story in their answers suggests friction.
> Used by `2-plan`, `2-plan`, `2-plan`, and `3-build` to decide when to walk through something versus proceed.

## Review Format

<!-- Ask once in 1-start. `markdown` = the agent reviews planning documents with the learner in the
     terminal. `html` = the agent also renders each planning document as a simple self-contained
     HTML page the learner opens in a browser. Markdown files stay canonical either way. -->

markdown | html

## Notes and Open Questions
Anything relevant that doesn't fit above, and anything still unknown that a later phase may need to ask about.
> Read by `2-plan`, the next phase and the longest conversation — it picks up anything
> left unresolved here while it already has the learner talking.
