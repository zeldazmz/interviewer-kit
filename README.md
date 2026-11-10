# interviewer-kit

> A skill that generates tailored interview guide PDFs from resumes and JDs — **for interviewers, not candidates**.<br>
> Built on a simple thesis: **interviewing is prediction, not audit**.

---

## Why most interviews are ineffective

Nearly every interview guide, AI tool, and coaching framework starts from the same assumption: "how do I catch a lie?" This produces a familiar outcome — candidates get good at being audited (STAR scripts, credential recitation), interviewers get good at being suspicious, and the conversation spends most of its time on low-signal verification.

What you end up with is a 30-minute chat that answers "did they do this?" but never answers "will they do *that* here?"

**interviewer-kit takes the opposite approach.** It anchors questions to the candidate's *actual signature work* — the projects they proudly cite, the numbers they choose to highlight — and asks questions that can *only* be answered by someone who did the thing, because the fake answers have different grammatical structure, different granularity, and different physics.

The output is a set of **teaching cards**: for each question, it tells you *what to ask, why it works, what strong answers sound like, what red flags sound like, and how to follow up without breaking the curiosity posture*. Using the cards is how the interviewer learns the method.

---

## What it is

| | |
|---|---|
| ✅ Tailored | Generated from *this specific resume + this specific JD*, not a generic question bank |
| ✅ Predictive | Questions probe future transfer, not past recitation |
| ✅ Educational | Every card carries the method — design principle, scoring anchors, follow-up tactics |
| ✅ Zero runtime deps | Single HTML file, inline rendering engine (html2canvas), no network calls at export time |
| ✅ Chinese + English | Two complete localizations, US/EU/UK compliance notes built into the English path |

## What it is *not*

- ❌ Not a candidate-side interview prep tool
- ❌ Not an AI "scoring" tool — it does not assign ratings to candidates
- ❌ Not an ATS or HR platform — it does not track applicants or store PII
- ❌ Not restricted to a single industry — designed for knowledge work across B2B, technology, operations, finance, and staff functions

---

## Case demo

All sample inputs and outputs are in [`examples/`](examples/). The candidate is fictional. Here is the compressed picture of what happens in one run:

### Input

<details><summary>JD (condensed, Northwind Supply)</summary>

> **Senior Growth Manager** · Northwind Supply · Series B sustainable home goods · Remote (US) · $140–170K base + 0.15% equity refresh + variable
>
> Own the end-to-end growth funnel; lead a team of 5–8 growth marketers; manage a $2.4M annual paid budget holding blended CAC flat at ~$38; partner with Product on site optimization. 7+ years in DTC / consumer growth. Data-driven, SQL proficient. **Preferred**: Shopify Plus, SMS marketing (Klaviyo), creator partnerships.

</details>

<details><summary>Resume (condensed, Alex Johnson)</summary>

> 7+ years building user acquisition and retention for consumer and e-commerce brands. Led growth at a DTC pet brand (PawPrints) to monthly revenue $0 → $2.4M, CAC held at $41. Built a Klaviyo referral program that hit 18% of new users at $19 CAC (lower than any paid channel). Previous role: EdTech scale-up, grew app from 0 → 320K users, CAC $39 → $26. Built team of 7 (1 departure in 18 months). Currently 14-month consulting gap — three early-stage DTC engagements. SQL, Looker, Shopify Pro, Klaviyo, TikTok Ads. *Two short tenures* (18 mo PawPrints, 2.5 yr EdTech).

</details>

### What the skill produces

**1. Fit summary** — not a scorecard, a diagnosis.

| Dimension | Verdict | Reasoning |
|---|---|---|
| Years, outcome ownership, CAC track record | ✅ Met | 7+ yrs, DTC scaled, held CAC flat while growing |
| Data stack (SQL, Looker), team building | ✅ Met | SQL + Looker, built team of 7, 1 departure in 18 mo |
| DTC business model | ✅ Met | PawPrints + LearnSphere are both DTC/consumer |
| Paid budget scope | ⚠️ Partial | Northwind is $2.4M annual; his largest was blended, need to confirm top-of-funnel ownership |
| Sustainable category transfer | ❌ Gap | Pet vs. home goods; purchase frequency and mindset are different |
| Shopify Plus (preferred JD) | ❌ Gap | Used Shopify Pro, not Plus |
| Overall | **Medium** | Strong outcomes + stability risk from two short tenures + 14-month gap |

**2. Six checkpoints** — signals to look for, with *how to verify*:

