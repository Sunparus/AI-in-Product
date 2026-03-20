# evals.md — AI Native Product Weekly · L2 Industry Intelligence
## Evaluation criteria for pipeline output quality assessment

---

## Purpose

This file defines the success criteria, failure modes, and evaluation dimensions
for assessing the quality of L2 newsletter output produced by the standalone L2
production skill. It serves as both a pre-sprint specification and a post-output
review instrument.

Use before writing: to set the quality bar.
Use after output: to assess whether the bar was met.

---

## Output specification

Two files per weekly cycle. Both must pass all criteria before publication.

```
AI_for_Product_Issue_NN_L2_Leadership.md   Target: 3–4 min read
AI_for_Product_Issue_NN_L2_Teams.md        Target: 7–9 min read
```

---

## Evaluation dimensions

Seven dimensions. Each has testable criteria and a pass/fail threshold.
A single dimension failure = the output requires revision before use.

---

### DIMENSION 1 — Vertical Relevance

**The core L2 test.** Every item must earn its place through genuine vertical
applicability — not general AI news with a vertical tag appended.

**Pass criteria:**
- Every Top Story has a vertical-specific implication stated in the body
  and a vertical-specific action. Not "this matters for product teams — and
  for fintech teams especially." A genuinely different implication.
- Every role block item names the vertical context in either the body or action
- Minimum 3 verticals covered substantively across both editions
- Thin verticals declared in file header — none silently omitted

**Failure indicators:**
- "For fintech teams, this is also relevant" appended to general content
- Actions that would be identical in a general edition
- EU/Regulatory section left empty without declaration in file header
- A vertical appearing only in the file header label but not in any item body

**Test:** Take any item. Remove the vertical context from the body and action.
If the remaining text would fit unchanged in a general product newsletter — the
vertical reframe has failed.

---

### DIMENSION 2 — This Week's Signal Quality

**The interpretive test.** The Signal is the most important editorial element.
It must be specific, actionable, and vertically grounded.

**Pass criteria — all three sentences must pass their individual test:**

Sentence 1 (THE MOMENT):
- Names a specific development this week — not a trend or pattern
- Would not apply to a different week without editing
- Contains vertical context (why this matters to regulated-sector teams)

Sentence 2 (THE FORK):
- Frames a binary path — act vs. don't act, with diverging outcomes named
- The divergence is specific, not generic ("things will be harder" fails)
- Applies to the target audience — a CPO at a fintech, not "product teams"

Sentence 3 (THE IMPLICATION):
- States a concrete consequence — not hedged with "could" or "may"
- Is now true or at risk, not eventually possible
- Carries regulatory, competitive, or operational weight for the verticals

**Failure indicators:**
- Signal reads as a summary of what's inside the issue
- Any sentence could be reused in a different week's issue unchanged
- No binary fork — only an observation
- Implication is hedged or generic

**Test (3-sentence comprehension test):** Read the Signal to someone who hasn't
seen the issue. Ask three questions: (a) What changed this week? (b) What do you
need to decide? (c) What happens if you don't? All three must be answerable from
the Signal alone.

---

### DIMENSION 3 — Source Independence and Balance

**The credibility test.** Output must be trustworthy to a sceptical reader
who is aware of vendor publishing interests.

**Pass criteria:**
- No single vendor's own publications > 25% of total sourced items
- Top Stories anchored by independent sources (practitioner, journalist,
  academic, or industry research) — vendor announcements as support only
- At least 1 item per issue sourced from an independent practitioner
  writing in personal capacity
- All vendor-only data labelled `[vendor data]`
- EU regulatory items sourced from EU institutional primary sources
  (EUR-Lex, Commission) alongside legal analysis firms

**Failure indicators:**
- A Top Story whose primary and sole source is a vendor blog
- 3+ items in the same edition all sourced from the same organisation
- Statistics from vendor announcements reproduced without qualification
- Legal analysis cited as if it were the regulation itself

**Test:** Remove the vendor-published items. Does the core editorial argument
of each Top Story still hold with the remaining sources? If not — the story is
dependent on vendor data, not independently sourced.

---

### DIMENSION 4 — Action Quality

**The usefulness test.** Actions are the primary value delivery mechanism.
A reader who acts on one action per issue and finds it useful will return.

**Pass criteria for every action:**
- Audience-specific: Leadership actions are strategic/governance; Teams actions
  are role-specific and practice-level; never mixed
- Achievable within one week without special access, budget, or vendor lock-in
- Vertically explicit: names the sector or workflow context specifically
- Stack-neutral: TYPE 1 open protocols named as protocols; TYPE 2 concepts list
  all configured-stack implementations; TYPE 3 proprietary features absent from
  editorial sections
- Does not restate the news — implies a decision, change, or new capability
- Prerequisites stated explicitly — never hidden in "if" clauses

**Failure indicators:**
- "Check out the new feature at [link]"
- An action that names only one vendor's tool when the concept is widely adopted
- Leadership action that is a technical implementation step
- Action that requires the reader to use a specific vendor's product not in
  the configured stack

**Test:** For each action: (a) Is it clear who does it? (b) Can they do it this
week with what they have? (c) Does it produce a different outcome than doing nothing?
All three must be yes.

