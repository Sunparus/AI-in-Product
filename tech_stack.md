# tech_stack.md — AI Native Product Weekly · L2 Industry Intelligence
## Tech Stack Intelligence Layer

---

## Purpose

A supplementary sweep targeting specific AI tools the team actively uses.
Runs in parallel with Stage 1 of the main pipeline — never replaces it.
Produces a **Stack Updates block** appended after the Resources section in the
Teams Edition only. Items do not compete for main pipeline slots.

**Activate only when a stack profile is configured.**
Never invent a generic stack. If no profile is set, this layer is inactive.

---

## Stack Profile

Edit this section to match your team's actual tooling.
Changes apply from the current issue forward.

```
STACK PROFILE: Product Team (default)

Collaboration:    Atlassian (Jira, Confluence, Jira Product Discovery)
                  Miro (AI, Intelligent Canvas)

Workplace:        Microsoft Teams (AI meeting intelligence)
                  M365 Copilot (Chat, Pages, Agent 365)

Design:           Figma (Figma Make — AI UI generation)

Engineering:      GitHub Copilot (Business / Enterprise)
                  Claude Code
                  Azure AI (Studio, Foundry, OpenAI Service)
```

To modify: "Add [tool]" / "Remove [tool]" / "Update [tool] to [plan/version]"

---

## Sweep Queries

Run these in parallel with the main Stage 1 sweep.
Query pattern: `[tool name] + [update or release or feature] + [month year]`

```
Atlassian:       "Jira AI update [month year]"
                 "Rovo agents Atlassian [month year]"

Miro:            "Miro AI features update [month year]"

Teams / M365:    "M365 Copilot Wave [month year]"
                 "Agent 365 Microsoft [month year]"

Figma:           "Figma Make AI update [month year]"

GitHub Copilot:  "GitHub Copilot update [month year]"
                 Primary source: github.blog/changelog

Claude Code:     "Claude Code update [month year]"
                 Primary source: anthropic.com/news

Azure AI:        "Azure AI Studio update [month year]"
                 "Azure AI Foundry [month year]"
```

---

## Item Filter

Higher actionability bar than the main pipeline — the reader already uses this tool.
All four must pass. Fail any one → cut the item.

```
1. AFFECTS CURRENT USAGE?
   Does this materially change how the team uses the tool today?
   If it's a minor UI tweak, a beta with no access, or future roadmap only → cut.

2. DECISION OR ACTION THIS WEEK?
   Does it create a decision or action the team can take this week?
   If it's awareness-only with no near-term implication → cut.

3. ROLE RELEVANCE?
   Which role does this primarily affect?
   Assign one tag: [Dev] [PM] [UX] [BA] [ProdOps] [Lead]
   If no clear primary role → cut.

4. TIMING EXPLICIT?
   Is the feature live now, rolling out this month, or on the roadmap?
   State it explicitly. Never leave timing vague.
```

---

## Item Format

```
🔧 [TOOL NAME] · [Maturity Tier] · [Role tag]

What changed — one sentence.
Operational implication for this team — one sentence.
→ Action: one action, achievable this week.
[Vertical relevance: Fintech · AaaS] (include only if relevant to L2 verticals)
Source: [direct changelog or official blog URL] · Date
```

---

## Stack Updates Block

**Teams Edition only.** Appears after the Resources section.
**Only when at least one item passes the filter.**
If nothing passes: omit the block entirely — no placeholder, no explanation.
Absence of the block means no material updates this week. That is the signal.

```markdown
## 🔧 Stack Updates

🔧 [TOOL] · [Tier] · [Role]
What changed. Operational implication.
→ Action: one action this week.
Source: [URL] · Date
```

---

## Boundary Rule

The main pipeline and the stack layer are distinct channels for distinct content.

```
MAIN PIPELINE   Structural insight — applies whether or not you use this tool.
                Covers TYPE 1 (open protocols) and TYPE 2 (widely-adopted concepts).
                Example: "MCP elicitation enables structured HITL in agent workflows"

STACK LAYER     Operational action — only relevant to teams on this specific tool.
                Covers TYPE 3 (proprietary features, single vendor).
                Example: "GitHub Copilot Enterprise: GPT-5.4 requires admin opt-in by March 31"
```

When a story has both dimensions: structural angle goes in the main pipeline,
stack note references it with a pointer. Never duplicate the full item in both.
**Main pipeline always wins when in doubt.**

For L2: stack items with clear vertical relevance (e.g. a Jira compliance workflow
feature relevant to AaaS teams, or an Azure AI update relevant to regulated fintech
deployments) get a one-line vertical tag appended to the item.

---

## QA Checks for This Layer

Run these after the main QA checklist, when the stack layer is active.

```
[ ] 1. Every stack item passes all four filter questions

[ ] 2. No stack item duplicates a main pipeline item
       (If it does — main pipeline wins, stack item is cut)

[ ] 3. All stack items carry a role tag and an explicit timing statement

[ ] 4. All stack links point to specific changelog entries or official release notes
       — not to tool homepages or marketing pages

[ ] 5. If zero items survive the filter: Stack Updates block is absent entirely
```

---

## Known Failure Modes

**Stack item duplicates a main pipeline story**
The stack layer is not a second chance for items that didn't make the main cut.
If an item is in the main pipeline, it cannot also appear in Stack Updates.
If it is in Stack Updates, it must not appear in the main pipeline.

**Timing left vague**
"Coming soon" and "rolling out" are not timing statements. Every item must say:
live now / rolling out in [month] / on the [Q] roadmap. If you cannot establish
timing from the source, cut the item.

**Stack block present when empty**
If no items pass the filter, the block must be absent — not present with a "nothing
this week" note. Absence is the signal. A present-but-empty block is noise.

**Generic stack invented when no profile is configured**
The stack layer is inactive without a configured profile. Do not sweep for tools
that aren't in the profile. Do not add tools because they seem relevant.