| Signal | Type | What to probe |
|---|---|---|
| 14-month consulting gap | Red line | Confirm engagements with deliverables; facts only, no personal questions |
| Two short tenures (18 mo + 2.5 yr) | Core | Exit logic; does the decision pattern repeat? |
| "$41 blended CAC" attribution | Core | What was included? Which channel drove it down from $45 target? |
| Team of 7 — 1 departure | Core | Timing relative to founder strategy shift; was anyone let go? |
| Budget scale match | General | His largest blended vs. Northwind's $2.4M annual — how would he adjust allocation? |
| Sustainable home-goods transfer | General | Ask how he'd learn the category in 60 days — never "have you sold home goods?" |

**3. Nine teaching cards** — here is one of them, verbatim:

```
Q1 · Primary: CAC control at scale · Secondary: metric integrity, budget ownership

Question
At PawPrints you held blended CAC flat at $41 — below your initial $45 target —
while scaling from $0 to $2.4M monthly revenue. Break down the $41: what's in it,
which specific channel or action drove it down from $45, and how did CAC trend
in months 10–18 when you were at scale?

Why this works
Anchored directly to the JD's core requirement: "scale while holding CAC stable".
Asking for composition and trend over time is the fastest way to distinguish a
trend from a one-month anomaly — real operators know the quarterly trajectory,
not just the headline number.

Strong signals
· Cites three channels and their individual CACs vs. blended
· Names a specific action (TikTok creative refresh, referral K-factor tuning)
· Describes month 10–18 trend honestly — not flat-line, with context
· Mentions cost rebound or saturation, even if CAC held

Red flags
· Totals only, no channel composition
· Blames "more efficient spend" — no specific lever
· Claims CAC was flat every month at scale (unrealistic)
· Cannot say what was included in the number

Follow-ups
[Calibrate]          Does the $41 include referral costs or media spend only?
[Time-series check]  Did CAC stay below $41 every month through month 18?
[Stress-test]        20% budget cut — which channels to protect, which to reallocate?
[Counterexample]     Did any channel not make it past 90 days? What killed it?
```

That's not a question bank — that's a **teaching card**. The interviewer sees the question, *why* it works, what a good answer sounds like, what to follow up with, and what to look for. Using the cards is how you learn the method.

**4. Agenda** — 30-minute business interview, 30-minute HR interview, with pacing notes.

**5. Editable HTML export** — click anything to edit, export as a long PNG or JPEG. Chinese products render at 750px (clear at 1.75x scale) with a responsive mobile view. English products follow the same layout, with UI strings switching automatically when `lang="en"`.

### Sample outputs (open them in a browser)

Both samples are fictional. The English sample is set in a **US DTC context** — Series B sustainable home-goods brand, remote team, real US resume conventions (education at the bottom, action-verb bullets, tool-stack specifics), and US-context HR questions (I-9 verification, no salary-history requests, equity refresh discussion).

