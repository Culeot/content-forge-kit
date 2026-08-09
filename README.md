# Content Forge Kit · 内容锻造全家桶

> 一套开箱即用的 **网页 + 视频 + 图文** 内容制作方法论全家桶,打包成 6 个可直接使用的 AI skills。
> ⭐ 如果对你有用,给个 star 支持一下!

---

## 这是什么

一个自包含的内容创作指挥中心。内含 6 个 skill + 2 份核心素材,任何 AI agent(Reasonix / Claude Code / Cursor 等)装上就能按这套方法论制作内容。

**核心亮点**:
- 🧠 辩证唯物主义思考框架(矛盾分析/实践认识/一分为二/实事求是)
- 🎬 科普视频完整流水线:脚本模板 → 费曼审查 → 去AI味 → 动效标准
- 🌐 Awwwards 级网页质感方法论(分层光/负字距/玻璃拟态/非淡出动效)
- ✍️ 文案去 AI 味改写(humanizer)
- 🔍 前端设计反模式检测(impeccable,60 条规则)
- ⚡ GSAP 动效参考(缓动/时间线/性能)

---

## 目录结构

```
content-forge-kit/
├── README.md               ← 本文件
├── skills/                 ← 6 个 skill,直接可用
│   ├── content-forge/      指挥中心(主入口,先装这个)
│   ├── humanizer/          去 AI 味改写(强制流程)
│   ├── feynman-review/     科普内容零基础审查
│   ├── impeccable/         前端设计反模式检测(含完整脚本)
│   ├── mao-zedong-perspective/  辩证唯物主义思考
│   └── gsap-motion/        GSAP 动效参考
└── content/
    ├── video-script-template.md   做视频前必须先出脚本
    └── high-end-quality-guide.md    质感方法论完整方案
```

---

## 快速安装(3 步)

### 第 1 步:装 skills
把 `skills/` 里的 6 个文件夹复制到你的 agent 的 skills 目录:

- **Reasonix**:`<Reasonix home>/skills/`(全局生效)
- **Claude Code**:`~/.claude/skills/`
- **Cursor**:`~/.cursor/skills/`
- **其他 agent**:直接读每个文件夹里的 `SKILL.md` 内容即可

### 第 2 步:放素材
把 `content/` 里的 2 个文件复制到你的项目目录(建议放 `content/` 下)。

### 第 3 步:开始用
告诉你的 agent:

```
用 content-forge skill 来做内容。读 skills/content-forge/SKILL.md 开始。
做视频 → 先按 content/video-script-template.md 出脚本 → 过费曼审查 + humanizer → 再做动画
做网页 → 按 content/high-end-quality-guide.md 定质感 → impeccable 审查 → GSAP 动效
做图文 → 直接 humanizer 去 AI 味
```

也可以用命令:`/content-forge 做一期XXX视频` / `/content-forge 做个落地页`

---

## 核心规则

1. **一切标准是活的**:时长/字数/技法/配色都是默认参考值,按项目最合适的来;只有两条铁律——数学/科普零错误、对外内容必过 humanizer
2. **辩证唯物主义思考**:想任何问题按四步——矛盾在哪 / 调查够吗 / 一分为二 / 实事求是
3. **交付前自查**:从头过一遍,确认无误再交

---

## 依赖

- `impeccable` 的检测脚本需要 Node.js(没有也能用,只是跳过自动检测)
- GSAP 是前端库,做动效时 CDN 引入即可,无需安装
- 其他 skill 全是纯 Markdown,任何 agent 都能读

---

## License

MIT · 自由使用、修改、分发(注:部分素材来源为公开方法论整理,详见各文件内说明)

*Made by 西红柿 · 欢迎 star ⭐*
