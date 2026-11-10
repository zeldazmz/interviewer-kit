# 英文与海外本地化（en-localization.md）

本文件处理**产物语言**与**招聘市场合规差异**。只改语言和市场校准，不改方法框架——三源制题源、一主两副、双轴锚定、四段排序在英文场景完全沿用。

## 一、何时启用

满足任一条件即读本文件：

- 候选人为英文母语/非中文面试（简历或面试语言为英文）
- 岗位在海外（US / EU / UK / APAC 其他市场）
- JD 为英文且要求当地合规

## 二、语言判定规则（自动判定，不额外弹窗）

| 简历 / JD 语言 | 面试语言 | 操作者语言 | 产物语言 | 弹窗语言 |
|---|---|---|---|---|
| 英文 | 英文 | 中文 | **英文** | 中文 |
| 英文 | 英文 | 英文 | **英文** | 英文（标签见附录 A） |
| 中文 | 中文 | 中文 | 中文 | 中文 |
| 中文 | 英文 | 中文 | **英文**（问题按英文问） | 中文 |
| 中英混合 | 按岗位所在地判断 | — | 跟面试语言 | 跟操作者 |

**核心原则：产物语言跟随面试语言，不跟随操作者语言。** 中文 HR 面英文候选人时，弹窗保持中文（操作者读），HTML 清单全英文（面试官照着问）。

判定不确定时（如简历中英混排、岗位在跨国团队），在 Step 1 回复中一句话确认：「这份清单按英文出，还是中文？」——不要为此开弹窗。

## 三、术语与场景参数对照

情境题的专业度来自具体参数，英文参数用错会立刻显得外行。

### 业务增长类

| 中文提法 | 英文表达 | 常见误用 |
|---|---|---|
| 业绩口径（合同额 / 回款额） | bookings vs. revenue collected | contract amount |
| 转化漏斗 | conversion funnel / funnel conversion rate | pipeline conversion（特指销售管道阶段） |
| 客单价 | average order value (AOV) / average selling price (ASP) | customer unit price |
| 决策链 | buying committee / decision-making unit (DMU) | decision chain |
| 分润机制 | commission structure / revenue-share model | profit sharing（通常指公司利润分配） |
| 大促 | peak season / major promotional event | big promotion |
| 达标率 / 任务完成率 | quota attainment | completion rate |
| 增量 | incremental lift | increment |
| 归因 | attribution | — |
| 过程量 | leading indicators / activity metrics | process volume |

### 产品技术类

| 中文提法 | 英文表达 | 常见误用 |
|---|---|---|
| 职级 | job level / IC vs. manager track | rank |
| 带人规模 | team size / span of control | management range |
| 汇报关系 | reporting line | reporting relationship |
| 跨部门协作 | cross-functional collaboration | cross-department |
| 交付质量 | release quality / defect escape rate | delivery quality |
| 线上规模 | scale (DAU/MAU, QPS, tenants) | online scale |
| 技术取舍 | trade-offs | technology choice only |
| 复盘 | post-mortem / retrospective | replay |
| 技术债 | tech debt | technical debt（可，但行业内多写 tech debt） |

### 职能支持类与通用

| 中文提法 | 英文表达 | 常见误用 |
|---|---|---|
| 背调 | background check（含身份/学历/犯罪记录核验） / reference check（前雇主评价） | 两者混用 |
| 竞业限制 | non-compete agreement | competition restriction |
| 保密义务 | NDA / confidentiality obligation | secrecy duty |
| 离职证明 | certificate of employment / separation letter | resignation certificate |
| 流水 | pay stubs / compensation documentation | salary flow |
| 到岗时间 | notice period / availability | onboarding time |
| 试用期 | probation period (UK) / introductory period (US) | trial period |
| 出差覆盖 | travel requirements | business trip coverage |
| 职业规划 | career trajectory | career plan（偏生硬） |
| 社保公积金 | （无对应，见第五节薪资段） | social security（会被理解为社会福利） |

## 四、句式规范

### 行为题

- 字数：≤35 words（对应中文 ≤60 字）
- 开头用 **Walk me through / Take me through**，不用 **Tell me about a time when**——后者是 STAR 模板腔，英文候选人已被训练出背诵式回答，拿不到真实颗粒度

✅ `Your resume shows GMV grew 42% year over year. Walk me through how you designed that plan — which moves actually drove the result?`
❌ `Tell me about a time when you achieved a significant sales increase. What was the situation, task, action, and result?`

### 情境题

