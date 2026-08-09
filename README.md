# Content Forge Kit · 内容锻造全家桶(可移植套件)

> 用户(西红柿)的个人内容制作方法论全家桶,纯自用不商用。
> **用途**:把整套「网页 + 视频 + 图文」制作流程打包带走,换电脑/U盘即插即用。

---

## 这是什么

一个自包含的内容制作指挥中心,包含:

| 目录 | 内容 |
|---|---|
| `skills/` | 全套 skill(直接可被 agent 读取执行) |
| `content/` | 素材文件(脚本模板、质感方案) |
| 本 README | 安装 & 使用说明 |

---

## 在新电脑上怎么装(3 步)

### 第 1 步:放 skills
把这 6 个 skill 文件夹复制到新电脑 agent 的 skills 目录:

- **Reasonix**:复制到 `<Reasonix home>/skills/`(全局,所有工作区生效)
- **Claude Code**:复制到 `~/.claude/skills/`
- **Cursor**:复制到 `~/.cursor/skills/`
- 其他 agent:把 `skills/` 里每个文件夹的 `SKILL.md` 内容喂给它或放到对应 skills 目录

包含的 skill:
1. `content-forge` —— **指挥中心(主入口)**,先读这个
2. `humanizer` —— 去 AI 味改写(强制流程)
3. `feynman-review` —— 科普内容零基础审查
4. `impeccable` —— 前端设计反模式检测(含完整脚本)
5. `mao-zedong-perspective` —— 辩证唯物主义思考(默认思考模式)
6. `gsap-motion` —— GSAP 动效参考(缓动/时间线/性能)

### 第 2 步:放素材
把 `content/` 里的文件复制到新电脑的项目里(建议放到 `content/` 目录):

- `视频脚本提示词模板.md` —— 做视频前必须先出脚本
- `高端质感升级方案.md` —— 质感方法论完整方案

### 第 3步:告诉 agent 用起来

```
用 content-forge skill 来做内容。读 skills/content-forge/SKILL.md 开始。
做视频 → 先按 content/视频脚本提示词模板.md 出脚本 → 过费曼审查 + humanizer → 再做动画
做网页 → 按 content/高端质感升级方案.md 定质感 → impeccable 审查 → GSAP 动效
做图文 → 直接 humanizer 去 AI 味
```

---

## 核心规则(三句话记住)

1. **一切标准是活的**:时长/字数/技法/配色都是默认参考值,按项目最合适的来;只有两条铁律——数学零错误、对外内容必过 humanizer
2. **辩证唯物主义思考**:想任何问题按四步——矛盾在哪 / 调查够吗 / 一分为二 / 实事求是
3. **交付前自查**:从头过一遍,确认无误再交

---

## 依赖说明

- `impeccable` 的脚本需要 Node.js(检测 UI 反模式用);没有也能用,只是跳过检测
- GSAP 是前端库,做动效时用 CDN 引入即可,不需要安装
- 其他 skill 全是纯 Markdown,任何 agent 都能读

---

*版本:2026-08-10 · 由 Reasonix 打包 · 更新时重跑打包流程即可*
