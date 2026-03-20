---
name: ai-native-product-weekly-L2
description: >
  Standalone production skill for the AI Native Product Weekly — Industry Intelligence
  (L2 Private) edition. Produces two output files per weekly cycle:
  L2 Leadership Edition (executives, BU leads, product leads, strategic decision-makers)
  and L2 Teams Edition (PMs, UX, Devs, BAs, ProdOps).
  Content filtered and reframed for target verticals: fintech, BNPL, e-commerce,
  parking & transit, accounting-as-a-service, B2C products, B2B products, EU/global lens.
  Published Monday after the week reviewed. Email-ready markdown output.
  No dependency on any other skill file. Runs as a complete standalone process.
version: 1.1
derived-from: SKILL v2.4 (main newsletter skill)
changelog:
  1.1 — edition split enforced (Top Stories Leadership only); link validation protocol
        added; quality-over-quantity rule for Teams role blocks; Signal is the only
        summary (no separate exec summary); Teams Worth Watching removed
  1.0 — initial standalone version derived from SKILL v2.4
---

# AI Native Product Weekly — Industry Intelligence (L2)
# Standalone Production Skill

---

## What This Produces

Two files, published together every Monday:

```
AI_for_Product_Issue_NN_L2_Leadership.md
AI_for_Product_Issue_NN_L2_Teams.md
```

**Leadership Edition** — 3–4 min read
Audience: executives, BU leads, product leads, strategic decision-makers
Format: scannable bullets, Product Relevance scores, strategic actions

**Teams Edition** — 7–9 min read
Audience: PMs, UX designers, developers, business analysts, ProdOps
Format: role-based blocks, process case study, tool/resource, detailed actions

**What both editions share:**
- This Week's Signal — identical 3 sentences, verbatim in both
- Top 3 Stories — same stories, different depth per edition
- Worth Watching — same 3 bullets

---

## Governing Principle

Quality is determined at classification, not at writing. A well-classified shortlist
produces a good issue almost automatically. A poorly classified one cannot be rescued
by good writing. Never skip or merge pipeline stages. Narrate every decision.

---

## Pipeline at a Glance

```
STAGE 1  Source Sweep        L2-specific sources + EU regulatory sweep.
                              15–25 raw candidates. Breadth first.
                              [Optional: Stack layer sweep in parallel]

STAGE 2  Classify            Maturity tier + domain tag + vertical score +
                              edition tag. Every item. No exceptions.

STAGE 3  Filter              7-step editorial filter including vendor announcement
                              check. Vertical filter. Coverage check.

STAGE 4  Assemble            Section assignments for both editions confirmed.
                              Source balance checked. No writing yet.

STAGE 5  Write               Leadership Edition first. Teams Edition second.
                              This Week's Signal written last, inserted verbatim.

STAGE 6  QA                  29-point checklist. Binary pass/fail.
                              QA log presented before files.

STAGE 7  Output              Two email-ready markdown files.
```

---

## Stepped Execution Protocol

Run in discrete steps. Pause after each step. Wait for confirmation before proceeding.
Never collapse stages — classification decisions must be reviewed before writing begins.

```
STEP 1  Present raw candidate list              → pause for review
STEP 2  Present classified shortlist +
        vertical scores + section map           → pause for review
STEP 3  Write Leadership Edition (Signal TBD)
STEP 4  Write Teams Edition (Signal TBD)
STEP 5  Write This Week's Signal
        Insert verbatim into both editions
STEP 6  QA log for both editions                → present log before files
STEP 7  Present both output files
```

**Step 1 output format:**
```
RAW CANDIDATES — L2 Issue #N · Week of [date] · Published Monday [date]
[N items found — EU sweep: [result summary]]

[Letter] | Headline | Source | Date | One-line excerpt
```

**Step 2 output format:**
```
CLASSIFIED SHORTLIST — [N items proceeding to assembly]

[Letter] | Headline | Tier | Domain | Verticals | Edition | Section

Vertical coverage:
  Fintech ✅/❌ · BNPL ✅/❌ · E-commerce ✅/❌ · Parking/Transit ✅/❌
  AaaS ✅/❌ · B2C ✅/❌ · B2B ✅/❌ · EU/Regulatory ✅/❌

Domain coverage:
  Architecture/tooling ✅/❌ · Agentic systems ✅/❌
  Independent practitioner ✅/❌ · Org & ways of working ✅/❌

Source balance: [vendor with most items] — [N] of [total]. Over 25%? [Y/N]
Convergence pairs: [describe or none]
Thin verticals: [list or none]
Items cut: [letter — reason]
```

**Step 6 QA log format:**
```
QA LOG — L2 Issue #N · [Leadership / Teams]

[ ] 1–29  [pass/fail + note per check]
Reading time: ~N min (target: Leadership 3–4 min · Teams 7–9 min)
Verbosity pass: [key cuts made]
Near-misses and editorial calls: [list]
```

---

## STAGE 1 — Source Sweep

**Goal:** 15–25 raw candidates. If under 10 after initial sweep, run additional
searches. Do not filter a thin list.

### L2-specific search query patterns

Five patterns. Use all five every issue. Never use broad topic searches — they
return vendor content and evergreen guides.

```
[practitioner name] + [publication venue] + [month year]
  → independent voices
  → "Ethan Mollick Insight Partners March 2026"
  → "Simon Willison simonwillison.net March 2026"

[specific product or feature] + [launch or release] + [month year]
  → primary announcements with vertical relevance
  → "MCP elicitation enterprise workflows March 2026"

[decision or tradeoff] + [year] + [production or enterprise]
  → architecture and tooling with vertical application
  → "agent observability regulated workflows 2026"
  → "RAG audit trail fintech 2026"

[vertical domain] + [AI deployment or adoption or governance] + [year]
  → vertical-specific use cases and signals
  → "fintech AI agent production deployment 2026"
  → "BNPL AI affordability assessment 2026"
  → "e-commerce AI personalisation architecture 2026"
  → "accounting automation AI reconciliation 2026"

[regulation] + [sector] + [enforcement or compliance or deadline] + [year]
  → regulatory and governance — run this for EU every issue
  → "EU AI Act high-risk fintech compliance 2026"
  → "DORA operational resilience AI 2026"
  → "GDPR AI features data processing EU 2026"
```

### Tier 1 — Sweep every issue across all categories

