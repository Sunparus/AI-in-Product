# Research Focus Levels — AI Assistant Brief

> **Purpose**: This document instructs an AI assistant on how to scope, filter, and tailor research based on three distinct audience levels. When given a research task, identify which level(s) apply and calibrate depth, language, sources, and framing accordingly.

---

## Overview

| Level | Label | Audience | Primary Lens |
|-------|-------|----------|--------------|
| L1 | Strategic | Leaders, Executives, Architects | Organisational impact & direction |
| L2 | Operational | Product & Cross-Functional Teams | Workflows, roles & delivery |
| L3 | Individual | Solo Practitioners | Personal productivity & execution |

---

## L1 — Strategic Layer

### Who This Is For
- C-suite and senior leadership (CEO, CTO, CPO, CDO, COO)
- Enterprise architects and solution architects
- Procurement and vendor management teams
- Legal, compliance, and risk officers
- Industry analysts and strategic advisors
- Board-level stakeholders

### Research Persona
> *"I need to understand the landscape, evaluate options, make decisions, and justify them to the organisation. I think in terms of risk, ROI, competitive positioning, and organisational readiness."*

### Goals
- Understand market trends, industry movements, and emerging paradigms
- Evaluate build vs. buy vs. partner decisions
- Assess vendor landscapes and procurement implications
- Identify regulatory, legal, and compliance considerations
- Benchmark against industry peers and best practices
- Inform strategic roadmaps and transformation programs
- Communicate direction to boards, investors, and stakeholders

### Research Signals to Prioritise
- Analyst reports (Gartner, Forrester, IDC, McKinsey)
- Industry frameworks and maturity models
- Case studies from enterprise-scale organisations
- Regulatory guidance, legislation, and standards bodies
- M&A activity, funding rounds, and market consolidation
- Executive whitepapers and thought leadership
- Procurement frameworks and vendor evaluation criteria

### Language & Framing
- Use business and strategic vocabulary (ROI, TCO, risk appetite, competitive advantage)
- Frame findings around decisions, not implementations
- Lead with implications, not details
- Use executive summaries; put depth in appendices
- Avoid implementation-level jargon

---

## L2 — Operational Layer

### Who This Is For
- Product managers (PMs) and product owners
- Business analysts (BAs) and process designers
- UX/UI designers and researchers
- Software engineers and developers
- Product operations and delivery leads
- Cross-functional product teams throughout the PDLC (Product Development Lifecycle)

### Research Persona
> *"I need to understand how things work in practice — what tools, methods, and workflows help my team ship better products faster. I care about role-specific fit, integration with existing processes, and measurable team outcomes."*

### Goals
- Discover tools, platforms, and frameworks that improve team delivery
- Understand role-specific workflows and how they interconnect
- Map processes across the PDLC (discovery → design → build → test → release → iterate)
- Evaluate tools for fit within cross-functional team dynamics
- Improve product operations, team rituals, and collaboration patterns
- Surface use cases relevant to specific disciplines (e.g., dev tooling, UX research methods, BA documentation practices)
- Identify adoption patterns and change management approaches

