# interviewer-kit

[English](README.md) · [中文](README.zh-CN.md)

---

> **Interviewer-side interview kit · 面试官侧人岗匹配问题清单生成器**

## The problem · 痛点

Most business interviewers have had no structured interview training. With only a resume and a JD in hand, the questions that come out are "tell me about yourself," "why are you leaving," "what did you do on that project." Thirty minutes later, the decision rests on fluency and presence rather than evidence of delivery.

Run the same role past two interviewers and the conclusions rarely align — one weighs industry background, another weighs communication style — so the hiring decision falls back to gut feel. HRBPs absorb the cost: a fresh outline for every session, with no guarantee the business interviewer will follow it.

业务面试官多数没有接受过结构化面试训练。手里只有一份简历和一段岗位描述，能问出口的往往是"介绍一下你自己""为什么离职""这个项目你做了什么"。三十分钟过去，判断依据主要是表达是否流畅、气场是否合拍，而不是这个人能否在岗位上交付。

同一岗位换两位面试官，结论往往对不上：有人看行业背景，有人看沟通感觉，最终决策退回到"我觉得还行"。成本落在 HRBP 身上——每场面试重新写一份提纲，还不知道业务方会不会照着问。

## The approach · 解决方案

Two inputs, one deliverable. The JD defines what the role actually requires — hard requirements, preferred items, transferable skills. The resume locates the outcomes the candidate chose to emphasize. Questions come from the intersection of the two, not from a generic question bank.

Each card states the question, its design rationale, what a strong answer contains, what a red flag looks like, and how to follow up. The output is a single HTML file: edit any line in place, export a long image, send it to the interviewer.

两份输入，一份交付物。JD 用来确定岗位真正要求什么——硬条件、优先项、可迁移能力；简历用来定位候选人主动强调的成果。问题从两者的交叉点产生，不从通用题库里挑。

每张卡写明问题本身、设计依据、合格回答应包含什么、红旗信号长什么样、以及如何追问。产物是单文件 HTML：任何一行都能就地修改，导出长图后直接发给面试官。

```
JD 文本 / 简历文件           一次对话
      │                         │
      ▼                         ▼
┌──────────────┐          ┌──────────────┐
│ 核心要求提取   │          │ 标志性成果锚定  │
│ 哪些硬条件     │  ──►    │ 哪几个项目能   │
│ 哪些优先项     │          │ 证明这些条件   │
│ 哪些可迁移     │          │                │
└──────────────┘          └──────────────┘
      │                         │
      └─────────┬───────────────┘
                ▼
          问题卡 + 节奏表
                │
                ▼
         可编辑 HTML
                │
                ▼
         750px 长图导出
          （微信 / Slack / Lark 直接发）
```

Three input modes: JD plus resume (default); a role from the built-in library plus resume (skips JD extraction, for repeat hiring in the same function); resume only (generic profile, with fit explicitly marked as not role-anchored).

三种输入方式：JD 与简历（默认）；常用岗位库中的岗位与简历（跳过 JD 采集，适合同类岗位重复招聘）；仅简历（按通用画像出卡，匹配度明确标注"缺少岗位锚定"）。

## The value · 价值

| Value | 价值 |
|---|---|
| **Evidence-based** — every judgment traces to a specific line in the resume or a specific answer | **判断有依据** — 每条结论都能对应到简历或回答中的具体证据，不是印象分 |
| **Comparable** — one set of dimensions and anchors per role, so interviewer conclusions can be compared | **标准可对齐** — 同一岗位共用一套评估维度与问题锚点，多位面试官的结论可横向比较 |
| **Prepared once** — HRBPs input once and distribute, instead of rewriting per session | **准备只做一次** — HRBP 输入一次即可分发，不必逐场重写 |
| **Reusable** — cards accumulate as role assets for the next hire in the same function | **可持续复用** — 问题卡沉淀为岗位资产，下次招聘同类岗位直接调用 |

## Two moments · 两个使用场景

### Before the interview · 面试前准备