| Category | Sources |
|---|---|
| Model & capability | Anthropic Blog, OpenAI Blog, Google DeepMind, MIT Tech Review, Import AI, The Batch |
| Product practice | Lenny's Newsletter, SVPG/Marty Cagan, Reforge, Gibson Biddle, One Useful Thing (Ethan Mollick) |
| UX & design | Nielsen Norman Group, Figma Blog, Intercom Product Blog |
| Engineering & tooling | Simon Willison's Weblog, Latent Space, GitHub Changelog, LangChain Blog, Hugging Face |
| Industry analysis | a16z AI, Sequoia AI, Benedict Evans |
| EU regulatory | EUR-Lex AI Act tracker, IAPP, Morrison Foerster, Taylor Wessing, K&L Gates |
| Vertical — Fintech | Finextra, The Finanser, PYMNTS, Open Banking Expo, FinTech Futures |
| Vertical — E-commerce | Practical Ecommerce, Digital Commerce 360, Retail Gazette |
| Vertical — Enterprise/B2B | McKinsey AI insights, Deloitte AI reports, HBR product leadership |
| Vertical — AaaS | AccountingToday, Journal of Accountancy, Sage Blog |

### Tier 2 — Scan for breakthrough items

Named practitioner substacks and LinkedIn posts (product leads, AI engineers, CPOs
writing in personal capacity). Hacker News top AI threads (practitioner discussion
threads only — not link aggregation). Podcast transcripts only — never audio.

### EU regulatory sweep — mandatory every issue

Run as a dedicated pass, separate from the main sweep. If no material news this
week, state it explicitly in both file headers. Never skip silently.

```
Required every issue:
  "EU AI Act [month year] update"
  "EU AI Act [vertical] compliance [year]"
  "DORA [sector] [month year]"
  "Digital Omnibus AI Act [month year]"

Situational — run when relevant:
  "GDPR AI features [month year]"
  "EU Digital Fairness Act [month year]"
  "EUDI Wallet [month year]"
  "NIS2 AI systems [year]"
  "PSD3 open banking [month year]"
```

### Immediate cut criteria — apply during sweep

- No verifiable publication date, or >14 days ago and not explicitly evergreen
- Evergreen "how to use AI" guides, PM courses, certification marketing
- No traceable primary source — repost of a repost
- Org already used in previous issue (cap per org publisher, not per individual)
- Zero vertical relevance after scoring (see Stage 2)

### Raw candidate list format

```
[Letter] | Headline | Source name | URL | Date | One-line excerpt
```

### Link validation — mandatory before writing begins

Every URL must resolve to the specific article, report, or page being cited —
not to a domain homepage, section page, or search result.

**Validate each link before Stage 5 writing:**
```
1. RESOLVES?       Does the URL load without redirect to a homepage or 404?
                   Broken or redirected links → find the correct direct URL or
                   cite the source by name only with no link.

2. SPECIFIC?       Does the URL point to the exact article or document cited,
                   not to a publication homepage or section index?
                   Homepage links (e.g. journalofaccountancy.com without /article/)
                   → find the direct article URL or remove the hyperlink.

3. PAYWALLED?      Does the linked page require a subscription to read?
                   If yes → label [paywalled] inline next to the link.
                   Paywalled sources may still be cited; readers must know upfront.

4. ACCESSIBLE?     Is the content still live (not moved or deleted)?
                   If moved → update URL. If deleted → remove link, cite source only.
```

**On link uncertainty:** If the specific article URL cannot be confirmed, cite the
source name and publication date in plain text without a hyperlink rather than
linking to a homepage. A named source without a link is more honest than a link
that doesn't point to the cited content.

---

## STAGE 2 — Classify

Every item receives four tags before the filter is applied. Untagged items do not
proceed to the filter.

### Tag 1 — Maturity Tier

| Tier | Definition | What it requires |
|---|---|---|
| **Industrial Shift** | Structural change in how AI is built, bought, or governed at scale | 2+ independent sources confirming the pattern |
| **Research & Concepts** | Academic findings, frameworks, foundational thinking with practitioner application | Digestible by non-researchers; flag if purely theoretical |
| **Experiment / Early Signal** | Beta, pilots, preview access, unverified reports | Label `[Early Signal]`; no actions stated as certainties |
| **Validated Use Case** | Deployed in production with reported outcomes | Named org + specific metric — not a projection |
| **Proven Best Practice** | Replicated across multiple orgs with measurable results | Highest bar; only when convergence is genuine |

Maturity tier appears as a bracketed label in every published item header.
Reader-facing — tells them what kind of claim they are reading.

### Tag 2 — Domain Tag (assign one or two)

`Model & capability` · `AI tooling & DX` · `Architecture & infra` · `Agentic systems`
· `UX & human-AI interaction` · `Org & ways of working` · `Governance & risk`
· `Research & concepts`

Domain tag drives section placement within the Teams Edition:
`Architecture & infra` → Dev or BA block depending on angle
`Org & ways of working` → PM or ProdOps block
`Governance & risk` → Leadership top story or L2 regulatory item
`UX & human-AI interaction` → UX block

### Tag 3 — Vertical Score

Score each item against every vertical. Required before filter is applied.

```
  □ Fintech        payments, lending, fraud, KYC, open banking, neobanks, wealth tech
  □ BNPL           credit risk, regulation, checkout UX, consumer behaviour, defaults
  □ E-commerce     conversion, personalisation, search, logistics, pricing, marketplace
  □ Parking/Transit mobility, smart city, ticketing, dynamic pricing, fleet, MaaS
  □ AaaS           accounting automation, compliance, reconciliation, reporting, audit
  □ B2C products   consumer trust, onboarding, retention, personalisation at scale
  □ B2B products   sales intelligence, workflow integration, enterprise AI adoption
  □ EU/Global lens EU AI Act, GDPR intersections, European market dynamics,
                   regulatory divergence affecting product decisions

2+ verticals → HIGH PRIORITY for L2
1 vertical   → include if strong actionability
0 verticals  → cut from L2 entirely
```

### Tag 4 — Edition Tag

```
[LE]    Leadership Edition only — strategic, org-level, investment/governance
[TE]    Teams Edition only — role-specific practice, technical implementation
[BOTH]  Both editions — different depth and framing per edition
```

Assignment rule:
- Strategic, org, or investment implications → [LE] or [BOTH]
- Role-specific practice, tooling, technical depth → [TE] or [BOTH]
- Top Stories and Worth Watching → always [BOTH]
- This Week's Signal → always [BOTH]; written once, placed verbatim

---

## STAGE 3 — Filter

Apply all seven steps in sequence. Stop at first failure.

