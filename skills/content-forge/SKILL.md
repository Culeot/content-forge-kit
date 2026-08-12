---
name: content-forge
description: |
  Content Forge all-in-one kit: the complete methodology command center for web/video/graphic content production. Trigger words: build a webpage, make a video, write copy, content creation, high-end quality, visual design. Embeds dialectical-materialist thinking, high-end quality standards, video scripting workflow, feynman review, and humanizer de-AI-ification, and routes to sub-skills like impeccable/GSAP.
  中文:内容锻造全家桶:网页/视频/图文制作的完整方法论指挥中心。触发词:做网页、做视频、做文案、内容创作、高端质感、视觉设计。内嵌辩证唯物主义思考、高端质感标准、视频脚本流程、费曼审查、humanizer 去 AI 味,并路由到 impeccable/GSAP 等子 skill。
---

# Content Forge (All-in-One Command Center)

> The user's (Tomato) personal creation methodology kit. **Not for commercial use, personal use only.**
> For any "build a webpage / make a video / write copy" task, follow this skill's workflow first.

---

## Core Principle: All Standards Are Living, Not Rigid

**Everything written in this skill — durations, word counts, techniques, color schemes, workflows, review requirements — is a "default reference value", not a "hard rule". Before starting, choose what best fits the actual situation of the project; deviating from defaults or switching approaches is allowed.**

- Templates are a starting point, not shackles: adjust script structure, copy length, and shot count to the actual content
- Use techniques on demand: not every project needs every technique; what fits is what's good
- The only two inviolable bottom lines (explicitly required by the user):
  1. **Zero errors in math/science content**
  2. **Anything published externally must first pass humanizer to remove the AI flavor**
- When unsure: first use dialectical materialism to think through "what approach best fits this project", then act

---

## 0. Thinking Mode (Think First, Then Act)

Before any creation, think it through with the four dialectical-materialist steps (don't write it out, just run it mentally):
1. **Where's the contradiction?** — What is the core contradiction / core selling point of this content? (What problem is the user really solving?)
2. **Enough investigation?** — Are materials, data, and references sufficient? If not, research first
3. **Split into two** — Benefits vs. costs, goals vs. constraints
4. **Seek truth from facts** — Set the plan based on actual conditions (platform / duration / audience)

---

## 1. Task Routing (Determine the Type First)

| Task Type | Which Workflow | Deliverable |
|---|---|---|
| **Video** | See §2 (script → feynman → humanizer → animation) | `videos/<project>/script.json` + final product |
| **Web/Frontend** | See §3 (quality standards → impeccable → GSAP) | Page code |
| **Graphic/Copy** | See §4 (humanizer de-AI-ification) | Copy |

---

## 2. Video Workflow (Science-Explainer Shorts)

### 2.1 Script Must Come First
- Material: `content/video-script-template.md` (full template, 87 lines)
- Process: dispatch a sub-agent to generate `script.json` per the template (shot list / four-part copy / motion effects / visuals / voiceover & BGM / quality red lines) → **must** pass feynman review + humanizer → user confirmation → then animate
- Structure: hook (0-3s) → negation (3-6s) → core breakdown (6-32s, zero-math-error red line) → elevation (32-42s, life metaphor)
- Copy constraints: 550-700 characters, each sentence ≤25 characters, terms must be explained in one sentence on first appearance, conversational tone

### 2.2 Quality Standards (Hard Requirements)
- Material: `content/high-end-quality-guide.md` (full guide, 159 lines)
- Core techniques (universal every time): deep blue-gray (not pure black) background + 3-5 layers of faint light + fading grid + 3% noise; negative letter-spacing -0.03em on titles; white at 55-65% opacity instead of pure gray; glassmorphism; layered glow; GSAP `power3.out`/`expo.out` + stagger; no pure fade transitions (use scale-zoom-in / displacement); Mono ticks + fading dividers + viewfinder corners
- ⚠️ **Techniques are universal, visuals are customized per theme**: colors/materials/fonts are decided per project; reusing the same skin is forbidden (badminton = purple & gold, health = fresh & clean, tech = deep blue…)

### 2.3 Motion Effects
- Route to GSAP skills: `hyperframes/skills/hyperframes-animation/adapters/` (gsap-easing-and-stagger / gsap-timeline-and-labels / gsap-transforms-and-perf)
- Red lines: no layout-property animation (left/fontSize), use transform; no linear easing

### 2.4 Voiceover & Publishing
- edge-tts (Yunxi bright male voice, +45% speed); BGM at 0.2-0.25 so it doesn't cover the voiceover; Xiaohongshu publishing via `publish_video_xhs.py`

---

## 3. Web/Frontend Workflow

### 3.1 Define the Visual World First (Not Code First)
- For each project, first define: theme colors + materials + fonts → then apply techniques
- Style anchor references: linear.app / vercel.com / raycast.com, Awwwards SOTD level
- Anti-pattern red lines: no pure black, no harsh neon, no linear easing, no everything-at-once

### 3.2 Quality Techniques (Same as §2.2, Use on Demand)
- Material: `content/high-end-quality-guide.md`

### 3.3 Design Review
- Route to the `impeccable` skill (frontend design anti-pattern detection: AI-flavored UI traits, accessibility, contrast, typography)
- Self-check after completion: layered light? negative letter-spacing? non-fade transitions? clear visual rhythm?

### 3.4 Motion Effects
- Route to GSAP skills (same as §2.3)

---

## 4. Graphic/Copy Workflow

### 4.1 Must Pass humanizer
- Route to the `humanizer` skill (de-AI-ification: clichés / template sentences / no personal trace → authentic human tone)

---

## 5. Quality Red Lines (Pre-Delivery Self-Check, Applied Flexibly per the Core Principle)

1. **Zero-error red line**: for math/science content, numbers, formulas, and conclusions must be exact (user's hard requirement)
2. **AI-flavor red line**: externally published content must not be delivered without passing humanizer (user's hard requirement)
3. **Quality**: judge per actual project needs — projects requiring a premium feel must meet the bar (layered light / negative letter-spacing / non-fade transitions); simple projects don't force it
4. **Review**: video scripts go through feynman review by default (a zero-background reader nitpicks); simple content may skip it
5. **Self-check red line**: before delivery, do a full self-check from the top and confirm everything is correct

---

## 6. Related Skills & Materials (Full Index)

**Sub-skills (routed on demand):**
- `humanizer` (global): de-AI-ification rewriting
- `feynman-review` (project): zero-background review of science content
- `impeccable` (global): frontend design anti-pattern detection
- `mao-zedong-perspective` (global): dialectical-materialist thinking
- GSAP series (hyperframes): gsap-easing-and-stagger / gsap-timeline-and-labels / gsap-transforms-and-perf / gsap-effects

**Material files (global-workspace/content/):**
- `video-script-template.md` — full video script template
- `high-end-quality-guide.md` — full quality methodology guide

**External libraries (already registered, do not reinstall):**
- Full hyperframes suite (GSAP/Three/Lottie/TypeGPU and other animation skills)
- impeccable (frontend design review)

---

## 7. Usage

- Shorthand: `/content-forge` or `run_skill({name: "content-forge", arguments: "what to do"})`
- You can also just say "make a video", "build a landing page", or "write some copy" — this skill automatically takes over the workflow
- When dispatching sub-agents for specific steps, pass them the corresponding material file paths as well
