---
name: content-forge
description: 内容锻造全家桶:网页/视频/图文制作的完整方法论指挥中心。触发词:做网页、做视频、做文案、内容创作、高端质感、视觉设计。内嵌辩证唯物主义思考、高端质感标准、视频脚本流程、费曼审查、humanizer 去AI味,并路由到 impeccable/GSAP 等子 skill。
---

# Content Forge · 内容锻造(全家桶指挥中心)

> 用户(西红柿)的个人创作方法论全家桶。**不商用,仅自用。**
> 收到任何「做网页 / 做视频 / 做文案」类任务时,先按本 skill 走流程。

---

## 总原则:一切标准都是活的,不是死的

**本 skill 里写的所有东西——时长、字数、技法、配色、流程、审查要求——都是「默认参考值」,不是「硬性规定」。每次动手前,根据这个项目最合适的实际情况选择,可以偏离默认、可以换方案。**

- 模板是起点,不是枷锁:脚本结构、文案字数、分镜数量都按实际内容调整
- 技法按需取用:不是每个项目都要全上所有技法,合适的才是好的
- 唯一不能动的两条底线(用户明确要求的):
  1. **数学/科普内容零错误**
  2. **对外发布的内容必须先过 humanizer 去 AI 味**
- 拿不准时:先用辩证唯物主义想清楚「这个项目最合适的做法是什么」,再动手

---

## 0. 思考模式(先想,再动手)

所有创作前,先用辩证唯物主义四步想清楚(不写出来,心里过):
1. **矛盾在哪?** —— 这个内容的核心矛盾/核心卖点是什么?(用户真正要解决什么问题)
2. **调查够吗?** —— 素材、数据、参考都够了吗?不够先查
3. **一分为二** —— 收益/代价,目标/约束
4. **实事求是** —— 按实际条件(平台/时长/受众)定方案

---

## 1. 任务路由(先判断类型)

| 任务类型 | 走哪套流程 | 产物 |
|---|---|---|
| **视频** | 见 §2(脚本 → 费曼 → humanizer → 动画) | `videos/<项目>/script.json` + 成品 |
| **网页/前端** | 见 §3(质感标准 → impeccable → GSAP) | 页面代码 |
| **图文/文案** | 见 §4(humanizer 去 AI 味) | 文案 |

---

## 2. 视频流程(科普短视频)

### 2.1 必须先出脚本
- 素材:`content/video-script-template.md`(完整模板,87 行)
- 流程:派子 agent 按模板生成 `script.json`(分镜表/文案四段式/动效/视觉/配音BGM/质量红线)→ **必须**过费曼审查 + humanizer → 用户确认 → 再做动画
- 结构:钩子(0-3s)→ 否定(3-6s)→ 核心拆解(6-32s,数学零错误红线)→ 升华(32-42s,比喻人生)
- 文案约束:550-700 字,每句 ≤25 字,术语首现必须一句话点破,口语化

### 2.2 质感标准(硬性)
- 素材:`content/high-end-quality-guide.md`(完整方案,159 行)
- 核心技法(每次通用):极深蓝灰非纯黑背景 + 3-5 层微弱光 + 渐隐网格 + 3% 噪点;标题负字距 -0.03em;白 55-65% 透明度代替纯灰;玻璃拟态;分层发光;GSAP `power3.out`/`expo.out` + stagger;禁止纯淡出转场(用缩放钻入/位移);Mono 刻度 + 渐隐分割线 + 取景框角
- ⚠️ **技法通用,视觉按主题定制**:配色/材质/字体每个项目单独定,禁止套同一皮肤(羽毛球=紫金,健康=清新,科技=深蓝…)

### 2.3 动效
- 路由到 GSAP skills:`hyperframes/skills/hyperframes-animation/adapters/`(gsap-easing-and-stagger / gsap-timeline-and-labels / gsap-transforms-and-perf)
- 红线:禁布局属性动画(left/fontSize),用 transform;缓动禁 linear

### 2.4 配音与发布
- edge-tts(Yunxi 阳光男声,+45% 语速);BGM 0.2-0.25 不盖配音;小红书发布走 `publish_video_xhs.py`

---

## 3. 网页/前端流程

### 3.1 先定视觉世界(不是先写码)
- 每个项目先定:主题配色 + 材质 + 字体 → 再上技法
- 风格锚定参考:linear.app / vercel.com / raycast.com,Awwwards SOTD 级
- 反例红线:no pure black, no harsh neon, no linear easing, no everything-at-once

### 3.2 质感技法(同上 §2.2,按需取用)
- 素材:`content/high-end-quality-guide.md`

### 3.3 设计审查
- 路由到 `impeccable` skill(前端设计反模式检测:AI 味 UI 特征、无障碍、对比度、排版)
- 完成后自查:分层光?负字距?非纯淡出?有主次节奏?

### 3.4 动效
- 路由到 GSAP skills(同上 §2.3)

---

## 4. 图文/文案流程

### 4.1 必须过 humanizer
- 路由到 `humanizer` skill(去 AI 味:套话/模板句/没个人痕迹 → 真人语气)

---

## 5. 质量红线(交付前自检,按总原则灵活执行)

1. **零错误红线**:数学/科普内容,数字、公式、结论必须精确(用户硬性要求)
2. **AI 味红线**:对外发布的内容不经过 humanizer 不许交付(用户硬性要求)
3. **质感**:按项目实际需求判断——需要高级感的项目必须达标(分层光/负字距/非淡出),简单项目不硬套
4. **审查**:视频脚本默认过费曼审查(零基础读者挑刺),简单内容可跳过
5. **自查红线**:交付前从头自查一遍,确认无误再交

---

## 6. 关联 skill 与素材(完整索引)

**子 skill(按需路由):**
- `humanizer`(全局):去 AI 味改写
- `feynman-review`(项目):科普内容零基础审查
- `impeccable`(全局):前端设计反模式检测
- `mao-zedong-perspective`(全局):辩证唯物主义思考
- GSAP 系列(hyperframes):gsap-easing-and-stagger / gsap-timeline-and-labels / gsap-transforms-and-perf / gsap-effects

**素材文件(global-workspace/content/):**
- `video-script-template.md` —— 视频脚本完整模板
- `high-end-quality-guide.md` —— 质感方法论完整方案

**外部库(已注册,不重装):**
- hyperframes 全套(GSAP/Three/Lottie/TypeGPU 等动画 skills)
- impeccable(前端设计审查)

---

## 7. 使用方式

- 简化指令:`/content-forge` 或 `run_skill({name: "content-forge", arguments: "要做什么"})`
- 也可以直接说「做一期视频」「做个落地页」「写篇文案」,本 skill 自动接管流程
- 派子 agent 执行具体环节时,把对应的素材文件路径一并给它
