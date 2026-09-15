# Portfolio matrices: BCG Matrix and GE-McKinsey Matrix

Unlike Porter (industry structure) or the Business Model Canvas (designing a
single business), portfolio matrices don't analyze one business in isolation:
they compare and prioritize **multiple business lines, products, or units**
within the same organization, to decide where to invest, where to hold, and
where to divest.

## BCG Matrix (growth-share matrix)

Developed by the Boston Consulting Group, this is a 2x2 matrix that crosses
two metrics: the growth rate of the market each business line competes in
(Y-axis, high/low) and its relative market share compared to the largest
competitor (X-axis, high/low).

| | High relative market share | Low relative market share |
|---|---|---|
| **High market growth** | Star | Question Mark |
| **Low market growth** | Cash Cow | Dog |

- **Star** — leader in a market that is still growing fast. It generates cash
  but also consumes it, since continued investment is needed to defend
  leadership. *Decision:* invest to sustain the position; over time, if the
  market matures and share is maintained, it becomes a Cash Cow.
- **Cash Cow** — leader in an already mature or slow-growing market. It no
  longer needs heavy investment and generates cash steadily. *Decision:*
  "milk" it — extract the cash surplus without over-investing, and use it to
  fund Stars and Question Marks.
- **Question Mark** (sometimes called a "problem child") — low share in a
  fast-growing market. It consumes cash without generating it, and its future
  is uncertain: it can become a Star with the right investment, or turn into
  a Dog if it fails to take off. *Decision:* the most demanding of the four —
  pick a small number of Question Marks to bet on heavily, and exit or divest
  the rest before they keep draining cash with no clear direction.
- **Dog** — low share in a market that is no longer growing. It doesn't
  generate meaningful cash and has no prospect of improving its position.
  *Decision:* a natural candidate for divestment, liquidation, or
  discontinuation, unless it serves a specific strategic purpose (for
  example, rounding out a catalog or retaining a key customer relationship).

**Cash flow logic is the heart of the model**: Cash Cows fund the Stars (so
they don't depend on external capital) and a selected subset of Question
Marks; Dogs receive no further investment and are liquidated or discontinued
to free up resources. A healthy portfolio isn't made up of only Stars or only
Cash Cows: it needs today's Cash Cows to fund the Stars and Question Marks
that will become tomorrow's Cash Cows.

**What it's for:** giving a quick, visual diagnosis of a portfolio with
multiple business lines or products, using just two easily estimated metrics
(market growth and relative share), to decide where to redirect investment.

**When to use it:** when the user has several business lines, products, or
units and needs a fast diagnosis of "where to invest, hold, or close" without
a multi-factor analysis. It's the natural starting point when the user
doesn't have (or doesn't need) finer-grained data than revenue/share and
market growth per line.

### Guiding questions

- Of all your business lines or products, which generate cash today (Cash
  Cows) and which consume it (Stars, Question Marks)?
- Among your Question Marks, which deserves a strong investment bet, and
  which should be closed or sold before they keep draining cash?
- Are you reinvesting the surplus from your Cash Cows in the right place
  (your Stars and the chosen Question Mark), or is it being diluted into
  propping up Dogs or funding general overhead?
- Do you have any Dog that's still alive out of inertia or for non-financial
  reasons (customer relationship, brand image) that should be made explicit
  rather than left hidden?

## GE-McKinsey Matrix (business screen)

The GE-McKinsey Matrix emerged as an evolution of the BCG Matrix to overcome
its main limitation: reducing market attractiveness to a single metric
(growth) and competitive position to another (share). Instead, it uses two
**composite, weighted axes**, each built from several scored criteria with a
relative weight, plotted on a 9-cell (3x3) grid instead of 4.

- **Y-axis — Industry attractiveness**: market size, growth rate, average
  industry profitability, competitive intensity, relevant macro trends
  (regulation, technology). Each criterion is scored (for example, 1 to 5)
  and weighted according to its importance for the specific case; the
  weighted sum places the business at High/Medium/Low on this axis.