- 字数：60-90 words（对应中文 80-120 字）
- 必须含 ≥2 个具体参数 + 明确产出要求，结构与中文一致：场景参数 → 任务 → 约束 → 产出要求

✅ `Here's the situation: AOV is $300, your peak-season budget is cut in half, and fulfillment can only commit to next-day delivery. You have six weeks. What are the first three moves you'd make, and what would you expect each one to deliver?`

### 禁止清单（中英对应）

| 中文禁止 | 英文对应（同样禁止） |
|---|---|
| 哄人腔「里面一定有你最自豪的」 | "I'm sure there's something you're really proud of" |
| 水词「顺便好奇下」 | "Just curious…" |
| 万能收尾「你怎么看」 | "How do you see it?" |
| 陈词滥调 | "What's your greatest weakness?" / "Where do you see yourself in 5 years?" |
| 预设质疑 | "Why was that stint so short?" → 改为 "Walk me through that period." |

### 追问技巧标签（英文版，11 个）

| 中文标签 | 英文标签（页面显示） | 用途 | 触发信号 | 停止条件 |
|---|---|---|---|---|
| 亮点深挖 | Deep dive | 往深处问，看方法论成型度 | 讲到做得漂亮的地方 | 成功要素能拆成可复制的打法 |
| 情境模拟 | Scenario | 现场处理岗位真实场景 | 需要预测未来表现 | 给出具体打法与数字拆解 |
| SMART 校验 | Specificity | 目标/结果是否具体可衡量 | 说到目标、KPI 但没拆解 | 时间/数值/构成三项落地 |
| 对口径 | Metric check | 数字口径：范围/时间/含税/归属 | 抛出业绩数字或百分比 | 口径四要素说清 |
| 漏斗追问 | Funnel | 把过程拆环节追问转化 | 讲结果不讲过程 | 关键环节动作与转化都有数 |
| STAR 补问 | STAR gap | 补 Situation/Task/Action/Result | 故事缺背景/任务/动作 | 四要素齐、无跳跃 |
| 对抗验证 | Stress test | 给反例或质疑，看能否自圆其说 | 说法太顺、太完美 | 能接住质疑并给出解释 |
| 时间线验证 | Timeline | 按时间顺序重走，抓空档与矛盾 | 履历多段、时间含糊 | 各段起止与衔接对得上 |
| 假设法 | What if | 换条件看应变 | 需测迁移能力 | 给出可执行新打法 |
| 反例法 | Counter-example | 让他举失败案例，看归因 | 只讲成功、归因全在己 | 有真实失败且归因含自省 |
| 递进追问 | Drill down | 连问"然后呢/为什么" | 回答停在概括层 | 细节落到具体的人和事 |

### 高分锚定与红旗

- 单条 ≤12 words（对应中文 ≤18 字），确保页面单行可读
- 强度轴 / 真伪轴表述：`Strength: pattern is repeatable` / `Authenticity: numbers decompose`

## 五、HR 面四段：英文版（重构，不是翻译）

⚠️ **不要逐句翻译中文四段。** 中文段里的「是否全日制」「社保公积金」「学信网」在海外市场不存在或不可问，直译会直接踩线。以下为重构后的英文骨架。

### 1. Work Authorization & Credentials

- Are you authorized to work in [country]? Will you now or in the future require sponsorship?
- Degree and institution: verify through the background-check vendor after the interview.
- ⚠️ **US**：不得询问国籍、民族、母语、移民身份细节；可问工作授权与是否需要 sponsor。
- ⚠️ **US**：不要在面试中问毕业年份——可推断年龄；改由背调核验学历。
- ⚠️ **US**：不要问「是否全日制」——该分类在海外无对应含义。
- ⚠️ **EU/UK**：学历核验属个人数据，需告知用途与保存期限。

### 2. Compensation Expectations

- What are your compensation expectations for this role? What's the basis for that number?
- Structure: base / bonus / equity / benefits（无「社保公积金」对应项）。
- ⚠️ **US**：多个州与城市（如加州、纽约市、马萨诸塞州、科罗拉多州、华盛顿州等）已立法禁止询问当前或历史薪酬——只问期望，不问历史；以当地最新立法为准。
- ⚠️ **EU/UK**：薪资历史同样趋于禁止或受限；流水核验须候选人明示同意，并说明保留期限。

### 3. Role Alignment

沿用职能骨架，英文重写：