```
1. VERIFIED?          Primary source exists and is linked. Claims attributable.
                      Speculative → [Early Signal] or cut.

2. INDEPENDENT?       At least one non-vendor source confirms the claim.
                      Vendor-only data → flag [vendor data]; exclude from Top Stories.

3. VENDOR ANNOUNCE?   If primary or sole source is a vendor's own blog, press
                      release, or partner programme:
                      — Identify the independent industry signal within it.
                      — Find 1+ non-vendor source confirming that signal.
                      — No independent confirmation → downgrade to [vendor data] /
                        [Early Signal] or cut from Top Stories entirely.
                      — Vendor announcements may support an independently-sourced
                        story. They may never anchor a Top Story alone.

4. VERTICAL?          Scores at least 1 vertical (see Stage 2 Tag 3).
                      0 verticals → cut from L2.

5. ACTIONABLE?        Can a product professional in a target vertical do, decide,
                      or think differently this week because of this?
                      Leadership: strategic decision or governance implication.
                      Teams: role-specific workflow, tooling, or technique change.
                      Purely interesting → cut regardless of quality.

6. REFRAMEABLE?       Can this story be written with a vertical-specific implication
                      genuinely distinct from a general framing?
                      If L2 writing would be identical to a general edition → cut
                      or hold until the vertical angle is clearer.

7. SO WHAT?           Write: "This matters for [vertical] product teams because ___."
                      Cannot write it cleanly → item is not ready.
```

### Convergence test — run after all items are classified

Look for two independent items pointing at the same structural shift from different
angles — regulatory + practitioner, technical + organisational, EU + global.
Pairs produce stronger Top Stories than standalone items. Treat as a single
editorial unit with multiple sources.

### Coverage check — all required before proceeding to assembly

```
[ ] Minimum 3 distinct verticals with substantive items (not passing mentions)
[ ] At least 1 item: Architecture & infra or AI tooling & DX
[ ] At least 1 item: Agentic systems
[ ] At least 1 item: EU/Regulatory (or explicit "none this week" in file header)
[ ] At least 1 item: independent practitioner voice
[ ] At least 1 item: Org & ways of working or Governance & risk
[ ] Leadership Edition: at least 3 stories with strategic/org-level vertical implications
[ ] Teams Edition: at least 2 items per role block confirmed
```

Missing any → run additional targeted searches. Do not fill gaps with weak items.

---

## STAGE 4 — Section Assembly

**Goal:** Every item assigned to exactly one section in exactly one edition
(or explicitly mapped to both with distinct treatments). Source balance checked.
No writing until assembly is confirmed.

### Leadership Edition — section map

```
① THIS WEEK'S SIGNAL    3 sentences. Verbatim in both editions.
                        Written last (Stage 5). Placeholder during assembly.

② TOP 3 STORIES        3 stories. Hard cap. Scannable bullet format.
                        Vertically reframed — not general industry news + vertical tag.
                        Each story has 4 structured fields (see format below).

③ WORTH WATCHING        3 bullets. Vertically relevant signals only.
                        Same as Teams Edition. One line each.

④ RESOURCE OF THE WEEK  1 item — may be a regulatory guide, legal analysis,
                        or practitioner framework, not only tools.
                        Name · one-sentence vertical value · link.
```

**Leadership story format:**
```
### [Story headline] · [Maturity Tier]
[Source](URL) · [Source](URL) · Date

· [What happened — one sentence]
· [The vertical-specific strategic signal — one sentence]
· [The implication for org or investment in your sector — one sentence]

Product Relevance: N/10
Relevant for: [verticals / roles / functions]
Impact: [one sentence — what changes in your vertical if this is true]
Action: [one sentence — what to decide or initiate this week]
```

**Product Relevance score — rubric:**

Score is the sum of four criteria, each 0–2.5. Apply before writing. Score in
context of the L2 audience — a story relevant only to general product teams but
not to any of the target verticals scores lower than the same story with clear
vertical implications.

| Criterion | 0 | 1.25 | 2.5 |
|---|---|---|---|
| **Strategic impact** | Marginal or niche | Affects one function or team | Changes org-level decisions or investment |
| **Implementation readiness** | 2+ years away | 6–18 months | Available now or within 6 months |
| **Breadth of roles affected** | 1 role only | 2–3 roles | 4+ roles or cross-functional |
| **Time sensitivity** | Monitor only | Act within a quarter | Act this week or month |

8+ = Top Story material. Below 5 = Worth Watching or cut. Never round up.

### Teams Edition — section map

Teams Edition contains NO Top Stories — those live in the Leadership Edition only.
Both editions open with the same Signal. After that, content is completely distinct.

```
① THIS WEEK'S SIGNAL    Same 3 sentences as Leadership. Verbatim.

② ROLE-BASED BLOCKS     Up to 5 roles × up to 2 items each.
                        Skip any role where no high-signal item exists this week.
                        Skip any item slot where the content would be filler.
                        Minimum 2 distinct sources across the block set as a whole.
                        Items here do not appear in Leadership Edition.
                        All items vertically framed — not general + vertical tag.

    Product Managers    Regulated product spec quality, evals as compliance
                        documentation, adoption strategy in vertical contexts,
                        distribution moat analysis, build-vs-buy in regulated env
    UX & Design         Consumer trust in regulated AI, regulated UX patterns,
                        onboarding and consent design, modality shifts in
                        transactional contexts
    Business Analysts   Data governance and retrieval architecture for regulated
                        data, DORA compliance, audit trail design, cost modelling
                        for AI features in regulated workflows
    Developers          Regulated codebase governance, agentic workflow compliance,
                        model lifecycle as DORA dependency, architecture decisions
                        with audit trail implications, agent sandboxing
    ProdOps             Delivery operations in regulated orgs, specification quality
                        as compliance control, AI tooling rollout and adoption,
                        process instrumentation, sprint ops for regulated delivery

③ PROCESS & WAYS OF    1 item — only if a genuinely high-signal case study or
   WORKING             validated pattern exists this week. Skip if not.
                       Named org + specific outcome. No projections.
                       Preference for regulated-sector case study.
                       Cross-reference: "See Leadership Edition for strategic context."

④ TOOL OR RESOURCE     1 item — only if a genuinely useful resource exists.
                       May be a regulatory guide, legal analysis, compliance
                       framework, or practitioner tool. Skip if nothing high-signal.
                       What it is · best use case for your verticals ·
                       honest caveat. Access/pricing in first line.
```

**Quality over completeness rule:** An empty section is always better than a weak
item. If a role block, process section, or tool slot has no high-signal content this
week — omit it entirely. Do not write anything to fill the space. Readers will notice
filler faster than absence.

**ProdOps note:** Covers delivery operations and process — not PM strategy or
product discovery. If items are interchangeable with the PM block, one block is wrong.

### Assembly rules — all mandatory

**One edition, one section per item. No exceptions.**

