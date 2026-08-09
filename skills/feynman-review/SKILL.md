---
name: feynman-review
description: Feynman review for science-explainer content: nitpick as a zero-background reader across six dimensions plus scoring; failures are sent back. Mandatory review for all science-explainer deliverables.
---

# Feynman Review Playbook

User requirement: from now on, **all science-explainer content** (Xiaohongshu posts, video scripts, knowledge explainers) must pass this "zero-background reader" review after generation. This is a long-term mechanism, not a one-off action.

## Review Process

1. **Enter the zero-background state**: pretend you know nothing about the field and understand only from the content itself.
2. **First read**: write down "what did I learn" — how many points can you retell?
3. **Second read**: note "what would I ask" — where does it feel off, which term is unclear, which number is left hanging.
4. **Check against the original**: answer each of your own questions one by one, and find where the content failed to meet the reader's expectations.
5. **Score and conclude** (see below).

## Six Review Dimensions

1. **Phenomenon chain**: can a layperson retell the full process? (skipped steps / scrambled order → fail)
2. **Principle hook**: is the biggest counterintuitive point explained? Is what readers most want to know covered first?
3. **Terms grounded**: is every term defined in one sentence? (naming a term without explaining → fail)
4. **Number anchors**: does every number/angle state "from what to what"?
5. **Clean language**: mixed-in English, AI-flavored wording, awkward colloquialisms → points deducted
6. **Image-text consistency**: do the images cover all key steps of the body text?

## Scoring & Outcomes

- 5 stars: a zero-background reader can retell it + draw inferences → pass
- 4 stars: phenomenon is clear, minor flaws → pass (note optimization points)
- 3 stars: phenomenon retellable but principle missing → **send back for rewrite** (add principle hooks / ground the terms)
- ≤2 stars: phenomenon itself unclear → **send back for rewrite**

## Output Format (for Delivery)

```
## Feynman Review Result
What was learned (retelling):...
Where it gets stuck / questions: ① ② ③
Dimension score table: phenomenon chain / principle hook / terms grounded / number anchors / clean language / image-text consistency (X/5 each)
Conclusion: pass / send back for rewrite + specific improvement suggestions
```

## Where It Lives

- Full review criteria: `ai-content-pipeline/docs/feynman-review.md`
- After generating a post and before publishing, proactively run this review and write the result into the publishing log.