- **Sales trio**：Territory & market size / Product, ACV and sales motion (direct vs. channel) / Quota history — attainment for the last three years, and one best and one worst year in detail.
- **Product & engineering trio**：Scope and personal deliverables / Scale and quality (users, QPS, defect escape rate) / Stack depth and interfaces with product, QA and customers.
- **Functional trio (HR/Finance/Legal)**：Population and scale supported / Modules owned vs. supported, with representative outcomes / Performance ratings and one best and one worst year.
- **Generic four**：Understanding of the role / Most relevant experience / First 90 days / What you'd need from us.

### 4. Motivation & Availability

- Why this role, and why now? What's your notice period and earliest start date?
- Stability framing — 只问与工作安排相关的可问项：
  - ✅ `This role requires roughly 30% travel. Can you meet that expectation?`
  - ✅ `What are your plans over the next 2-3 years?`
  - ❌ `Are you planning to have children?` / `Are you married?` / `Do you have childcare arrangements?` / `How old are you?`

## 六、合规红线（US / EU / UK）

| 类别 | US（EEOC 及各州法） | EU（GDPR + 成员国法） | UK（Equality Act 2010） |
|---|---|---|---|
| 年龄 / 出生日期 | ❌ | ❌ | ❌ |
| 婚姻 / 怀孕 / 育儿安排 | ❌ | ❌ | ❌ |
| 种族 / 肤色 / 民族 / 国籍 | ❌（工作授权可问） | ❌ | ❌ |
| 宗教 / 信仰 | ❌ | ❌ | ❌ |
| 残障 / 病史 | ❌（仅可问能否完成岗位核心职能，且需提供便利） | ❌ | ❌ |
| 性取向 / 性别认同 | ❌ | ❌ | ❌ |
| 薪资历史 | ⚠️ 多州/市禁止 | ⚠️ 受限 | ⚠️ 受限 |
| 工会成员身份 | ❌ | ⚠️ 受限 | ❌ |
| 个人数据收集 | — | 需告知目的、范围、保存期限；候选人有权访问与删除 | 需符合 UK GDPR |
| 录音 / 转写 | ⚠️ 部分州要求双方同意（如加州） | 需告知并取得同意 | 需告知并取得同意 |
| 背景调查 | 需候选人书面授权 | 需单独告知并取得同意 | 需符合 DPA 2018 |

**免责声明（须在产物页脚保留）**：本清单为通用招聘合规提示，**不构成法律建议**。US 各州、EU 各成员国、UK 及 APAC 各地规定存在差异且持续变化，正式使用前须经当地法务或合规负责人复核。

## 七、市场差异校准（影响分析判断，不只是措辞）

英文场景下，中文框架里的部分硬判据会误伤，必须按市场校准：

| 判据 | 中国市场 | US / EU 市场 |
|---|---|---|
| 平均在职 <1.5 年 = 频繁跳槽 | 成立 | 偏短但不算高危；US tech 2-3 年一跳常见，<12 个月连续多段才升为红线 |
| 经历空档 | 需重点解释 | 常见（裁员周期、caregiving、sabbatical），**不默认视为风险**，只作为叙事完整性核验 |
| 学历「全日制 / 统招」 | 重要判据 | 无对应概念，删除该判据 |
| 晋升停滞 >3 年 | 停滞信号 | 仍适用，但 IC 长期深耕同一层级在欧美是正常路径，需结合 title track（IC vs. manager）判断 |
| 外包 / 驻场 | 职级口径差异 | 用 contract vs. FTE 区分，核验的是 scope 与 deliverable，不是「含金量折算」 |
| 竞业限制 | 常见 | 部分州（如加州）基本不可执行，不作为风险信号 |

原则：**判据的市场默认值不同，但方法论不变**——仍然是圈疑点、中性进入、深挖验证，不因为「海外空档很常见」就放弃核验，只是把它的风险等级下调。

## 八、产物与导出适配