### Research Signals to Prioritise
- Product and design community publications (Lenny's Newsletter, Mind the Product, UX Collective, InfoQ)
- Tool documentation, comparison sites, and integration guides
- Role-specific playbooks and methodology guides (e.g., BABOK, Shape Up, Dual-Track Agile)
- Case studies from product teams (not just enterprise, also scale-up and startup)
- Job descriptions and skills taxonomies (to understand role expectations)
- Community forums and practitioner discussions (Reddit, Slack communities, LinkedIn)
- Product ops frameworks and team topology resources

### Language & Framing
- Use role-appropriate terminology (sprint, backlog, discovery, PRD, wireframe, API, user story)
- Frame around team workflows, not individual tasks or boardroom strategy
- Include practical examples and real-world application
- Reference tooling ecosystems (e.g., Jira, Figma, Notion, Confluence, GitHub)
- Show how findings connect across roles in a team

---

## L3 — Individual Layer

### Who This Is For
- Knowledge workers optimising their personal workflow
- Freelancers, consultants, and solo operators
- Individual contributors across any discipline
- Early-career professionals building habits and systems
- Anyone seeking personal productivity gains regardless of role

### Research Persona
> *"I want to work smarter, not harder. Give me actionable techniques, tools, templates, and habits I can implement today. I care about what actually works for real people, not theoretical frameworks."*

### Goals
- Discover tools, apps, and extensions that save time and reduce friction
- Learn techniques, shortcuts, and workflows for personal efficiency
- Access templates, prompts, and ready-to-use resources
- Build sustainable systems for task management, focus, and output
- Stay current on productivity trends and personal effectiveness
- Find quick wins as well as longer-term habit and system improvements

### Research Signals to Prioritise
- Productivity blogs and newsletters (Tiago Forte, Ali Abdaal, Ness Labs, Superorganizers)
- YouTube tutorials, demos, and walkthroughs
- App directories and tool review sites (Product Hunt, AlternativeTo, G2)
- Reddit communities (r/productivity, r/notion, r/pkm, r/getdisciplined)
- Template libraries and prompt repositories
- Personal knowledge management (PKM) resources (Obsidian forums, Notion templates, Roam Research)
- Lifehack and GTD (Getting Things Done) adjacent content

### Language & Framing
- Use plain, conversational language — no jargon unless explaining it
- Be specific and actionable: name the tool, describe the step, show the template
- Lead with the "what" and "how", not the "why" at length
- Use bullet points, numbered steps, and examples liberally
- Acknowledge time investment vs. payoff trade-offs

---

## AI Assistant Instructions

### How to Apply This Framework

1. **Identify the level(s)** — Determine which level(s) the research request maps to. A single request may span multiple levels (e.g., "how are enterprises adopting AI in product teams" touches L1 + L2).

2. **Calibrate depth and sources** — Prioritise the source types listed for each level. Avoid mixing signal types inappropriately (e.g., don't cite Reddit threads in an L1 executive brief).

3. **Adapt tone and framing** — Match the language register of the level. L1 = strategic, L2 = operational, L3 = practical.

4. **Structure output accordingly**:
   - L1 → Executive summary first, implications, then supporting evidence
   - L2 → Workflow-first, role-specific sections, tool recommendations with context
   - L3 → Actionable steps, tool names, templates, quick wins up front

5. **When level is ambiguous** — Default to asking which level the research is for, or produce a layered response with clearly labelled sections per level.

6. **Cross-level research** — When a topic spans all three levels, structure output with three clearly separated sections (L1 / L2 / L3) so each audience can consume only what's relevant to them.

---

## Editing Guidelines by Audience Level

> **Purpose**: When editing or reviewing any document or post, apply the rules below based on the intended audience level. Editing is not just proofreading — it is calibrating the content to land correctly with the right reader.

---

### Editing for L1 — Strategic Audience

**Tone & Language**
- Every sentence must justify itself in terms of decisions, risk, or value. If it doesn't, cut it.
- No implementation detail in the body. If it must be included, move it to a footnote or appendix.
- Replace operational verbs (configure, implement, test) with strategic ones (evaluate, direct, invest, govern).
- Numbers and data must be present — but only if they change a decision. Vanity metrics out.
- Hedging is acceptable; vagueness is not. "Up to 40% cost reduction in pilot conditions" is fine. "Significant savings" is not.
- No em dashes. No casual connectors ("also," "plus," "on top of that").

**Structure & Formatting**
- Lead with the implication, not the background. The reader already knows the context.
- Maximum one level of sub-heading. Deep nesting signals content that hasn't been thought through.
- Use tables for comparisons, not prose lists.
- Executive summary at the top: three sentences maximum. What happened, what it means, what to do.
- Supporting evidence follows the summary — never precedes it.
- Call-to-action or decision prompt at the end of every section.

**What to Cut**
- Any sentence that explains how something works rather than what it means strategically.
- Background context the audience already knows.
- Tool names, feature names, and version numbers (unless the document is explicitly a vendor evaluation).
- Enthusiasm or advocacy language ("exciting," "powerful," "game-changing").
- Anything that reads like it belongs in a how-to guide.

**What to Keep**
- Competitive positioning signals — who is doing what, and what it costs to ignore it.
- Regulatory and compliance implications with dates and named obligations.
- Quantified outcomes from named organisations (with scope qualifiers).
- Clear decision fork: what changes if we act vs. if we don't.
- Source attribution for all claims — credibility matters to this audience.

---

### Editing for L2 — Operational Audience

**Tone & Language**
- Write as a senior peer who has done the work. Not a consultant, not a journalist.
- Role-specific language is expected and correct — use it precisely (sprint, acceptance criteria, design system, pipeline, backlog refinement).
- Be direct about trade-offs. This audience evaluates options daily; present the trade-off, not just the recommendation.
- Qualify tool recommendations: name the tool, state what it does, note the constraint or caveat.
- Active voice. Short sentences. One idea per sentence.

**Structure & Formatting**
- Role-based sections where content differs by function (PM / UX / Dev / BA / ProdOps).
- Lead each section with the workflow context, not the tool or concept.
- Use numbered steps for processes; bullet points for options or considerations.
- Actions at the end of every item — specific, achievable this week, role-explicit.
- Cross-references between roles where handoffs or dependencies exist.
- Reading time estimate is useful for longer documents — include it in the header.

**What to Cut**
- Strategic rationale the team doesn't need to re-litigate (they're already building, not deciding whether to).
- Generic "AI is changing everything" framing — it adds no signal.
- Tool recommendations with no vertical or workflow context.
- Items that apply to all roles equally — these belong in a cross-functional section, not a role block.
- Filler transitions and preview sentences ("In this section, we will explore...").

**What to Keep**
- Named tools with stated use cases and limitations.
- Process descriptions with enough specificity to act on.
- Real examples — named organisations, stated outcomes, scoped conditions.
- Vertical context: why this matters specifically for fintech, BNPL, e-commerce, AaaS, etc.
- Explicit connection to adjacent roles where relevant (e.g., "BAs should align this with the Dev team's constraint file before sprint planning").

---

### Editing for L3 — Individual Audience

**Tone & Language**
- Conversational but not casual. Friendly but not chatty.
- Write in second person ("you") throughout — it is personal and direct.
- Avoid jargon unless the audience clearly uses it. If in doubt, define it on first use.
- Shorter is always better. If a sentence can be cut without losing meaning, cut it.
- Energy and specificity over polish. A useful tip stated plainly beats an elegant paragraph that says nothing new.

**Structure & Formatting**
- Quick win or key takeaway at the very top — one sentence.
- Numbered steps for anything procedural. Bullet points for lists of options or ideas.
- Screenshots, examples, or templates referenced inline — not buried at the end.
- Headers should be action-oriented ("How to set this up in 10 minutes") not descriptive ("Overview of the feature").
- Bold the most important phrase in each section — scannable at a glance.

**What to Cut**
- Organisational or team-level context (this audience is acting alone).
- Strategic rationale — they want the how, not the why at length.
- Caveats that don't change the action ("results may vary" without specifics is noise).
- Any sentence that starts with "It's important to note that..." — it never is.
- More than one tool recommendation per use case unless comparison is the point.

**What to Keep**
- The exact name of the tool, template, prompt, or technique.
- Time investment estimate — L3 readers weigh effort vs. payoff constantly.
- A single, clear action at the end of every section.
- Honest caveats that actually affect the decision (free vs. paid, platform limitation, learning curve).
- Links to the specific resource, not to a homepage.

---

### Quick Reference — Editing Decisions by Level

| Decision point | L1 Strategic | L2 Operational | L3 Individual |
|---|---|---|---|
| Lead with | Implication / decision | Workflow context | Quick win / key action |
| Cut first | Implementation detail | Generic framing | Strategic rationale |
| Tone | Boardroom peer | Senior practitioner | Knowledgeable friend |
| Data use | Decision-changing only | Scoped, with caveats | Effort vs. payoff |
| Tool names | Avoid unless evaluating | Name with context | Name specifically |
| Call to action | Strategic / governance | Role-specific, this week | Personal, today |
| Length bias | Shorter | Right-sized per role | As short as possible |

---

*Last updated: March 2026*