HRBP drops in the JD and resume, confirms the extracted profile once, and receives a complete guide: fit assessment, checkpoints, nine question cards, a 30-minute timing plan. Review it, rewrite what doesn't fit, add a follow-up, export the long image, post it to the interviewer group. The interviewer opens it ten minutes before the session and knows what to ask and what a passing answer sounds like.

HRBP 把岗位描述与简历一起提交，确认一次画像，即得到该岗位的完整清单：匹配度诊断、待考察点、九张问题卡、30 分钟节奏表。审阅一遍，改掉不适用的提问、补上需要的追问，导出长图发到面试官群。面试官在开始前十分钟打开，知道这 30 分钟要问什么、听到什么算过关。

### During the interview · 面试中提问

The interviewer follows the timing plan: open with a broad question and let the candidate finish, then check the answer against the card's anchors and red flags. Where the answer stays vague, follow the card's path — break down the number, ask for the timeline, ask for the failed case — instead of improvising. No dead air, and no interrogation spiral.

面试官按节奏表推进：先用开放问题让候选人讲完，再对照卡上的高分锚定与红旗信号判断回答落在哪一侧。回答含糊时，沿卡上的路径追问——拆开数字构成、要时间线、问失败案例——而不是临场想问题。既不冷场，也不会因为追问过密把候选人逼进应试状态。

---

## What it doesn't · 它不做什么

- ❌ **不做候选端** — 不是刷题工具、不是简历润色器
- ❌ **不做 AI 打分** — 不给候选人评级。预测人岗匹配需要具体证据，不是一个分数
- ❌ **不做 ATS / HR 平台** — 不追踪申请人、不存储 PII、不集成招聘流程
- ❌ **不替代合规审查** — 内置了禁止问题的护栏，但不是穷举，正式使用前请与你所在区域的法务或合规负责人确认

---

## Sample outputs · 样例产物

两份样例均为虚构。英文样例设定在**美国 DTC 场景**（B 轮可持续家居品牌、远程团队、真实美国简历规范、US 语境 HR 问题），不是"从中文翻译过来"的感觉。

