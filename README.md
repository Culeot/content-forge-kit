# Content Forge Kit · 内容锻造全家桶(The All-in-One Content Forge)

> An out-of-the-box **web + video + graphics/text** content-creation methodology kit, packaged as 6 ready-to-use AI skills.
> 开箱即用的**网页+视频+图文**内容创作方法论全家桶,打包成 6 个可直接使用的 AI skill。
> ⭐ If you find it useful, please give it a star! / 觉得有用的话给个 star 吧!

---

## What is this / 这是什么

A self-contained content-creation command center. It ships with 6 skills + 2 core assets; any AI agent (Reasonix / Claude Code / Cursor, etc.) can install it and immediately start producing content with this methodology.

一个自包含的内容创作指挥中心,自带 6 个 skill + 2 份核心资产;任何 AI 智能体(Reasonix / Claude Code / Cursor 等)装上就能立刻按这套方法论产出内容。

**Highlights / 亮点**:
- 🧠 **Jian-Lu-Bu-Zou thinking OS / 见路不走思考系统**: fused from Ye Zinong + Ding Yuanying + Mao — don't copy experience, start from your own conditions, find the principal contradiction, act according to objective law, rely on yourself never on a savior / 融合叶子农+丁元英+毛泽东——不照搬经验,从自身条件出发,抓主要矛盾,按客观规律办事,靠自己不靠救主
- 🎬 Full pop-science video pipeline: script template → Feynman review → de-AI-ification → motion standards / 完整科普视频流水线:脚本模板→费曼审查→去 AI 味→动效标准
- 🌐 Awwwards-level web quality methodology (layered lighting / negative letter-spacing / glassmorphism / non-fade transitions) / Awwwards 级网页质量方法论(分层打光/负字距/玻璃拟态/非淡入转场)
- ✍️ De-AI copy rewriting (humanizer) / 去 AI 味文案改写(humanizer)
- 🔍 Frontend design anti-pattern detection (impeccable, 60 rules) / 前端设计反模式检测(impeccable,60 条规则)
- ⚡ GSAP motion reference (easing / timelines / performance) / GSAP 动效参考(缓动/时间线/性能)

---

## Directory structure / 目录结构

```
content-forge-kit/
├── README.md               ← this file / 本文件
├── skills/                 ← 6 skills, ready to use / 6 个即用 skill
│   ├── content-forge/      command center (main entry, install this first) / 指挥中心(主入口,先装这个)
│   ├── humanizer/          de-AI rewriting (mandatory step) / 去 AI 味改写(强制步骤)
│   ├── feynman-review/     zero-prerequisite review of pop-science content / 科普内容零基础审查
│   ├── impeccable/         frontend design anti-pattern detection (full scripts included) / 前端设计反模式检测(含完整脚本)
│   ├── mao-zedong-perspective/  dialectical-materialist thinking / 辩证唯物主义思考
│   ├── jianlu-buzou-perspective/  Jian-Lu-Bu-Zou thinking OS (Ye Zinong + Ding Yuanying + Mao) / 见路不走思考系统(叶子农+丁元英+毛泽东)
│   └── gsap-motion/        GSAP motion reference / GSAP 动效参考
└── content/
    ├── video-script-template.md   a script is mandatory before making any video / 做视频前必须先写脚本
    └── high-end-quality-guide.md    the complete quality methodology / 完整高端质感方法论
```

---

## Quick install (3 steps) / 快速安装(3 步)

### Step 1: Install the skills / 第一步:安装 skills
Copy the 6 folders in `skills/` into your agent's skills directory:

把 `skills/` 下的 6 个文件夹复制进你智能体的 skills 目录:

- **Reasonix**: `<Reasonix home>/skills/` (takes effect globally / 全局生效)
- **Claude Code**: `~/.claude/skills/`
- **Cursor**: `~/.cursor/skills/`
- **Other agents**: just read the `SKILL.md` in each folder directly / **其他智能体**:直接读各文件夹里的 `SKILL.md` 即可

### Step 2: Place the assets / 第二步:放置资产
Copy the 2 files in `content/` into your project directory (recommended under `content/`).

把 `content/` 下的 2 个文件复制进你的项目目录(建议放在 `content/` 下)。

### Step 3: Start using it / 第三步:开始使用
Tell your agent: / 告诉你的智能体:

```
Use the content-forge skill to create content. Read skills/content-forge/SKILL.md to start.
用 content-forge skill 创作内容,先读 skills/content-forge/SKILL.md。
Making a video → first write a script per content/video-script-template.md → pass Feynman review + humanizer → then do the animation
做视频→先按 content/video-script-template.md 写脚本→过费曼审查+humanizer→再做动效
Making a webpage → set the quality bar per content/high-end-quality-guide.md → impeccable review → GSAP motion
做网页→按 content/high-end-quality-guide.md 定质感标准→impeccable 审查→GSAP 动效
Making graphics/text → run humanizer directly to remove the AI flavor
做图文→直接跑 humanizer 去 AI 味
```

Or use the command: `/content-forge make a video about XXX` / `/content-forge make a landing page`

或用命令:`/content-forge make a video about XXX` / `/content-forge make a landing page`

---

## Core rules / 核心规则

1. **All standards are living defaults**: duration / word count / techniques / color palettes are default reference values — use whatever fits the project best; there are only two iron rules — zero errors in math/pop-science content, and all outward-facing content must pass humanizer / **所有标准都是活的默认值**:时长/字数/技法/配色都是参考值——怎么合适怎么用;只有两条铁律——数学/科普内容零错误,所有对外内容必须过 humanizer
2. **Dialectical-materialist thinking**: approach any problem in four steps — where is the contradiction / is the investigation sufficient / see both sides / seek truth from facts / **辩证唯物主义思考**:任何问题四步走——矛盾在哪/调查够不够/一分为二/实事求是
3. **Self-check before delivery**: review everything from the top, confirm it's correct, then deliver / **交付前自查**:从头过一遍,确认无误再交付

---

## Dependencies / 依赖

- `impeccable`'s detection script requires Node.js (it still works without it — the automatic checks are just skipped) / `impeccable` 的检测脚本需要 Node.js(没有也能用——只是自动检查会跳过)
- GSAP is a frontend library; load it via CDN when doing motion — no installation needed / GSAP 是前端库,做动效时用 CDN 加载即可——无需安装
- All other skills are pure Markdown, readable by any agent / 其余 skill 全是纯 Markdown,任何智能体都能读

---

## License / 许可

MIT · free to use, modify, and distribute (note: some assets are compiled from publicly available methodologies; see the notes inside each file for details) / MIT 协议,自由使用、修改、分发(注:部分资产整理自公开方法论,详见各文件内说明)

*Made by Tomato · stars welcome ⭐ / 由 Tomato 制作 · 欢迎 star ⭐*
