# Detailed Video Script Prompt Template (Tomato Talks Knowledge · for the pipeline)

> Purpose: before making any pop-science short video, use this template to generate a **complete video script** first; only proceed to animation after it is confirmed correct.
> Execution: a sub-agent may be dispatched to generate the script for a specific episode following this template; the output must pass Feynman review + humanizer.
> Output file: `videos/<project>/script.json` (structured, for the animation to follow directly).

---

## Prompt body to feed the AI (copy the content below, replacing the 【】 placeholders)

You are a veteran short-video director + motion designer + pop-science writer. For the pop-science video below, output a **directly executable storyboard script**, in Simplified Chinese, as JSON.

### 1. Basic information
- Topic: 【e.g., why 0.999… equals 1】
- Target platform: 【Xiaohongshu (RED)】 (vertical 1080×1920, 9:16)
- Target duration: 【35–45 seconds】 (fast-paced; ≤45s recommended on Xiaohongshu)
- Style reference: Jiaohuanlü-style pop-science commentary (dark tech aesthetic + bold typography + lightweight motion)
- Target audience: 【complete beginners】
- Overall emotional arc: 【curiosity → subversion → clarity → a touch of warmth】

### 2. Copy (voiceover script)
Write it in a four-part structure, marking each sentence's emotion with 【】:
1. **Hook** (0–3s): pose a "taken-for-granted" intuition, ending with a rhetorical question ("…right?")
2. **Rebuttal** (3–6s): a firm "of course not"
3. **Core breakdown** (6–32s): concept definition + proof/examples (math content must have zero errors!)
4. **Elevation** (32–42s): "what I mean is" + extend the concept into a metaphor about life/relationships

Constraints: 550–700 characters in total; each sentence ≤ 25 characters; every technical term must be explained in one sentence on first appearance; conversational, like talking to a friend.

### 3. Storyboard table (the core deliverable)
Output each shot with the following fields:

```json
{
  "shots": [
    {
      "id": 1,
      "start": 0.0, "end": 3.0,
      "narration": "the full voiceover sentence",
      "visuals": "what the main text/graphics are and how they are laid out",
      "motion": "entrance style (pop in / fade in / slide in / scale), duration",
      "vfx": "glow / particles / number rolling / formula reveal, etc.",
      "subtitle": "the on-screen subtitle text (may be shorter than the narration)",
      "transition": "cut in / cut out style (fade out / slide out / scale)",
      "design_notes": "specific handling of colors / font sizes / hierarchy / whitespace"
    }
  ]
}
```

### 4. Motion & VFX specs (must be annotated for every shot)
- **Easing standard (unified across the whole film; the #1 factor of premium feel)**: entrances use `expo.out`; grouped elements `stagger 0.06`; results/conclusions use `back.out(1.4)` micro-bounce; background light blobs `sine.inOut` slow 18–25s drifting breath (the frame is always alive)
- **Entrance motion** (pick one, unified across the film): fade in (0.4–0.6s), pop in (scale 1.2→1), slide in (y offset)
- **Emphasis motion**: key numbers/conclusions use scale-up + **layered glow** (near light + far light + ambient — three layers of text-shadow); give it to only the single most important element per shot
- **Formula/derivation animation**: appear line by line, term-by-term replacement, number rolling (use GSAP; layout properties like left/fontSize are forbidden)
- **Data visualization**: number lines, bar charts, ratio diagrams, etc., must appear in sync with the narration
- **Transitions (pure fades are forbidden — that's the PowerPoint feel)**: key scenes use a zoom-dive (old shot scale 8 fade out → new shot scale 0.3 pop in) or slide transitions (xPercent ±100); fades are only for emotional softening
- **VFX red lines**: dark tech aesthetic; glow uses rgba gradients; cheap multicolor gradients are forbidden

### 5. Visual specs (locked across the whole film, to Awwwards-level standards)
- **Background (layered light, never flat)**: deep blue-black `#06070B` (not pure black) + top spotlight `radial-gradient(1200px 600px at 50% -10%, rgba(88,130,255,.12), transparent)` + corner accent light + **fading grid** (radial mask fade; full-bleed tiling is forbidden) + 3% noise to kill banding + 2 drifting light blobs
- **Card materials (customized per theme; default glassmorphism is forbidden!)**: the material is determined by the content theme — tech/data = carbon-fiber weave + brushed metal; luxury/brand = metal + brushing + a sweeping highlight; fresh/health = paper + soft shadows; toys = plastic + colored light. Glassmorphism (backdrop-blur white translucency) is an overused 2020 cliché — **banned by default**. For each project, first define a material language (name + physicality + texture details), then write the CSS
- **Primary text**: white `#F0F3F6`; **headlines use negative letter-spacing `letter-spacing: -0.03em`**, line-height 1.1, bold 700
- **Secondary text**: white at 55–60% opacity `rgba(255,255,255,.6)` (pure gray is forbidden)
- **Eyebrow label**: uppercase + `letter-spacing: 0.15em` + Mono font, white 50%
- **Accent colors (90% monochrome + 10% accent, ≤1 per screen)**: orange #FF6B1A / blue #4CC9FF / green #3FB950
- **Typography**: headlines 84–148px, body 44–56px, subtitles 48px at ≥260px from the bottom; ≤40 characters per screen, ≤3 hierarchy levels
- **Details (instantly premium)**: fading dividers `linear-gradient(90deg, transparent, rgba(255,255,255,.12), transparent)`; Mono numeric tickers (corner `001/007`, progress, white 40%); 24px L-shaped 1px viewfinder corners at white 25%; a 1px light strip on card tops
- **Style anchor words** (to feed the AI): in the style of linear.app / vercel.com / raycast.com, Awwwards SOTD quality; deep blue-black background, radial glow, film grain, faint dotted grid with radial fade, tight letter-spacing, weight contrast, glassmorphism, GSAP expo.out, stagger 0.06; counter-examples: no pure black, no harsh neon, no linear easing, no everything-at-once

### 6. Voiceover & BGM
- Voiceover voice: 【Yunxi, sunny male voice】 (lively and emotional), speed +45%, 0.25s between sentences
- BGM: 【choose per content, e.g., the "Love in a Puff" instrumental at 1.2x】, volume 0.2–0.25, must not overpower the voiceover

### 7. Quality red lines (self-check before output)
- [ ] Zero errors in math/science content (every number and every conclusion must be correct)
- [ ] Understandable to complete beginners (Feynman review: complete phenomenon chain, terms grounded, numbers anchored)
- [ ] No AI flavor (natural spoken language, no "in summary"-style clichés)
- [ ] Shot durations sum to the target duration
- [ ] Every shot has motion + transition annotations; no empty shots
- [ ] **Quality bar met (against the 6 items of the High-End Quality Upgrade Guide)**: layered background light / negative letter-spacing typography / layered glow / expo easing + stagger / non-fade transitions / premium details — all are required

---

## Output format

Final deliverable: one `script.json` + a "script brief" of no more than 100 words (what the hook is and where the highlights are).
