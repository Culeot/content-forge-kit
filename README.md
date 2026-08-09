# Content Forge Kit · The All-in-One Content Forge

> An out-of-the-box **web + video + graphics/text** content-creation methodology kit, packaged as 6 ready-to-use AI skills.
> ⭐ If you find it useful, please give it a star!

---

## What is this

A self-contained content-creation command center. It ships with 6 skills + 2 core assets; any AI agent (Reasonix / Claude Code / Cursor, etc.) can install it and immediately start producing content with this methodology.

**Highlights**:
- 🧠 Dialectical-materialist thinking framework (contradiction analysis / practice & cognition / seeing both sides / seeking truth from facts)
- 🎬 Full pop-science video pipeline: script template → Feynman review → de-AI-ification → motion standards
- 🌐 Awwwards-level web quality methodology (layered lighting / negative letter-spacing / glassmorphism / non-fade transitions)
- ✍️ De-AI copy rewriting (humanizer)
- 🔍 Frontend design anti-pattern detection (impeccable, 60 rules)
- ⚡ GSAP motion reference (easing / timelines / performance)

---

## Directory structure

```
content-forge-kit/
├── README.md               ← this file
├── skills/                 ← 6 skills, ready to use
│   ├── content-forge/      command center (main entry, install this first)
│   ├── humanizer/          de-AI rewriting (mandatory step)
│   ├── feynman-review/     zero-prerequisite review of pop-science content
│   ├── impeccable/         frontend design anti-pattern detection (full scripts included)
│   ├── mao-zedong-perspective/  dialectical-materialist thinking
│   └── gsap-motion/        GSAP motion reference
└── content/
    ├── video-script-template.md   a script is mandatory before making any video
    └── high-end-quality-guide.md    the complete quality methodology
```

---

## Quick install (3 steps)

### Step 1: Install the skills
Copy the 6 folders in `skills/` into your agent's skills directory:

- **Reasonix**: `<Reasonix home>/skills/` (takes effect globally)
- **Claude Code**: `~/.claude/skills/`
- **Cursor**: `~/.cursor/skills/`
- **Other agents**: just read the `SKILL.md` in each folder directly

### Step 2: Place the assets
Copy the 2 files in `content/` into your project directory (recommended under `content/`).

### Step 3: Start using it
Tell your agent:

```
Use the content-forge skill to create content. Read skills/content-forge/SKILL.md to start.
Making a video → first write a script per content/video-script-template.md → pass Feynman review + humanizer → then do the animation
Making a webpage → set the quality bar per content/high-end-quality-guide.md → impeccable review → GSAP motion
Making graphics/text → run humanizer directly to remove the AI flavor
```

Or use the command: `/content-forge make a video about XXX` / `/content-forge make a landing page`

---

## Core rules

1. **All standards are living defaults**: duration / word count / techniques / color palettes are default reference values — use whatever fits the project best; there are only two iron rules — zero errors in math/pop-science content, and all outward-facing content must pass humanizer
2. **Dialectical-materialist thinking**: approach any problem in four steps — where is the contradiction / is the investigation sufficient / see both sides / seek truth from facts
3. **Self-check before delivery**: review everything from the top, confirm it's correct, then deliver

---

## Dependencies

- `impeccable`'s detection script requires Node.js (it still works without it — the automatic checks are just skipped)
- GSAP is a frontend library; load it via CDN when doing motion — no installation needed
- All other skills are pure Markdown, readable by any agent

---

## License

MIT · free to use, modify, and distribute (note: some assets are compiled from publicly available methodologies; see the notes inside each file for details)

*Made by Tomato · stars welcome ⭐*
