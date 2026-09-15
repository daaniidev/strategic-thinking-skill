# 🧭 Strategic Thinking Skill

**A Claude Code skill** that turns any business situation into a structured
analysis by applying the right strategic-consulting framework — not all of
them at once, and not before it has enough context.

> 🇪🇸 Versión en español: [pensamiento-mentalidad-estrategica](https://github.com/daaniidev/pensamiento-mentalidad-estrategica)

Instead of answering with generic frameworks or a wall of text, the skill
first asks the minimum needed (business, objective, time horizon, scope),
identifies whether the problem is **strategic** (long-term) or **tactical**
(short-term), picks 1–3 frameworks from its decision tree, and delivers a
report with clear sections and tables, ready to use.

## ✨ Why this skill

- **Asks before analyzing.** No auto-generated SWOT without context — the
  skill collects business, objective, time horizon and scope before picking
  a framework.
- **A decision tree, not a catalog.** 20+ frameworks organized by *user
  situation*, so the right one gets applied, not just the most popular one.
- **Explicitly separates strategy from tactics** in every report — never
  mixed without saying so.
- **Consistent output.** A report template plus per-framework tables (SWOT,
  PESTEL, Porter, BMC, 7S, impact/effort matrix, stakeholder map...) instead
  of free-form prose.
- **Optional narrative close.** Only if the user asks, it offers to help
  communicate the strategy once it's already defined — never before it
  exists.

## 📦 Installation

Copy this folder into your Claude Code skills directory (`.claude/skills/`
or `.agents/skills/`, depending on your setup):

```bash
git clone https://github.com/daaniidev/strategic-thinking-skill.git
```

Claude Code will automatically detect `SKILL.md` and activate the skill
when the conversation calls for it.

## 🚀 When it triggers

Say things like:

> "I need a SWOT analysis for my business"
> "How do I structure a strategic expansion plan?"
> "I want to validate my business model with a Business Model Canvas"
> "We're stuck on a big decision, what framework can help?"
> "Analyze the competition using Porter's five forces"

## 🗂️ Framework decision tree

| Situation | Framework(s) |
|---|---|
| Fast, unpredictable environment | VUCA / BANI |
| General starting point, internal/external risks | SWOT |
| Macro environment | PESTEL |
| Competitive structure of an industry | Porter's Five Forces |
| Designing or validating the business model | Business Model Canvas |
| Expansion into new markets | Ansoff Matrix |
| Internal organizational design | McKinsey 7S |
| Internal competitive advantage | VRIO, value chain, generic strategies |
| Portfolio of businesses/products | BCG Matrix / GE-McKinsey |
| New market space needed | Blue Ocean, Jobs to be Done, Three Horizons |
| Setting goals | SMART / OKR |
| Tracking an already-defined strategy | Balanced Scorecard |
| Stuck on a decision | Cynefin, Six Thinking Hats, decision trees |
| Stakeholder mapping / prioritization | Mendelow Matrix, impact/effort |
| Organizational change under way | Kotter's 8-step change process |
| Investment decision with direct economic impact | Business case, ROI/NPV, unit economics |
| Communicating strategy to others | Strategic narrative (offered at the end, on request) |

*(Full table with file references in [`SKILL.md`](SKILL.md).)*

## 📁 Project structure

```
.
├── SKILL.md                        # Skill definition, flow, and decision tree
├── assets/templates/
│   ├── strategic-report.md         # Final report skeleton
│   └── framework-tables.md         # Per-framework tables (SWOT, PESTEL, BMC...)
├── references/                     # One file per framework family
│   ├── environment-frameworks.md
│   ├── swot-pestel.md
│   ├── porter-canvas.md
│   ├── mckinsey-7s.md
│   ├── competitive-strategy.md
│   ├── portfolio-matrices.md
│   ├── innovation-growth.md
│   ├── smart-goals.md
│   ├── balanced-scorecard.md
│   ├── decision-making.md
│   ├── stakeholders-risk.md
│   ├── financial-fundamentals.md
│   ├── strategy-fundamentals.md
│   ├── strategic-narrative.md
│   └── glossary-and-checklist.md
└── LICENSE
```

## 🔗 Boundary with branding skills

If the request is purely about brand identity or positioning (naming,
manifesto, brand architecture), this skill says so explicitly and points to
`brand-strategy` or `brand-positioning` instead of forcing a SWOT/PESTEL
onto a problem that isn't one.

## 📄 License

[MIT](LICENSE) © 2026 daanidev
