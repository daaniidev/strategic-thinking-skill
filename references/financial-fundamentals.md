# Financial Fundamentals for Investment Decisions

**Scope warning**: this is NOT a corporate finance course and it does not
replace professional financial analysis for major decisions (an investment
round, an acquisition, a debt restructuring). It's the minimum set of numbers
a developer/founder needs in order not to decide blindly when a strategic
decision has an investment or scaling component — just enough to spot
whether an idea is obviously good, obviously bad, or deserves a closer look
from someone with deeper financial expertise before committing money. It
deliberately excludes WACC, company valuation, adjusted EBITDA, and full
discounted cash flow models: that belongs with a financial advisor, not this
skill.

## 1. Business case (strategic business case)

A business case is a short document (3-7 pages) that justifies an investment
by connecting the problem, options, cost, expected benefit, risk, and an
explicit recommendation. It's not a new analysis framework — it's how the
result of an analysis (SWOT, cost/benefit, a decision tree — see
`references/decision-making.md`) is **packaged** to request approval or
budget from someone who wasn't part of the process.

**When to use it**: once the internal decision on what to do has already been
made and someone (a partner, an investor, a client, or yourself before
committing savings) needs to be convinced the investment makes sense. It's
never the starting point of an analysis — it's the final wrapper.

### Minimum structure

1. **Executive summary** — one page, written last even though it goes first.
   Problem, recommendation, and cost/benefit in four sentences.
2. **Problem/opportunity** — what happens if this isn't addressed, with data
   where available.
3. **Options** — at least 3, always including:
   - Do nothing (baseline option, to compare against the cost of inaction).
   - Partial solution (cheaper, solves part of the problem).
   - Full solution (the recommended one, if applicable).
4. **Expected cost and benefit** — figures, even if they're estimated ranges
   ("between €8,000 and €15,000", not just "expensive"). This is where
   sections 2 and 3 of this file (unit economics and investment criteria)
   fit in, if the decision requires them.
5. **Risks** — 3-5, each with probability, impact, and mitigation.
6. **Recommendation** — the chosen option, explicitly tied to the numbers
   above, with a decision or execution deadline.

This structure is filled in within the existing
`assets/templates/strategic-report.md` (the "Context gathered", "Analysis",
and "Prioritized recommendations" sections cover most of the business case);
don't create a parallel template.

### Guiding questions

- Is the "do nothing" option genuinely viable, or is it just the convenient
  excuse for not deciding?
- Is the expected benefit backed by data (past sales, conversion rates,
  industry benchmarks), or is it hope disguised as a projection?
- Which risk on the list, if it materializes, invalidates the entire
  recommendation? If the answer is "none in particular", the real risk has
  probably not been identified yet.

## 2. Unit economics (CAC, LTV, per-unit margin)

Before looking at a business's aggregate P&L, you need to know whether it
makes or loses money on each individual customer or unit. This is essential
before scaling: a business can look healthy in aggregate (more revenue every
month) while losing money on every new customer, offset only by volume — an
accounting illusion that blows up as soon as you try to grow faster.

**Simplified formulas:**

- **CAC** (customer acquisition cost) = Total marketing and sales spend /
  Number of new customers acquired.
- **LTV** (customer lifetime value) ≈ (Average revenue per customer × Gross
  margin) / Churn rate.
- **LTV:CAC ratio** = LTV / CAC. Rule of thumb: ≥ 3:1 is considered healthy;
  < 1:1 means each customer costs more than they generate (the business
  loses money per customer, not just "in the short term").
- **Per-unit margin** = Selling price − Direct variable cost per unit.

**When to use it**: before deciding to scale customer acquisition, enter a
new market, or when the business is growing in revenue but it's unclear
whether it's growing in real profitability.

### Guiding questions

- Do we make money per customer before overhead, or only "at scale" — i.e.,
  does the improvement only appear if you assume a volume that doesn't exist
  yet?
- If we double acquisition spend to enter a new market, does CAC rise faster
  than LTV rises in that market?
- What happens to the LTV:CAC ratio if churn worsens by 5% when entering a
  new segment? (A healthy ratio in the current segment may not survive
  different churn in a new one.)

## 3. Simple investment evaluation criteria

Three quick ways to assess whether a specific investment pays off, ordered
from simplest to most complete. None replaces rigorous financial analysis —
they're enough to rule out clearly bad options or compare alternatives from
the business case against each other.

- **Payback period** = Investment cost / Annual cash flow generated. Gives
  the number of months or years to recover what was invested. Simple to
  calculate, but ignores what happens after the investment is recovered and
  the time value of money (€1,000 today is worth more than €1,000 three
  years from now).
- **Simple ROI** = (Benefit − Cost) / Cost, expressed as a percentage.
- **Very simplified NPV** (net present value): converts future money into
  "today's euros" by discounting it at a percentage, and subtracts the
  initial investment. Positive means the project generates more value than
  it costs (including opportunity cost); negative means it doesn't pay off
  compared to that alternative. Single-flow formula:

  ```
  NPV = Future cash flow / (1 + i)^t − initial investment
  ```

  There's no need to calculate it by hand or with decimal-level precision —
  the point to convey is: be careful comparing two projects purely on total
  benefit if they land on very different timelines; NPV corrects for that
  time bias. Also beware false precision: making up a specific discount rate
  and presenting it as if it were a rigorous calculation is worse than not
  calculating it at all, because it projects a rigor that doesn't exist.

### Guiding questions

- How long does it take to recover the investment, and is that timeframe
  acceptable given the risk of the chosen option?
- Is this option's ROI clearly better than the alternatives ruled out in the
  business case, or is it a tie that's actually decided by other factors
  (risk, timeline, team capacity)?
- If comparing two options with the same ROI but one takes twice as long to
  deliver results, which do we prefer and why? (There's no single answer — it
  depends on how much speed is worth in that context — but the question must
  be made explicit, not assumed.)

## When to load this file

Only when the decision has an explicit investment or scaling component
(requesting budget, deciding whether to scale customer acquisition, comparing
investment alternatives with figures). It's never the default entry point of
an analysis: the starting point remains SWOT/PESTEL for diagnosis and the
qualitative cost/benefit analysis in `references/decision-making.md` for
decisions that don't require this level of numerical detail.
