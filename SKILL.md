---
name: strategic-thinking-mindset
description: Applies corporate strategic thinking and mindset to a business situation — first asking for whatever context is missing (business, objective, time horizon, scope), then applying the right framework, distinguishing whether the request is strategic (long-term) or tactical (short-term). Covers environment frameworks (VUCA, BANI, PESTEL, scenario planning), competitive and portfolio analysis (SWOT, Porter's Five Forces, VRIO, BCG, GE-McKinsey), business model and growth (Business Model Canvas, Ansoff, Blue Ocean, Jobs to be Done), organization and goals (McKinsey 7S, SMART, OKR, Balanced Scorecard), decision-making and change (Cynefin, Six Thinking Hats, Kotter), and financial fundamentals / strategic narrative. Returns a structured report with prioritized recommendations. Use when the user says "strategy", "SWOT", "PESTEL", "strategic plan", "competitive analysis", "business model", "Business Model Canvas", "McKinsey 7S", "OKR", "BCG matrix", or when they need to expand, invest, or decide something complex.
---

# Strategic Thinking and Mindset

Strategic-consulting skill: turns a business situation into a structured
analysis using the right framework — not all of them at once.

## Boundary with branding skills

If the request is purely about brand identity/positioning (naming,
manifesto, brand architecture), say so explicitly and suggest
`brand-strategy` or `brand-positioning` instead of forcing a SWOT/PESTEL
onto a branding problem.

## 1. Hybrid flow: ask before analyzing

Before applying any framework, ask whatever is missing from this list (don't
repeat what the user already gave in their message; max 4-5 questions,
asked once):

1. **Business context** — industry, size, current situation (already
   operating, an idea, in crisis?).
2. **Objective / problem to solve** — what decision needs to be made or what
   question needs to be answered.
3. **Time horizon** — short-term (< 1 year → tactical) vs. long-term
   (expansion, investment, transformation → strategic). This answer decides
   the explicit "this is strategic" / "this is tactical" label that must
   appear in the output.
4. **Scope** — internal (organization, processes, people), external (market,
   competition, macro environment), or both.
5. *(Optional, only if relevant)* constraints — budget, hard deadline,
   stakeholders to convince.

Never mix strategic and tactical without saying so explicitly in the
response.

## 2. Framework decision tree

Don't apply more than 2-3 frameworks per analysis unless the user
explicitly asks for "a complete analysis." If the situation is ambiguous,
use SWOT as the default entry point and offer to expand.

| User situation | Framework(s) | Reference |
|---|---|---|
| Fast, unpredictable changes in the environment | VUCA | `references/environment-frameworks.md` |
| Internal dynamics / existential challenges of the new world of work | BANI | `references/environment-frameworks.md` |
| Internal/external risk factors, general starting point | SWOT | `references/swot-pestel.md` |
| Macro environment (political, economic, social, technological, environmental, legal) | PESTEL | `references/swot-pestel.md` |
| Competitive structure of an industry/market | Porter's Five Forces | `references/porter-canvas.md` |
| Designing or validating the business model | Business Model Canvas | `references/porter-canvas.md` |
| Expansion into new markets or growth (current vs. new product/market) | Ansoff Matrix | `references/porter-canvas.md` |
| Internal organizational design (structure, systems, culture) | McKinsey 7S | `references/mckinsey-7s.md` |
| Internal analysis of competitive advantage (resources, activities, competitive posture) | Porter's generic strategies, value chain, VRIO | `references/competitive-strategy.md` |
| Portfolio of several businesses/products: where to invest, hold, or divest | BCG Matrix / GE-McKinsey | `references/portfolio-matrices.md` |
| Saturated industry, need for new market space or rethinking where to innovate | Blue Ocean, McKinsey's Three Horizons, Jobs to be Done, Innovator's Dilemma | `references/innovation-growth.md` |
| Defining goals and objectives | SMART (+ OKR if it needs to be rolled out over time) | `references/smart-goals.md` |
| Translating an already-defined strategy into a tracking system of indicators | Balanced Scorecard | `references/balanced-scorecard.md` |
| Stuck on a specific decision | Decision models (rational, intuitive, Cynefin, Six Thinking Hats, decision trees, cost/benefit) | `references/decision-making.md` |
| Need to generate options before deciding | Brainstorming, Delphi, cross-functional teams, design thinking | `references/decision-making.md` |
| Mapping stakeholders or prioritizing initiatives/risks | Mendelow Matrix, impact/effort matrix, risk matrix | `references/stakeholders-risk.md` |
| Organizational change under way | Kotter's 8-Step Change Process (urgency, guiding coalition, vision, communication, empowerment, short-term wins, consolidating, anchoring in culture) | `references/decision-making.md` |
| Highly uncertain environment, big and irreversible multi-year decision | Scenario planning | `references/environment-frameworks.md` |
| Investment/expansion decision with direct economic impact | Business case, unit economics, simplified payback/ROI/NPV | `references/financial-fundamentals.md` |
| Need to communicate or sell the plan to others | Strategic narrative — offered at the end, not applied upfront | `references/strategic-narrative.md` |
| General fundamentals (the 6 Ps, what a strategy contains, leadership vs. management) | Background framework, almost always implicit | `references/strategy-fundamentals.md` |
| Terminology questions, quality checklist before delivering | — | `references/glossary-and-checklist.md` |

Only load the `references/` file(s) that match the situation — don't load
all of them upfront.

## 3. Output template

Use `assets/templates/strategic-report.md` as the report skeleton, and
`assets/templates/framework-tables.md` for the table of the applied
framework (SWOT 2x2, PESTEL, Porter, BMC's 9 blocks, 7S, impact/effort
matrix, stakeholder map). Default output: a structured report with
sections/tables, not a wall of conversational text.

Before delivering, review the quality checklist in
`references/glossary-and-checklist.md`.

## 4. Closing: offer the strategic narrative

At the end of the report, if the user hasn't already asked for it, ask:

> "Would you also like help communicating this strategy — building the
> narrative to present it to your team or to others?"

Only if they say yes, load `references/strategic-narrative.md` and apply
that module. Never before: the narrative communicates a strategy that
doesn't exist yet.

## 5. General tone

The strategic mindset (values, leadership, narrative, long-term vision) can
color the general tone of your responses in this session when the user is
clearly in a business reflection or decision-making mode — but don't force
it into one-off, technical, or conversational questions within the same
session; return to a neutral tone as soon as the topic moves away from
strategy.