**Content split between editions:**
- Leadership Edition: Signal + Top Stories + Worth Watching + Resource
- Teams Edition: Signal + Role Blocks + Process + Tool

**This Week's Signal is the only content that appears verbatim in both editions.**
Top Stories appear in Leadership Edition only.
Worth Watching appears in Leadership Edition only.
Role Blocks, Process, Tool appear in Teams Edition only.

**Role blocks do not repeat Top Story statistics verbatim.** Same story, different
vertical-specific angle and different action — acceptable. Same number or sentence
— cut and replace.

**Top Stories must be editorially independent.** Two Top Stories anchored by the
same single source → demote one to a role block.

**Source concentration:** Max 2 items from any single organisation's publications
across both editions combined. Applies to publishing org, not individual author.

**Process belongs in Teams Edition only.** Strategically significant case studies
get a one-line reference in Leadership Worth Watching — never the full item.

**Thin vertical:** If a vertical has only a passing mention this week, declare it
"light" in both file headers. Never manufacture coverage.

### Source balance check — before writing

Count sourced items per vendor across the full draft plan. If any single vendor's
own publications account for more than 25% of planned items:
1. Review each of that vendor's items — is this the best available source for the
   underlying signal, or does a better-sourced alternative exist?
2. Apply Filter step 3 to any vendor announcement used as a primary source.
3. Vendor blogs are secondary sources. Independent practitioners, academic papers,
   and reputable journalism are primary. Vendor content can support a story; it
   cannot anchor one without independent corroboration.

This check applies equally to all vendors: Anthropic, OpenAI, Google, Microsoft,
Meta, and any organisation with a publishing interest in the topics covered.

---

## STAGE 5 — Writing

**Goal:** Leadership Edition first. Teams Edition second. Signal written last,
inserted verbatim into both. One pass per section. No placeholder text in final output.

### This Week's Signal — written last, placed verbatim in both

**Exactly 3 sentences. Hard cap.**

```
Sentence 1 — THE MOMENT:
What specifically happened or crystallised this week that didn't exist last week?
Not a trend. A specific development or convergence creating a new fact on the ground.
Name it with vertical context — why does this week's development matter specifically
to regulated-sector product teams?

Sentence 2 — THE FORK:
What must a team or organisation now decide, do, or stop ignoring?
Frame as a binary: the path that acts on this signal vs. the path that doesn't —
and what diverges between them in your verticals specifically.

Sentence 3 — THE IMPLICATION:
One concrete consequence for regulated-sector teams, stated plainly.
What is now true, possible, or at risk that wasn't before?
No hedging. No "could" or "may."
```

**Three-sentence test:** Read the Signal to someone who hasn't seen the issue.
They should answer: (a) what changed this week, (b) what they need to decide,
(c) what happens if they don't. If any is unclear — rewrite that sentence.

**Vertical test:** Would this Signal make sense in a general (non-vertical) edition
without editing? If yes — it hasn't been reframed for L2. Rewrite.

**Swap test:** Could this Signal introduce a different week's issue without editing?
If yes — it lacks specificity. Rewrite.

**Anti-patterns:**
```
❌ Trend framing:            "AI governance is becoming increasingly important..."
❌ Observation without fork: "Three developments point at the same moment..."
❌ Hedged implication:       "This could affect how teams approach..."
❌ Vertical tag appended:    "[general signal]. For fintech teams, this is relevant."

✅ Moment + fork + implication, vertically specific:
"This week two independent signals confirmed that coding agents operating without
explicit documented constraints are making undocumented architecture decisions in
regulated production codebases — the same week the implementation infrastructure
to accelerate that deployment at enterprise scale was formalised.
Teams in fintech and AaaS that define agent governance frameworks this quarter
will have auditable, defensible systems before their next regulatory review;
teams that don't will retrofit governance under pressure when audit questions arrive.
August 2, 2026 is the EU AI Act hard stop for high-risk AI compliance — and the
acceleration of agent adoption is compressing the available preparation time."
```

### Reframe, don't repurpose

Every item in L2 must be genuinely rewritten — not summarised differently, but
interpreted differently. The editorial question changes.

```
GENERAL question: "What does this mean for product teams?"

L2 question:      "What does this mean for a senior PM or CPO at a European
                   fintech, BNPL provider, e-commerce platform, or AaaS firm?"
```

If writing the L2 version produces text that would be unchanged in a general edition
— the reframe has failed. Cut or hold until the vertical angle is clearer.

### Regulation is product strategy

In L2, EU AI Act obligations are not legal background. They are product and
engineering decisions. Frame them as such.

```
❌ "The EU AI Act requires providers of high-risk AI systems to conduct
   conformity assessments before market placement."

✅ "The conformity assessment requirement is a roadmap dependency.
   For credit decisioning teams: the technical documentation, accuracy
   thresholds, and human oversight design that conformity assessment
   requires are product and engineering deliverables — start now,
   the documentation cannot be completed in the final weeks."
```

**Provider vs. deployer is a product and architecture decision, not a legal one.**
The classification shifts when you: fine-tune a third-party model, post-process its
outputs, combine it with proprietary data that changes its behaviour for specific
use cases, or market the resulting system to other businesses. PMs making
build/integrate/configure decisions are simultaneously making regulatory
classification decisions.

### Open protocols vs. proprietary features — mandatory classification

Before writing any item involving a specific tool, API, file convention, or
integration pattern: classify it as one of three types and apply the framing rule.

```
TYPE 1 — Open protocol or standard
Applies across vendors and implementations. Cover fully. No vendor qualification.

Examples: MCP (Model Context Protocol — supported by Anthropic, OpenAI, Google,
Microsoft, Cursor, Windsurf, and 100+ third-party tools), OpenAPI, OAuth,
LangChain/LangGraph patterns, LlamaIndex, OTEL tracing, JSON Schema.

Framing: name the protocol. Do not attribute it to one vendor.
✅ "MCP elicitation enables agents to request structured input mid-task"
❌ "Claude Code's MCP elicitation" when describing the protocol itself

TYPE 2 — Widely-adopted practice, vendor-specific implementations
The concept is universal. The implementation varies by tool.
Cover the concept. Name the implementations for the configured stack.

Examples:
  Coding agent constraint files:
    Claude Code     → CLAUDE.md
    GitHub Copilot  → .github/copilot-instructions.md
    Cursor          → .cursorrules
    Windsurf        → .windsurfrules
    Amazon Q        → .amazonq/rules

  Eval / specification artefacts:
    Claude Code     → evals.md (as a practice convention)
    Any stack       → testable acceptance criteria in Jira, Linear, Confluence,
                       Definition of Ready checklists, BDD-style spec documents

  Agent observability:
    Datadog MCP Server, Langfuse, Galileo, Azure Monitor, Arize AI

  Structured HITL in agentic workflows:
    MCP elicitation (open protocol, multi-tool)
    LangGraph interrupt nodes
    Azure AI Studio human review steps
    GitHub Actions environment approvals
    OpenAI Assistants tool call confirmations

Framing: "[Concept] — implementations for your stack: [Tool A: X], [Tool B: Y]"
Never name only one vendor's implementation when the concept is widely adopted.

TYPE 3 — Proprietary feature, single vendor only
Only relevant to users of that specific tool and plan.
Route to Stack Updates block. Never appear in role blocks or editorial sections.

Examples: Claude Code /loop cron command, GitHub Copilot Enterprise policy settings,
Azure OpenAI PTU deployment configs, Jira Rovo agent triggers,
M365 Copilot Agent 365 governance console.
```

