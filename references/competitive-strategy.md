# Competitive strategy: Porter's generic strategies, value chain, and VRIO

## Porter's generic strategies

Once the industry has been diagnosed (Five Forces, `porter-canvas.md`),
generic strategies answer the following question: within that industry,
how is this specific organization going to compete? They cross two axes —
market scope and the basis of competitive advantage — in a 2x2 matrix.

| | Cost advantage | Uniqueness advantage (differentiation) |
|---|---|---|
| **Broad scope** (whole market) | Cost leadership | Differentiation |
| **Narrow scope** (one segment) | Cost focus | Differentiation focus |

- **Cost leadership** — competing by being the cheapest option in the whole
  market, sustained by operational efficiency, economies of scale, or
  preferential access to resources. Only sustainable if cost is
  structurally lower than the competition's, not just a one-off low price.
- **Differentiation** — competing by offering something the customer
  perceives as unique (brand, technology, design, service) and is willing
  to pay a premium for, targeted at the whole market.
- **Cost focus** — the same low-cost logic, but applied to a narrow segment
  where the organization can operate more cheaply than any generalist.
- **Differentiation focus** — the same uniqueness logic, but applied to a
  narrow segment with specific needs that a generalist competitor doesn't
  serve well.

**The central risk: "stuck in the middle"**

An organization that doesn't clearly choose any of the four paths — that
tries to compete on both price and differentiation at once, without a real
advantage in either — ends up "stuck in the middle": it's neither the
cheapest option nor the most valued one, and loses to whoever has actually
picked a side. Typical signs: margins under constant pressure without being
the cost leader, and a positioning message that tries to be "good quality
at a good price" without evidence of either against the competition.

**What it's for**: deciding the basis of competitive advantage an
organization will compete on within an already-diagnosed industry, and
detecting whether the current problem is precisely that none has been
clearly chosen.

**When to use it**: after Porter's Five Forces (`porter-canvas.md`), when
the question shifts from "is this industry attractive?" to "how do we
compete within it?". It differs from the Ansoff Matrix (`porter-canvas.md`):
Ansoff decides the product/market axis for growth, this decides the basis
of competitive advantage used to compete, whether or not the organization
grows.

**Guiding questions**:
- If you had to choose only one lever of advantage — price or
  differentiation — which does your organization defend better today with
  data, not intent?
- Do you compete across the whole market, or would you be better off
  focusing on a narrow segment where you can clearly win?
- Are there signs of being "stuck in the middle" — neither the cheapest nor
  the most valued, with margins under pressure?

## Porter's value chain

The value chain breaks the organization down into the specific activities
that create value for the customer, to locate where competitive advantage
is generated (or lost). It splits into primary activities — the direct flow
of creating the product or service — and support activities — what sustains
the primary ones without directly touching the customer.

**Primary activities** (the operational flow, from input to output)

| Activity | What it covers |
|---|---|
| Inbound logistics | Receiving, storing, and managing inputs and raw materials |
| Operations | Transforming inputs into the final product or service |
| Outbound logistics | Storing and distributing the product or service to the customer |
| Marketing and sales | Communication, pricing, and channels that get the customer to buy |
| After-sales service | Support, maintenance, and care after the sale is made |

**Support activities** (sustain the primary ones, cross-cutting)

| Activity | What it covers |
|---|---|
| Firm infrastructure | General management, finance, planning, quality |
| HR management | Recruiting, training, retaining, and developing talent |
| Technology development | R&D, automation, systems that improve any primary activity |
| Procurement | Acquiring the resources used by both primary and support activities |

**Margin** is the difference between the total value the customer perceives
across the set of activities and the cost of performing them. The value
chain is used to locate exactly which activity generates that margin and
which one destroys it.

**What it's for**: identifying, activity by activity, where real
competitive advantage is generated (lower cost or higher perceived value
than the competition) and where the organization is simply incurring cost
without creating any differential.

