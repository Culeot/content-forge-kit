---
name: humanizer
description: AI-taste rewriting: diagnose AI-taste (clichés/template sentences/no personal traces) → rewrite into a real human voice → self-check against the checklist. Mandatory for all outward-facing published content.
---

# Humanizer Playbook (AI-taste rewriting)

User requirement: take AI-generated text (copy, scripts, Xiaohongshu posts, WeChat public account articles, reports) and rewrite it so it reads **like a real person dashed it off**, eliminating any "machine feel." **This is a global mandatory process** (rules defined in the global REASONIX.md, effective in all workspaces): all AI-generated content intended for external publication must pass through this playbook before release; it must not be skipped, unless the user explicitly says "no need to revise."

## Step 1: Diagnose first — don't rush to rewrite

Read through the original text, list the AI-taste issues (see below), and mark the location of each problem. Show the diagnosis to the user first (if the user is present), or proceed directly to rewriting.

## AI-taste checklist (the more hits, the stronger the machine feel)

**Word level:**
- Overuse of stock phrases like "in-depth," "empower," "underlying logic," "essentially," "it's worth noting," "undeniably," "in conclusion," "increasingly," "can be called," "not only... but also..."
- All-purpose filler words: "help," "improve," "optimize," "build," "scenario," "dimension" — whenever a concrete word exists, use it instead
- Overly formal phrasing: using "conduct/implement/execute" where "do/make/handle" would do
- Stacking of hollow adjectives: "powerful," "comprehensive," "excellent," "remarkable" appearing in a row

**Sentence-structure level:**
- Every sentence is complete, symmetrical, and parallel; the rhythm is too uniform (real human writing mixes long and short sentences, with fragments)
- Every paragraph follows the same "claim + explanation + example" three-part template
- Excessive connectives: "first... second... then... finally," "moreover," "meanwhile"
- Three or more clauses crammed into one sentence — suffocating to read

**Content level:**
- Every point gets equal weight; no focus, no hierarchy
- No personal traces: no concrete details, no exceptions, no "last time I..." or "that time when I..."
- No emotional variation: neutral reporting tone throughout
- Too perfect: no filler, no slips, no real-life interjections like "actually," "honestly," or "believe it or not"

## Step 2: Rewriting rules

1. **Replace stock phrases**: find a plain-language substitute for every AI-taste word — "in-depth analysis" → "tear it open and look"; "empower" → "help... get it done"; "in conclusion" → just delete it.
2. **Break the rhythm**: split 1-2 long sentences into short ones; deliberately leave one incomplete, colloquial sentence.
3. **Insert personal traces**: add concrete details, add exceptions, add a sentence with genuine emotion (if the information is accurate and fits the user's persona).
4. **Delete connectives**: wherever meaning alone can carry the flow, cut "first/moreover/meanwhile."
5. **Preserve accuracy**: rewriting changes only the *expression* — never tamper with facts, numbers, or conclusions.
6. **Adapt to the persona**: when the user has a clear persona (e.g., a Xiaohongshu blogger), match that voice; otherwise default to "an ordinary person explaining to a friend."

## Step 3: Self-check (re-read against the checklist)

- Go through the AI-taste checklist item by item and confirm each has been addressed
- Read it aloud (or silently, to feel whether it flows): any sentence that reads awkwardly? Fix it
- Check whether facts/numbers were lost or corrupted during rewriting
- Check whether over-colloquializing introduced ambiguity (plain speech ≠ sloppy grammar; it must read smoothly)

## Output format (for delivery)

```
## Rewrite notes
AI-taste diagnosis: [N] hits (word level: X / sentence level: X / content level: X)
Main changes: ①… ②… ③…
Accuracy preserved: numbers/conclusions unchanged (list any changes item by item)
Self-check result: checklist fully reviewed, no residual AI-taste
Full rewritten text: ...
```

## Where it lives

- The mandatory rule is written into the global `REASONIX.md` (Reasonix home, auto-loaded in all workspaces); this skill is the corresponding execution detail
- Works with `ai-content-pipeline/`: generate content → pass through this playbook first → for science/explainer content, then pass the [[feynman-review]] check → publish
- Xiaohongshu / WeChat public account and other outward-facing copy **must** follow this process; the only exception: the user explicitly says "no need to revise."