### Leadership Edition — writing rules

**Voice:** Boardroom peer with vertical expertise. No jargon. No cheerleading.
Every sentence answers: "what does this mean for how I govern my org or allocate
investment in this sector this week?"

**Signal in Leadership Edition:** The Signal is the only opening. No separate
executive summary. The Signal IS the summary — 3 sentences, scannable in 15 seconds,
specific enough to flag whether each story matters to this reader today.

**Bullet discipline:** Each story has exactly 3 bullets. Each bullet is one sentence.
No sub-bullets. The 4 structured fields appear after bullets — never embedded in them.

**Action at Leadership level:** A strategic decision, an investment signal, a
governance question to put on the next agenda, a vendor or partner conversation to
initiate, a regulatory calendar dependency to act on. Never a technical step —
those belong in Teams Edition.

**Resource of the Week:** Name, one-sentence vertical value, link. No usage
instructions. No caveats at Leadership level — just the signal value.

### Teams Edition — writing rules

**Voice:** Senior peer who has done the work in this sector. Direct. Specific.
Every sentence answers: "what do I do differently in my role in this vertical
this week?"

**Per-item format:**
```
HEADLINE · [Maturity Tier Label]
Source: [Name](URL) · [Name](URL) · Date

Body (2–4 sentences):
Specific facts. Named organisations. Statistics with source + scope qualifiers.
The vertical-specific insight — why this item survived the L2 filter.
Context the reader needs to evaluate the claim independently.

→ What this means for [vertical]: [2 sentences, vertical-specific implication]
→ Action: [one concrete action, achievable this week]
```

**Top Stories in Teams Edition:** Same stories as Leadership, but with technical
and practice-level vertical implications too granular for Leadership Edition.

**Role block items:** Exclusive to Teams Edition. Not in Leadership Edition.
Each item must name the vertical context explicitly in either the body or the action.

### Tone — both editions

**Anti-patterns — never use:**
- "The era of X is over"
- "The question has shifted from X to Y"
- "The bottleneck is no longer X — it's Y"
- "This week saw..." / "In a significant development..."
- Any sentence that could appear unedited in a vendor press release or legal summary

Vary analytical framing — rotate between: "what changed," "what this reveals,"
"what this enables," "what this requires," "what this risks."

### Workforce and skills framing — mandatory in both editions

Any item touching role changes, skill demand shifts, or task automation must follow
this framing without exception.

**The principle:** This briefing is read by the professionals whose roles are being
discussed. Framing that implies job loss creates anxiety without agency. Framing
that names growth targets creates motivation and direction.

**Skills under lower demand → automation targets:**
Frame as capacity freed for higher-value work.

```
❌ "Manual reconciliation skills are becoming less valuable"
✅ "Reconciliation is automating — that capacity moves to exception handling,
   client advisory, and the judgment calls that AI cannot make independently"
```

**Skills in higher demand → development focus:**
Specific, named, learnable. Not vague.

```
❌ "AaaS teams need to upskill or risk falling behind"
✅ "The skill expanding most in value for AaaS practitioners: designing the
   audit trail architecture that makes AI-generated entries verifiable —
   a direct extension of existing compliance work"
```

**For Leadership Edition actions:** Frame as capability to identify and develop
within the existing team. Default: the people to grow these skills are already in
the org.

```
❌ "Hire for systems thinkers who can maintain coherence at speed"
✅ "Identify who on your team already does this naturally — then give
   them the mandate and scope to develop it further"
```

**Anti-patterns — never use:**
- "X skill is becoming obsolete"
- "Teams will need fewer [role]s"
- "Professionals who don't adapt will be left behind"
- Any framing positioning the reader as the problem rather than the solution

When a source uses threatening framing: keep the fact, reframe for agency.

### Factual precision

Statistics carry source name and scope qualifier always.
"47% more efficient" → "47% more efficient on [benchmark name]."
Vendor-internal data labelled `[vendor data]` without exception.
Regulatory summaries carry: "as of [date]" + the legal disclaimer in the footer.
Preview/beta features: state availability constraints in body text, not label only.
Qualified claims retain their qualifiers through editing — "on some tasks" stays.

### Continuing stories — UPD format

When a story was covered in the last 2 issues and has material new developments:

```
**UPD: [Story name]** · [Maturity Tier] · [best current source link]
One sentence: what changed since last week, with vertical context.
→ Action: updated action only if the new development changes it.
```

Trigger: new data, reversal, GA after preview, regulatory ruling, enforcement action.
Do not use UPD for minor incremental updates — cut those entirely.
UPD items may appear in any section including Top Stories. Count toward section caps.

### Labelling conventions

```
[Early Signal]    Unverified, beta, preview, pilot — no action stated as certain
[vendor data]     Vendor-published metric, no independent corroboration
[paywalled]       Source requires subscription to read in full
```

### Action rules — every action must pass all five

1. **Audience-specific** — Leadership: strategic/governance. Teams: role-specific
   practice. Never mix. A technical step in a Leadership action belongs in Teams.

2. **Achievable this week** — within one week without special access or budget.
   State prerequisites explicitly; never hide them in "if" clauses.

3. **Not the news** — implies a decision, workflow change, or question now
   answerable. "Read the report" is not an action.

4. **Vertically explicit** — names the relevant sector context. Not "audit your
   AI features" — "for each AI feature processing EU customer credit or affordability
   data, answer three questions..."

5. **Stack-neutral** — a TYPE 3 proprietary feature belongs in Stack Updates, not
   role blocks. TYPE 2 concepts name all relevant stack implementations. TYPE 1 open
   protocols are named as protocols, not attributed to one vendor.

### Reading time — assess before output

```
Targets:
  Leadership Edition:   3–4 minutes
  Teams Edition:        7–9 minutes  (L2 adds ~1 min for regulatory content)
  Stack Updates:        30–60 seconds (when present)
```