**When to use it**: when you need to drill down from the chosen generic
strategy (cost or differentiation) into the operational detail of which
specific activity sustains it, or to decide which activities to outsource.
It differs from McKinsey 7S (`mckinsey-7s.md`): 7S looks at broad
organizational alignment (structure, culture, systems, people); the value
chain looks specifically at the operational flow of value creation,
activity by activity.

**Guiding questions**:
- Which activity costs you more than it costs the competition, and why?
- In which specific activity does the customer perceive differential value
  compared to other options in the market?
- Which activities add no competitive advantage and are candidates for
  outsourcing or simplifying?

## VRIO

VRIO evaluates whether a specific resource or capability of the
organization (brand, technology, data, team, a specific process...) is
really a source of competitive advantage. It's a sequence of 4 questions:
each "no" answer stops the analysis at that point, and the combination of
answers reached determines the result.

1. **Value** — does the resource allow the organization to exploit an
   opportunity or neutralize a threat from the environment?
2. **Rarity** — do few competitors (or none) have it?
3. **Imitability** — is it costly or difficult for others to replicate?
4. **Organization** — is the company organized (processes, structure,
   incentives) to actually exploit it?

| Value | Rarity | Imitability (hard) | Organization | Result |
|---|---|---|---|---|
| No | — | — | — | Competitive disadvantage |
| Yes | No | — | — | Competitive parity |
| Yes | Yes | No | — | Temporary competitive advantage |
| Yes | Yes | Yes | No | Unexploited advantage |
| Yes | Yes | Yes | Yes | Sustained competitive advantage |

**What it's for**: auditing specific resources and capabilities — not full
processes — to know which ones are truly defensible over time and which
ones only give a passing advantage or none at all.

**When to use it**: it's the internal complement to Porter's Five Forces
(external, `porter-canvas.md`): the Five Forces look at industry pressure
from the outside, VRIO looks at whether the organization's own resources
can withstand that pressure from the inside. It's different from the value
chain: the chain maps activities and processes end to end, VRIO evaluates
specific resources or capabilities in isolation (a particular dataset, a
patent, a team).

**Guiding questions**:
- Of your resources (brand, technology, data, team, processes), which ones
  pass all 4 VRIO tests?
- If you have a valuable and rare resource that's easy to copy, how much of
  an advantage window do you have left before the competition replicates
  it?
- Do you have valuable, rare resources the organization isn't exploiting
  due to a lack of internal structure, processes, or incentives?

## How they relate to each other

The three frameworks in this file work in cascade, from the broadest
decision to the most granular:

1. **Generic strategies** decide the basis of competitive advantage (cost
   or differentiation) and the scope (broad or narrow) used to compete.
2. **Value chain** brings that decision down to operational detail: which
   specific activities, from input to output, sustain the chosen advantage.
3. **VRIO** goes one level deeper: within those activities, which specific
   resources or capabilities are truly defensible against the competition,
   and which aren't.

And with the rest of the repo:

- **Porter's Five Forces** (`porter-canvas.md`) diagnose whether the
  industry is attractive from the outside; generic strategies decide how to
  compete within that already-diagnosed industry. VRIO is the internal
  equivalent of the Five Forces: while they look at external pressure,
  VRIO looks at whether the organization's own resources can withstand
  that pressure.
- **Ansoff Matrix** (`porter-canvas.md`) decides which direction to grow in
  (product/market axis); Porter's generic strategies decide what advantage
  to compete with, regardless of the growth path chosen. They aren't
  alternatives: an organization can decide on "market penetration" with
  Ansoff and "cost leadership" with Porter at the same time.
- **McKinsey 7S** (`mckinsey-7s.md`) audits broad organizational alignment
  (structure, systems, culture); the value chain specifically audits the
  operational flow of value creation. Both can reveal that a well-chosen
  strategy isn't holding up internally, but from different angles.

## Template

Ready-to-fill tables (generic strategies matrix, value chain, and VRIO
table) are in `assets/templates/framework-tables.md`.