- **X-axis — Competitive strength of the business**: market share,
  capabilities and talent, product/service quality, brand strength, cost
  position relative to competitors. As with the Y-axis, each criterion is
  scored and weighted individually.

| | High competitive strength | Medium competitive strength | Low competitive strength |
|---|---|---|---|
| **High industry attractiveness** | Invest/grow | Invest/grow | Selectivity/hold |
| **Medium industry attractiveness** | Invest/grow | Selectivity/hold | Harvest/divest |
| **Low industry attractiveness** | Selectivity/hold | Harvest/divest | Harvest/divest |

The 9 cells group into three decision zones:

- **Invest/grow** (top-left corner, high-high) — the industry is attractive
  and the business competes strongly within it. *Decision:* concentrate
  investment here; this is the equivalent of BCG's Star, but justified with
  more criteria than just share and growth.
- **Selectivity/hold** (central diagonal) — a mixed combination: an
  attractive industry with medium/low strength, or a medium industry with
  high strength. *Decision:* invest selectively, only where there's a
  concrete reason to strengthen the position, and hold the rest without major
  new capital commitments.
- **Harvest/divest** (bottom-right corner, low-low) — an unattractive
  industry and weak competitive strength. *Decision:* extract remaining
  value without new investment (harvest) or divest outright; this is the
  equivalent of BCG's discarded Dogs and Question Marks.

**What it's for:** prioritizing investment across multiple businesses or
units when a single metric per axis (as in the BCG Matrix) oversimplifies
reality — for example, when industry profitability matters more than its
size, or when competitive strength depends on brand and capabilities rather
than just market share.

**When to use it:** when the user needs a more rigorous or nuanced analysis
than the BCG Matrix, has complex businesses where share and growth don't tell
the whole story, or has (or can reasonably estimate) several criteria per
axis instead of a single metric.

### Guiding questions

- Using your own attractiveness criteria (not just market growth) — size,
  profitability, competitive intensity, macro trends — how attractive is
  this industry for the coming years?
- How does this business score on competitive strength beyond market share —
  capabilities, quality, brand, cost position?
- What weight do you give each criterion, and why? (The same business can
  land in different cells depending on how the user weights the criteria —
  make that explicit rather than leaving it implicit.)
- Given where this business falls on the grid, is the right decision to
  invest for growth, hold with selective investment, or divest?

## When to use each

The **BCG Matrix** is fast and simple: it only needs two metrics per business
line (market growth and relative share), which makes it the best option for
a quick diagnosis or when the user lacks finer-grained data. The
**GE-McKinsey Matrix** is more nuanced and multi-factor: it requires scoring
and weighting several criteria per axis, so it's worth using when the user
needs a more rigorous analysis, the portfolio is complex, or a single metric
per axis (like share or growth) would distort the decision. When in doubt,
start with the BCG Matrix — it's cheaper to build — and move up to the
GE-McKinsey Matrix if the user asks for more depth or the BCG result leaves
businesses in ambiguous zones (especially Question Marks) that need more
criteria to decide.

### Difference from the Ansoff Matrix

The BCG Matrix and GE-McKinsey Matrix shouldn't be confused with the Ansoff
Matrix (see `porter-canvas.md`), even though all three are 2x2/3x3
strategic decision matrices:

- **The Ansoff Matrix** decides **how to grow a single business or product**,
  crossing product (current/new) with market (current/new). Its question is
  "which direction should I expand in?".
- **The BCG Matrix and GE-McKinsey Matrix** compare and prioritize **among
  several businesses or products that already exist** within the
  organization's portfolio. Their question is "of everything I already have,
  where do I invest, hold, or close?".

In practice, they can be combined: first use the BCG Matrix/GE-McKinsey
Matrix to decide which business line to concentrate investment in, and then
the Ansoff Matrix to decide how that chosen line should specifically grow.

## Template

Ready-to-fill tables (the 2x2 BCG Matrix and the 3x3 GE-McKinsey Matrix) are
available in `assets/templates/framework-tables.md`.