**Verbosity pass — apply before every output:**
```
1. Cut any sentence that restates the headline
2. Cut any sentence that previews what you are about to say
3. Cut filler transitions: "Additionally," "Furthermore," "It's worth noting that"
4. Compress: two sentences making the same point → keep the sharper one
5. Leadership: each bullet must contain a distinct fact or implication
6. Teams "What this means" must add vertical-specific interpretation not in the body
7. Cut any sentence that would be identical in a general (non-L2) edition —
   if it doesn't carry vertical context, it hasn't been reframed
```

Estimate at 200 wpm. If over target: compress longest item per section by one
sentence. Repeat until within target. State reading time in file header.

---

## STAGE 6 — QA

Present QA log before each output file. Fix all failures before presenting.

### Shared checks — both editions

```
[ ] 1.  Edition split respected: Leadership has Signal + Top Stories + Worth Watching
        + Resource. Teams has Signal + Role Blocks + Process + Tool.
        The Signal is the ONLY content appearing verbatim in both.
        No Top Stories in Teams Edition. No Role Blocks in Leadership Edition.

[ ] 2.  Minimum 8 distinct sources across both editions combined

[ ] 3.  Maximum 2 items from any single organisation's publications

[ ] 4.  At least 1 independent practitioner voice
        (Named person, personal capacity — not vendor, aggregator, or PR output)

[ ] 5.  At least 1 item: Architecture & infra or AI tooling & DX

[ ] 6.  At least 1 item: Agentic systems

[ ] 7.  All statistics carry source name + scope qualifier

[ ] 8.  All beta/preview/limited-access features state availability in body text

[ ] 9.  Workforce framing: no obsolescence or job-loss language

[ ] 10. Source balance: no single vendor >25% of sourced items;
        if over — independent corroboration confirmed for each of that vendor's items
```

### Leadership Edition checks

```
[ ] 11. This Week's Signal: exactly 3 sentences; moment + fork + implication;
        passes vertical test (wouldn't make sense in general edition unchanged);
        passes swap test (couldn't introduce a different week unchanged);
        passes 3-sentence comprehension test

[ ] 12. All 3 stories have Product Relevance score with rubric applied;
        scores reflect vertical audience, not general product professional

[ ] 13. Scores consistent — no inflation; 8+ reserved for genuinely strategic
        vertical stories; below 5 = Worth Watching or cut

[ ] 14. All Leadership Actions are strategic/governance — no technical steps;
        all Actions name vertical context explicitly

[ ] 15. Reading time within target (3–4 min); verbosity pass completed
```

### Teams Edition checks

```
[ ] 16. This Week's Signal matches Leadership Edition verbatim

[ ] 17. Every present role block contains only high-signal items —
        no filler. Empty role blocks are absent, not padded.
        ProdOps block, if present, is distinct from PM block.

[ ] 18. No section present that contains weak, low-signal, or
        general-not-vertical content written only to fill the slot.

[ ] 19. All Teams Actions: role-specific; achievable this week; vertically explicit;
        stack-neutral (TYPE 1 = protocol named; TYPE 2 = all stack implementations
        listed; TYPE 3 = absent from role blocks)

[ ] 20. Process & Ways of Working: named org or cross-vertical pattern with
        evidence; no projections; cross-reference to Leadership Edition present

[ ] 21. Reading time within target (7–9 min); verbosity pass completed
```

### L2-specific checks — both editions

```
[ ] 21b. All links validated: each URL resolves to the specific article,
         not a homepage or section page. Paywalled sources labelled [paywalled].
         Unresolvable links removed — source cited by name only.

[ ] 22. Minimum 3 distinct verticals with substantive coverage
        (not passing mentions — each must have an item with a vertical-specific
        implication and a vertical-specific action)

[ ] 23. EU regulatory sweep completed; if nothing found this week, stated
        explicitly in both file headers — never silently omitted

[ ] 24. Legal disclaimer present in both footers

[ ] 25. Thin verticals declared in both file headers — none silently omitted
        Format: [Verticals: Fintech (full) · BNPL (full) · Parking (light)]

[ ] 26. No L2 item is general content with a vertical tag appended —
        each item must have genuine vertical reframing in body and action

[ ] 27. Provider/deployer classification implications flagged where relevant

[ ] 28. EU regulatory content framed as product/engineering decisions,
        not as legal summary
```

### Stack layer checks — when active

```
[ ] 29. Every stack item passes all four filter questions

[ ] 30. No stack item duplicates a main pipeline item

[ ] 31. All stack items carry role tag and timing statement

[ ] 32. If zero items: Stack Updates block absent entirely
```

---

## STAGE 7 — Output

### File naming

```
L2 Leadership:  AI_for_Product_Issue_NN_L2_Leadership.md
L2 Teams:       AI_for_Product_Issue_NN_L2_Teams.md
```

### File headers

**L2 Leadership:**
```
# AI Native Product Weekly — Leadership Edition · Industry Intelligence
### Issue #NN · L2 Private · Week of [date] · ~N min read
### Published Monday, [date]

[L2 — Verticals: Fintech (full) · BNPL (full) · E-commerce (full) · B2C (full) ·
B2B (full) · AaaS (full) · Parking & Transit (light) · EU/Regulatory (full)]
```

**L2 Teams:**
```
# AI Native Product Weekly — Teams Edition · Industry Intelligence
### Issue #NN · L2 Private · Week of [date] · ~N min read
### Published Monday, [date]

[L2 — Verticals: Fintech (full) · BNPL (full) · E-commerce (full) · B2C (full) ·
B2B (full) · AaaS (full) · Parking & Transit (light) · EU/Regulatory (full)]
```

### Standard footer — both editions, always include

```
*Sources link to primary publications. Regulatory information reflects publicly
available sources as of [date]. This is not legal advice. Verify compliance
obligations with your legal team.*

*Leadership / Teams Edition also available this week.*
*Next issue: Week of [date] · Published Monday [date]*
```

---

## Tech Stack Intelligence Layer [Optional]

Supplementary sweep for specific AI tools the team actively uses. Runs in parallel
with Stage 1. Produces a Stack Updates block in Teams Edition only — never Leadership
Edition. Items do not compete for main pipeline slots.

Activate only when a stack profile is configured. Never invent a generic stack.
For L2: stack items with vertical relevance get a one-line vertical tag appended.

### Default profile

```
STACK PROFILE: Product Team (default)

Collaboration:    Atlassian (Jira, Confluence, JPD) · Miro (AI, Intelligent Canvas)
Workplace:        Microsoft Teams (AI) · M365 Copilot (Chat, Pages, Agent 365)
Design:           Figma (Figma Make)
Engineering:      GitHub Copilot (Business/Enterprise) · Claude Code · Azure AI
```