- 文件命名：`<Candidate>-<Role>-Interview-Guide.html`；导出 `<Candidate>-<Role>-Business-Interview.png` / `-HR-Interview.png` / `-Interview-Guide.png`
- 导出形态：微信长图不适用海外场景，默认 PNG/PDF，用于邮件或上传 ATS；「导出全部」保留
- 版式：仍用 750px 画布；英文在同等字号下视觉更小，正文 16px、主问题 20px、说明 14px
- 字体栈：现有 `-apple-system, "PingFang SC"…` 对拉丁字符已适用，不加载外部字体
- 文案膨胀：同一内容英文通常比中文译文长 ±15%，导出高度会变化，分段逻辑按实际高度自适应即可，无需改代码
- 页脚须含第六节免责声明；水印条改为 `Internal Use Only · For Interview Evaluation`
- `<html lang>`：英文产物必须设 `lang="en"`，中文产物 `lang="zh-CN"`；模板内 I18N 对象按 `document.documentElement.lang` 自动切换工具条/运行时/确认框文案
- **界面字符串对照表**（模板内 `I18N.zh` / `I18N.en`，Agent 无需手改，只需保证 lang 属性正确）：

  | 键 | 中文 | 英文 |
  |---|---|---|
  | edit | 编辑 | Edit |
  | exportBiz | 导出·业务面 | Export: Business |
  | exportHr | 导出·HR面 | Export: HR |
  | exportAll | 导出·全部 | Export: All |
  | reset | 重置 | Reset |
  | generating | 生成中… | Exporting… |
  | exportReady | 导出组件未就绪，请刷新页面后重试 | Export tool not ready. Please refresh. |
  | exported | 已导出 {name}（{w}×{h}） | Exported {name} ({w}×{h}) |
  | exportFailed | 导出失败，请重试；若多次失败请用浏览器「打印 → 另存为 PDF」 | Export failed. Please retry, or use Print → Save as PDF. |
  | confirmReset | 重置将丢弃所有手动编辑，恢复为 AI 生成版本，确定吗？ | Reset will discard all manual edits and restore the AI-generated version. Continue? |
  | bizSuffix | 业务面问题清单 | Business-Interview-Guide |
  | hrSuffix | HR面问题清单 | HR-Interview-Guide |
  | allSuffix | 面试问题清单 | Interview-Guide |

## 九、自检（英文产物交付前）

- [ ] 无中式英语：`cross-department`→`cross-functional`、`decision chain`→`buying committee`、`salary flow`→`pay stubs`
- [ ] 无 STAR 模板腔（`Tell me about a time when`）与陈词滥调（`greatest weakness` / `5 years from now`）
- [ ] 行为题 ≤35 words、情境题 60-90 words 且 ≥2 个参数
- [ ] 追问标签用英文短标签（附录 B），单标签占比 ≤25%
- [ ] HR 面为重构版四段，非中文直译
- [ ] 无年龄/婚育/国籍/宗教/残障类问题；薪资只问期望不问历史
- [ ] 页脚含免责声明与内部使用水印
- [ ] `<html lang="en">`，工具条 / toast / 确认框 / 导出文件名均为英文
- [ ] 实际点击一次导出，文件名形如 `<Candidate>-Business-Interview-Guide.png`，无报错
- [ ] 文件名与导出形态符合第八节

## 附录 A：点选项英文标签

**Popup 1 — Role basics**

| 字段 | 英文标签 |
|---|---|
| job_direction | Revenue-facing (sales, marketing, BD, growth) / Product & engineering / Operations & delivery / Corporate functions (HR, finance, legal, admin) |
| job_level | Individual contributor / Senior IC / Staff or principal / People manager |
| exp_years | 1-3 yrs / 3-5 yrs / 5-8 yrs / 8+ yrs |
| education | No requirement / Bachelor's / Master's or above / Top-tier university preferred |

**Popup 2 — Capabilities**

| 字段 | 英文标签 |
|---|---|
| duty_focus | Outcome ownership / Deep functional expertise / Cross-functional influence / Team building & management |
| key_ability | Industry experience / Hard skills / Analytical ability / Communication & influence |
| industry_req | No preference / Same industry preferred / Adjacent industry OK / Specific industry required |
| sales_kpi | Quota attainment / Activity-driven / Margin & profit / Balanced scorecard |
| work_mode | Independent execution / Project-based collaboration / Resource coordination / Management & delegation |
| manage_span | ≤5 / 5-10 / 10-20 / 20+ |

**Popup 3 — Calibration**

| 字段 | 英文标签 |
|---|---|
| company_stage | Early stage / High growth / Mature & stable / Transformation |
| soft_priority | Drive & resilience / Learning agility / Collaboration / Structured thinking |
| hr_mode | Structured template / AI-generated set |
| hr_insight | 自由文本：Prior notes from recruiter calls (compensation expectations, notice period, reason for leaving, reference feedback). Do not include marital, family or health information. |

## 附录 B：一问一卡英文排版要点

- 维度标签：`Primary: outcome ownership · Secondary: metric definition, repeatability`
- 主问题标签：`Question`；追问标签：`Follow-ups`；设计原理：`Why this works`；高分/红旗：`Strong signals` / `Red flags`
- 时间表：`Opening / Strength deep-dive / Risk validation / Motivation & close`，时长写 `3 min` 不写 `3'`