| | Live Preview | Source | Scenario |
|---|---|---|---|
| 🇨🇳 Chinese | [在线打开](https://zeldazmz.github.io/interviewer-kit/%E6%9D%8E%E6%98%8E-%E7%94%A8%E6%88%B7%E5%A2%9E%E9%95%BF%E7%BB%8F%E7%90%86-Interview-Guide.html) | [查看源码](examples/李明-用户增长经理-Interview-Guide.html) | TO B/G 业务增长类岗位 · 通用 JD |
| 🇺🇸 English | [Live demo](https://zeldazmz.github.io/interviewer-kit/Alex-Johnson-Senior-Growth-Manager-Interview-Guide.html) | [Source](examples/Alex-Johnson-Senior-Growth-Manager-Interview-Guide.html) | Series B DTC sustainable home goods · US remote · Shopify Plus gap · two short tenures + 14-month consulting gap |

> **Note**: GitHub Pages deploys from the `examples/` directory, so the live URLs drop the `examples/` prefix. Pages take 1–2 minutes to deploy after a push — if you get a 404, wait and refresh.

---

## Workflow

The skill runs in a single conversation (the Agent calls it once). Five steps, all with explicit stopping criteria — the Agent cannot proceed until the prior step's output meets the spec.

| Step | Input | Output |
|---|---|---|
| 1. Profile collection | Resume file + JD (text) | Structured profile + 3 success factors |
| 2. Analysis | Structured profile | Fit summary + dimension verdicts + checkpoints |
| 3. Question design | Analysis + success factors | Teaching cards (business + HR) + agenda |
| 4. Self-check | Full question list | Ten-item checklist; failed cards must be re-written |
| 5. HTML packaging | All prior outputs | Editable HTML file, ready to export |

The self-check is not decorative. In testing it caught real failures — e.g., "cross-functional influence was only covered as a secondary dimension, missing from the main dimensions" — and forced re-design.

---

## Features

### Methodology layer

- **3-source question generation**: success factors (4–5 cards, test ceiling) · scenario forward-look (1–2 cards, test future fit) · risk verification (1–2 cards). Quota exists, but "designing questions just to fill quota" is explicitly prohibited.
- **Gap question channel**: if the JD lists a *preferred* item the resume lacks, the question is always "how would you close this gap?" — never "have you done it?"
- **Teaching-card structure**: main question → primary/secondary dimension → design principle → strong anchors ↔ red flags → follow-ups with *tag + trigger signal + stop condition*
- **Neutral risk framing**: gaps, short tenures, and other risks are verified with a neutral frame first ("I'd like to confirm the timeline before we go deeper"), not an interrogative one

### Engineering layer

- Single-file HTML, inline rendering engine, no CDN, offline-capable
- Mobile view = single-column 375px; export = 750px desktop layout (action is intentional, not a bug)
- Adaptive canvas scale (16Kpx cap), segmented rendering for tall pages, JPEG fallback when PNG exceeds ~12 MB
- Export failure surfaces a toast; no blank image silently "succeeds"
- Export button busy-lock prevents double-click crashes
- Host-adapter design (see [`references/host-adapters.md`](references/host-adapters.md)): capability-abstraction only; no hard-coded tool names

### Internationalization

- Language follows the interview language, not the operator language
- English localization (`references/en-localization.md`): terminology, sentence structure, 11 follow-up tag variants
- US / EU / UK compliance red lines: age, marital status, nationality, disability, salary history — each marked "ask / do not ask" with regional notes
- HR interview section is **restructured** for English, not translated (four-section template replaces the Chinese one)
- UI strings centralized in `I18N` object; buttons, toasts, confirm dialogs, export filenames all switch automatically

---

## Quick start

### Option A — your agent supports skills

1. Clone or download this repo
2. Drop the `interviewer-kit/` folder into your agent's skills directory
3. Restart the agent, then paste:
   > "帮我用 interviewer-kit 生成面试清单，附件是候选人简历"（or the English equivalent）

### Option B — your agent does not support skills

Paste the contents of `SKILL.md` + all six files under `references/` into a single conversation as context, then ask the same way. The skill runs entirely from markdown instructions — zero code execution required.

### Host adapter note

The skill is written in **capability terms** ("ask the user a structured question", "write the HTML file") rather than tool names. If your agent uses different tool identifiers, add a line to [`references/host-adapters.md`](references/host-adapters.md) mapping the capability to your host's tool.

---

## Scope & boundaries

**Designed for:** knowledge-work interviewing across B2B, SaaS, growth, operations, finance, and staff functions — any role where past outcome predicts future outcome and JD skill maps to resume behavior.

**Less well-suited for:** roles where prediction from past behavior is weak (e.g., early-career "potential" hires, highly creative roles where past work is heavily curated), or roles in heavily regulated sectors (clinical, manufacturing quality, etc.) that have mandatory interview formats. The skill will still produce something, but you should treat the output as a *draft* that you customize.

**Not intended for:** replacing legal or compliance review. The compliance notes are guidance only — review with your local counsel or compliance owner before using formally.

---

## Compliance & data handling

- No telemetry. No analytics. The skill does not make outbound network calls at runtime.
- Products are single HTML files. They do not collect, store, or transmit PII after generation.
- The skill includes internal guardrails for prohibited questions (marital status, age, salary history, disability, etc.). This is not exhaustive.
- When sharing the output with others, consider replacing the candidate's full name with a role identifier (e.g., "Cand-A · User Growth Manager") if your org treats interview materials as sensitive.

---

## Contributions welcome

The method is open, the templates are open. Things that are genuinely useful to contribute:

- New function prototypes (e.g., clinical, manufacturing quality) with verified success factors and risk signals
- Additional follow-up tactic tags, verified across real interviews
- Improvements to the English localization — terminology, compliance notes, scenario parameters
- New host-adapter mappings

Open an issue with a clear use case, or submit a PR.

---

## License

MIT — see [`LICENSE`](LICENSE).

Third-party: the HTML template in `assets/template.html` inlines [html2canvas](https://github.com/niklasvh/html2canvas), which is also MIT-licensed. Thanks to the authors.