Modify: "Add [tool] / Remove [tool] / Update [tool] to [plan/version]."
Changes apply from the current issue forward.

### Stack sweep queries

```
Atlassian:      "Jira AI update [month year]"  · "Rovo agents [month year]"
Miro:           "Miro AI features [month year]"
Teams/M365:     "M365 Copilot Wave [month year]" · "Agent 365 [month year]"
Figma:          "Figma Make AI update [month year]"
GitHub Copilot: "GitHub Copilot update [month year]"   ← primary: github.blog/changelog
Claude Code:    "Claude Code update [month year]"      ← primary: anthropic.com/news
Azure AI:       "Azure AI Studio [month year]" · "Azure AI Foundry [month year]"
```

### Stack item filter

```
1. AFFECTS CURRENT USAGE?  Material change to how the team uses this tool today?
                           No → cut.
2. DECISION OR ACTION?     Creates a decision or action this week?
                           No → cut.
3. ROLE RELEVANCE?         Tag: [Dev] [PM] [UX] [BA] [ProdOps] [Lead]
                           Untagged → cut.
4. TIMING?                 Live now / rolling out this month / future roadmap?
                           State explicitly — never leave timing vague.
```

### Stack item format

```
🔧 [TOOL] · [Maturity Tier] · [Role tag]
What changed. One sentence: operational implication for this team.
→ Action: one action, achievable this week.
[Vertical relevance: X · Y] (if applicable)
Source: [changelog or official blog link] · Date
```

### Stack Updates block

Teams Edition only. Appears after Worth Watching.
Only if at least one item survives the filter.
If nothing passes: omit the block entirely. No placeholder. No explanation.
Absence of the block means no material updates this week.

```
## 🔧 Stack Updates
[TOOL] · item
[TOOL] · item
```

### Boundary rule

```
MAIN PIPELINE:  TYPE 1 (open protocol) and TYPE 2 (widely-adopted concept).
                Structural insight applicable regardless of specific tool used.

STACK LAYER:    TYPE 3 — operational action relevant only to users of one
                specific tool and plan.
```

When a story has both structural and operational dimensions: structural angle in
main pipeline, stack note references it. Never duplicate the full item.
Main pipeline always wins when in doubt.

---

## Architecture & Agentic Coverage for Regulated Sectors

Run a dedicated search for each category every issue — most under-served in weeks
dominated by model launches or org news.

### Architecture & tooling — what to look for in L2 context

- RAG architecture for regulated data: audit trail design, version control of
  retrieval corpora, reproducibility of AI decisions on a specific date
- CAG vs standard RAG for stable compliance corpora under 1M tokens
- Agent orchestration in financial/regulated workflows: approval gates, HITL design,
  rollback mechanisms — across LangGraph, Azure AI, OpenAI, Anthropic stacks
- Model selection for regulated tasks: accuracy vs cost where errors have compliance
  or financial consequences
- Unified embedding architectures for mixed-format financial and compliance documents
- Observability and evals: Datadog, Langfuse, Galileo, Arize, Azure Monitor —
  what good looks like for systems affecting credit decisions or financial entries
- MCP integration patterns for structured approval gates in regulated agent workflows

### Agentic systems — what to look for in L2 context

- Multi-agent deployment in fintech/AaaS: coordination patterns, accountability
  chains, audit trail design
- Execute-and-verify as compliance control: test coverage before agent deployment
  in regulated codebases — applies regardless of coding agent used
- Structured HITL for regulated decision points: where human oversight is a regulatory
  requirement, not just a quality choice (MCP elicitation, LangGraph interrupts,
  Azure AI human review, GitHub Actions approvals)
- Agent governance in regulated environments: permissions, sandboxing, the
  "lethal trifecta" (write + execute + sensitive data access)
- Model lifecycle as DORA dependency: silent model endpoint redirects as potential
  conformity assessment triggers
- Coding agent constraint files across stacks: CLAUDE.md, copilot-instructions,
  .cursorrules — documented technology constraints as audit evidence

---

## EU Regulatory Reference

Current operative deadlines as of Skill v1.0 (March 2026).
Always verify against primary sources — this section is orientation, not legal advice.

```
EU AI Act:
  Aug 2, 2026    High-risk AI system obligations — OPERATIVE DEADLINE
                 (Annex III — see below for L2-relevant categories)
                 Digital Omnibus delay proposed; not enacted as of March 2026
                 Do not plan around a delay you don't have
  Aug 2, 2026    Article 50 transparency obligations for new AI systems
  Feb 2, 2027    Article 50 extension for systems already on market before Aug 2026
  Omnibus backstop if enacted: Dec 2, 2027 (Annex III) · Aug 2, 2028 (Annex I)

Annex III high-risk categories relevant to L2 verticals:
  → Credit scoring, loan origination, affordability assessment  [Fintech · BNPL]
  → Fraud detection and AML profiling                           [Fintech]
  → Employment screening, worker management                     [B2B]
  → Access to essential private services                        [B2C · Fintech]
  → Biometric identification                                    [KYC · Identity]

DORA (Digital Operational Resilience Act):
  Jan 17, 2025   In force for all EU financial entities
  Active supervisory scrutiny in 2026
  Register of Information: machine-readable format now expected
  AI model dependencies: must be documented as ICT service dependencies
  Silent model endpoint redirects = potential ICT change management event

Provider vs. deployer classification:
  DEPLOYER: uses a third-party AI system as-is — lighter obligations
  PROVIDER: built the AI system or had it built — full obligation set

  Classification shifts to PROVIDER if you:
  → Fine-tune the model on your data
  → Post-process outputs in ways that change behaviour for specific use cases
  → Combine with proprietary data to modify performance
  → Market the resulting system to other businesses

  Get legal review before assuming deployer status if any of the above apply.

Forthcoming:
  EUDI Wallet:          EU member states required to offer wallets late 2026
  EU Digital Fairness:  Expected H2 2026 — dark patterns, dynamic pricing,
                        recommender algorithms [BNPL · E-commerce]
  PSD3 / PSR:           Legislative process ongoing; expected 2026–2027
```

### High-priority vertical signals