| | Live Preview · 在线预览 | Source · 源码 | Scenario · 场景 |
|---|---|---|---|
| 🇨🇳 中文 | [在线打开](https://zeldazmz.github.io/interviewer-kit/examples/%E6%9D%8E%E6%98%8E-%E7%94%A8%E6%88%B7%E5%A2%9E%E9%95%BF%E7%BB%8F%E7%90%86-Interview-Guide.html) | [查看源码](examples/李明-用户增长经理-Interview-Guide.html) | TO B/G 业务增长类岗位 · 通用 JD |
| 🇺🇸 English | [Live demo](https://zeldazmz.github.io/interviewer-kit/examples/Alex-Johnson-Senior-Growth-Manager-Interview-Guide.html) | [Source](examples/Alex-Johnson-Senior-Growth-Manager-Interview-Guide.html) | Series B DTC sustainable home goods · US remote |

---

## How it works · 五步工作流

技能在一次对话中跑完。每步有明确停止条件——上一步输出不符合规范，不能进入下一步。

| Step | Input | Output |
|---|---|---|
| **1. Profile · 画像采集** | JD + resume file | 结构化画像 · 3 条 success factors |
| **2. Analyze · 分析** | 结构化画像 | 逐维匹配度 · 待考察点（带验证方式） · 一句话诊断 |
| **3. Design · 问题设计** | 分析结果 + success factors | 问题卡（业务面 7–10 张 + HR 面 3–4 段） · 节奏表 |
| **4. Self-check · 自检** | 完整问题清单 | 十项检查清单；不达标卡片必须重做 |
| **5. Pack · HTML 打包** | 所有前置输出 | 可编辑 HTML 文件，导出即用 |

自检不是装饰。实测中它抓到了真实失败——比如"跨部门影响力只出现在副维度，主维度里完全缺失"——并强制重新设计。

---

## Design principles · 核心设计原则

### 方法论层

- **三源制题源**：success factors 卡（4–5 张，测上限）· 情境前瞻卡（1–2 张，测未来适配）· 风险验证卡（1–2 张）。配额存在，但"为凑配额出题"被明确禁止
- **缺口题通道**：JD 列了一个"优先项"而简历没有，问题永远是"你怎么补上这个缺口"——永远不问"你做过吗"
- **教学卡结构**：主问题 → 主/副维度 → 设计原理 → 高分锚定 ↔ 红旗信号 → 追问路径（带 *标签 + 触发信号 + 停止条件*）
- **中性风险框架**：空档、短任期等风险先用中性框架验证（"我想先确认一下时间线再往下聊"），不是审判式追问

### 工程层

- 单文件 HTML，内联渲染引擎（html2canvas），无 CDN，断网可用
- 手机端 = 375px 单列阅读视图；导出 = 750px 桌面版式（有意为之，非 bug——1.75x scale 保证清晰度）
- 自适应 canvas scale（上限 16Kpx），长图分段渲染，PNG 超过 ~12 MB 自动降级 JPEG
- 导出失败弹 toast；不会悄悄生成白图然后"成功"
- 导出按钮 busy-lock，防止双击崩溃
- 宿主适配器设计（见 [`references/host-adapters.md`](references/host-adapters.md)）：只写能力层描述，不硬编码工具名

### 国际化

- 产物语言跟随**面试语言**，不跟随操作者语言
- 英文本地化（`references/en-localization.md`）：术语、句式、11 个追问标签变体
- US / EU / UK 合规红线：年龄、婚育、国籍、残疾、薪资历史——每项标注"可问 / 不可问"并附区域说明
- HR 面试四段**为英文路径重构**（不是翻译，是四段模板替换了中文版）
- UI 字符串集中在 `I18N` 对象；按钮、toast、确认框、导出文件名全部自动切换

---

## Use cases · 适用场景

**为以下场景设计**：B2B、SaaS、增长、运营、财务、职能支持等知识工作面试——任何"过往成果能预测未来表现"、"JD 技能能映射到简历行为"的岗位。

**以下场景效果较弱**：预测力弱的岗位（比如早期"潜力型"校招、高度创意型岗位的作品集）、或有强制面试格式的强监管行业（临床、制造质量等）。技能仍然会产出东西，但应该视为**草稿**，需要你再加工。

---

## Quick start · 快速上手

### Way A — Your agent supports skills

1. Clone or download this repo
2. Drop the `interviewer-kit/` folder into your agent's skills directory
3. Restart the agent, then say:
   > "帮我用 interviewer-kit 生成面试清单，附件是候选人简历"

### Way B — Your agent doesn't support skills

Paste the contents of `SKILL.md` + the 6 files under `references/` into a single conversation as context, then ask the same way. The skill runs entirely on markdown instructions — zero code execution.

### Host adapter notes

The skill is written in **capability descriptions** ("ask the user a structured question", "write out an HTML file"), not tool names. If your agent uses different tool identifiers, add a mapping line in [`references/host-adapters.md`](references/host-adapters.md).

---

## Compliance & data · 合规与数据处理

- No telemetry, no analytics. The skill never makes outbound network requests at runtime.
- The output is a single HTML file. Nothing is collected, stored, or transmitted after generation.
- The skill ships with guardrails for prohibited questions (marital status, age, salary history, disability, etc.). This is not exhaustive.
- When sharing outputs, consider replacing full names with role identifiers (e.g. "Cand-A · Growth Manager") if your org treats interview materials as sensitive.

---

## Contribute · 欢迎贡献

The methodology is open, the template is open. Contributions that actually move the needle:

- New function archetypes (clinical, manufacturing quality, etc.) with validated success factors and risk signals
- New follow-up tactic tags, verified in real interviews
- Better English localization — terminology, compliance notes, scenario parameters
- New host adapter mappings

Open an issue describing your use case, or send a PR directly.

---

## License · 许可证

MIT — see [`LICENSE`](LICENSE).

Third-party: `assets/template.html` inlines [html2canvas](https://github.com/niklasvh/html2canvas), also MIT. Thanks to the original author.