---

### DIMENSION 5 — Regulatory Framing

**The L2-specific credibility test.** Regulatory content must be framed as product
and engineering decisions — not legal summaries. Readers are product professionals,
not lawyers.

**Pass criteria:**
- EU AI Act obligations stated as roadmap dependencies, architecture decisions,
  or UX requirements — not as legal text restatement
- Provider/deployer classification raised where relevant to build-vs-buy or
  fine-tuning decisions
- EU regulatory sweep completed and result noted in file header
- Legal disclaimer present in both footers
- Regulatory information attributed to primary EU institutional sources, not only
  to legal firm analysis

**Failure indicators:**
- "The EU AI Act requires providers to..." without translating to product decision
- August 2026 deadline mentioned without specifying which systems are in scope
- Provider/deployer classification ignored when fine-tuning or model adaptation
  is discussed
- Regulatory sweep skipped and file header silent about it

**Test:** Take any regulatory item. Rewrite it as a legal briefing paragraph.
If the original item reads like the legal briefing — it hasn't been translated
into product decision terms. Revise until the original clearly answers
"what do I build, decide, or configure because of this?"

---

### DIMENSION 6 — Workforce and Skills Framing

**The reader trust test.** Readers are the professionals whose roles are discussed.
Framing that implies job loss or obsolescence reduces trust and utility.

**Pass criteria:**
- No language implying job loss, obsolescence, or professional inadequacy
- Skills under lower demand framed as automation targets — capacity freed
  for higher-value work
- Skills in higher demand framed as specific, named, learnable development areas
- External sources using threatening framing reframed editorially before publication
- Leadership actions frame capability development as identifying and growing
  existing talent — not filling gaps through hiring

**Failure indicators:**
- "X skill is becoming obsolete"
- "Teams will need fewer [role]s"
- "Professionals who don't adapt will be left behind"
- Hiring criteria from sources reproduced verbatim without reframing

**Test:** Read every sentence that mentions a role, skill, or task that AI is
changing. Ask: does this sentence give the reader a growth direction, or does it
create anxiety without agency? Reframe any that do the latter.

---

### DIMENSION 7 — Editorial Independence Between Editions

**The duplication test.** Leadership and Teams editions must be distinct outputs,
not reformatted versions of the same content.

**Pass criteria:**
- This Week's Signal: identical in both editions (verbatim — this is correct)
- Top Stories: same stories, genuinely different treatment — Leadership is
  strategic/scannable; Teams is practice-depth with body + What this means + Action
- Role block items: exclusive to Teams Edition, not present in Leadership Edition
- Process & Ways of Working: Teams Edition only; Leadership Edition has at most
  a one-line Worth Watching reference
- Leadership Actions answer "what do I decide or govern?" — Teams Actions answer
  "what do I do in my role this week?"

**Failure indicators:**
- Leadership Edition with technical implementation steps in Actions
- Teams Edition with strategic-only content in role blocks
- Process & Ways of Working appearing in full in both editions
- Role block items that are role-generic rather than role-specific

**Test (editorial independence test):** Read only the Leadership Edition.
Then read only the Teams Edition. A practitioner reading only the Teams Edition
should feel they have everything they need for their role. An executive reading
only the Leadership Edition should feel the same. Neither should feel they need
the other edition to act on the content.

---

## Minimum pass thresholds

All seven dimensions must pass for the output to be considered publication-ready.

| Dimension | Hard fail condition |
|---|---|
| 1 — Vertical Relevance | Any item with zero vertical-specific framing in body and action |
| 2 — Signal Quality | Any sentence failing its individual sentence test |
| 3 — Source Independence | Any Top Story anchored solely by vendor publication |
| 4 — Action Quality | Any action that is a single vendor's proprietary step in an editorial section |
| 5 — Regulatory Framing | Any regulatory item framed as legal summary without product translation |
| 6 — Workforce Framing | Any sentence implying job loss or professional obsolescence |
| 7 — Editorial Independence | Leadership Edition containing technical implementation steps |

---

## QA checklist cross-reference

The 32-point QA checklist in the production skill (Stage 6) is the per-item
verification layer. This evals.md is the holistic quality assessment — applied
after the QA checklist passes, to evaluate the issue as a whole.

Both must pass before output is presented.

---

## Revision triggers

An output that fails any dimension is returned to the relevant stage:

| Dimension failure | Return to |
|---|---|
| Vertical Relevance | Stage 3 (Filter) — item may need to be cut or reframed from scratch |
| Signal Quality | Stage 5 (Writing) — rewrite Signal only |
| Source Independence | Stage 3 (Filter) — find independent corroboration or cut from Top Stories |
| Action Quality | Stage 5 (Writing) — rewrite actions only |
| Regulatory Framing | Stage 5 (Writing) — reframe regulatory items |
| Workforce Framing | Stage 5 (Writing) — reframe affected sentences |
| Editorial Independence | Stage 4 (Assembly) — reassign items to correct edition |

---

*This evals.md is a living document. Update it when a new failure mode is observed
in a live pipeline run. Every entry in the Known Failure Modes section of the
production skill should have a corresponding test in this file.*