```
Fintech:      Credit decisioning, KYC/AML, fraud detection, open banking APIs,
              explainability for lending decisions, EU AI Act Annex III obligations,
              DORA ICT Register, model lifecycle compliance

BNPL:         Affordability assessment AI, checkout UX friction, consumer default
              prediction, EU Consumer Credit Directive, trust signals,
              dark patterns legislation

E-commerce:   AI personalisation architecture, product search, dynamic pricing
              legality in EU, returns prediction, GDPR consent architecture,
              recommender regulation

Parking/      MaaS integration, smart ticketing, dynamic pricing models, fleet
Transit:      optimisation agents, accessibility obligations

AaaS:         Reconciliation automation, audit trail requirements for AI-generated
              entries, compliance reporting agents, multi-entity data management,
              DORA if serving financial clients, auditor access requirements

B2C:          Consumer trust design, onboarding conversion, AI feature disclosure
              obligations, GDPR personalisation consent, Article 50 labelling

B2B:          Enterprise AI adoption patterns, AI vendor procurement and governance,
              integration architecture, workflow agent governance, SLA and liability
              in AI contracts, EU AI Act deployer obligations

EU lens:      AI Act deadline status, Digital Omnibus progress, DORA supervision,
              GDPR + AI enforcement, Digital Fairness Act, EUDI Wallet timeline,
              NIS2 AI implications, CE marking for high-risk AI
```

---

## Source Credibility Tiers

**Primary (highest):** Academic papers (arXiv, ICML, AAAI, NeurIPS, CHI), named
practitioners writing in personal capacity, official product changelogs with version
specifics, EU institutional primary sources (EUR-Lex, Official Journal, Commission
communications), primary research reports with stated methodology and sample size.

**Secondary (good):** Reputable tech journalism (TechCrunch, The Verge, MIT Tech
Review, Ars Technica), independent legal analysis firms (K&L Gates, Morrison Foerster,
Taylor Wessing, Paul, Weiss), independent analyst firms, vendor blogs with external
corroboration from a non-vendor source.

**Tertiary (use with caution):** Aggregator newsletters, community discussions,
unattributed claims, vendor-only data, AI-generated summaries. Always label and
trace to primary before using.

**Do not use:** Sources promoting tools without disclosure, content mills,
SEO-optimised listicles, anything where a primary source cannot be traced.

**For regulatory content:** Always cite EU institutional primary sources (EUR-Lex,
Commission) alongside secondary legal analysis. Never cite legal firm analysis alone
as if it were the regulation itself. The analysis interprets; the regulation governs.

---

## Known Failure Modes

**Signal is fuzzy — observation without fork or implication**
Read the 3 sentences. If any of (a) what changed, (b) what to decide, (c) what
happens if they don't — is unclear, rewrite that sentence. The vertical test: if
it would be unchanged in a general edition, the L2 reframe has failed.

**Vendor announcement treated as independent industry signal**
A vendor's own press release is not independent confirmation. Find a non-vendor
source confirming the signal before anchoring a Top Story. Without it: [vendor data],
downgrade to supporting evidence, or cut from Top Stories.
Reference: Anthropic Partner Network in Issue #03 L2 — genuine signal sourced
primarily from one vendor.

**Top Stories duplicated in Teams Edition**
Top Stories belong exclusively to Leadership Edition. Teams Edition opens with the
Signal and proceeds directly to Role Blocks. A Teams Edition that includes Top Stories
is redundant for anyone reading both editions in the same channel.

**Teams Edition role block filled with weak items to meet section cap**
The quality-over-quantity rule supersedes the 2-items-per-block convention. A role
block with one strong item is better than a block with one strong item and one filler.
An absent block is better than a block with only weak content. Never write a role
block item whose sole purpose is to fill the slot.

**Links pointing to homepages instead of specific articles**
A link to journalofaccountancy.com is not a citation — it is a direction to a website.
Every link must resolve to the specific article, page, or document cited. Run the link
validation check at Stage 1 before writing begins. If the specific URL cannot be
confirmed: cite the source by name and date without a hyperlink.

**L2 item is general content with vertical tag appended**
"[General insight]. For fintech teams, this is also relevant." is the failure
pattern. Every L2 item must have its body and action written from the vertically-
specific editorial question. The reframe must produce different writing, not the
same writing with a vertical footnote.

**Proprietary feature in a role block action**
TYPE 3 features belong in Stack Updates only. Apply the 3-type classification
before writing every action. A Claude Code command, a GitHub Copilot Enterprise
policy setting, or an Azure-specific configuration in a role block is a bias failure.

**TYPE 2 concept written as if it has one implementation**
"Write an evals.md" with no acknowledgment that other stacks have equivalent
artefacts is the failure pattern. Name the concept. List the stack implementations.

**EU sweep skipped**
Mandatory every issue. If nothing found: state it explicitly in both file headers.
The absence of EU news is worth noting. Never silently omit.

**L2 thin vertical filled with weak items**
Declare "light" in file header. Transparency beats false completeness. An item
that passes the general filter but fails the "So what for [vertical]?" test is
a weak vertical item.

**Regulatory content framed as legal summary**
EU AI Act obligations are product and engineering decisions in L2. If writing reads
like a legal briefing — "the Act requires providers to..." — reframe to what this
means for roadmap, architecture, UX, or delivery.

**Provider/deployer classification assumed without review**
Flag when teams have fine-tuned, post-processed, or configured third-party models
in ways that may shift their classification. Never assume deployer status without
noting the review requirement.

**Model lifecycle treated as operational footnote**
Silent model endpoint redirects are potential DORA change management events and
EU AI Act conformity reassessment triggers in regulated systems. In L2, this class
of item belongs in the Dev block, not Worth Watching, when it affects regulated
workflows.

**Action is role-generic, not vertically explicit**
L2 actions must name the vertical. "Audit your AI features" is not a L2 action.
"For each AI feature processing EU customer credit or affordability data..." is.

**Leadership Edition reads like a Teams Edition with bullets**
Leadership Actions answer "what do I decide or govern?" not "what do I implement?"
Technical steps belong in Teams Edition.

**Product Relevance scores inflate over time**
Apply the rubric every issue. Reserve 8+ for genuinely strategic vertical stories.
Score 6 = good relevant story. Inflation destroys the score's signal value.

**ProdOps block defaults to PM block content**
ProdOps = delivery operations, process instrumentation, tooling rollout.
Not PM strategy or product discovery. If items are interchangeable — one block is wrong.

**Same story beat in 3+ sections**
Hard cap: 2 items from any single report across both editions combined.

**Pipeline stages collapsed**
Always pause after Step 2 before writing begins. Classification and vertical scoring
decisions must be reviewed before writing starts.

**Stack block present when empty**
If no items survive the filter: omit the block entirely. Its absence is the signal.

**Workforce framing uses anxiety instead of agency**
Obsolescence or "left behind" language → reframe as automation target or development
opportunity before output. See workforce framing rules in Stage 5.
