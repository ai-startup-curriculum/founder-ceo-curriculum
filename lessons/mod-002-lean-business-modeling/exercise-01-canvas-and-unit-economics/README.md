# Exercise 01 — Lean Canvas & Unit Economics

**Module:** 002 Lean Business Modeling · **Stage:** IDEA→PRE-SEED · **Time:** ~1
week (≈6–8 focused hours)

## Deliverables (two founder artifacts, plus one call)

1. **A lean canvas** (one page, nine blocks) traceable to your mod-001 discovery
   evidence.
2. **A unit-economics sheet** naming CAC, ARPA, gross margin, churn, LTV, LTV:CAC,
   and CAC payback — with sources or assumptions cited per line.
3. **A one-paragraph "riskiest assumption" call** — the single assumption that
   would kill the business if wrong, and the cheapest experiment that would tell
   you whether it holds.

## Scenario

Pick one:

- **Your real startup** (recommended if you're an operating founder): use your
  actual discovery notes and your real (or best-guess) numbers.
- **Simulated:** use the mod-001 exemplar's segment — *first-time technical
  founders in their first 12 months of raising* — and the sharpened problem
  framing ("what to learn when; what to ignore now"). Assume a subscription
  product priced somewhere in the $20–$200/mo range; you choose the point and
  defend it.

## Steps

1. **Fill the canvas problem-first.** Work in Ash Maurya's recommended order:
   Segment → Problem → UVP → Solution → Channels → Revenue → Cost → Key Metrics
   → Unfair Advantage. Each block gets one to three lines; a whole page beats a
   dense page.
2. **Trace each block to evidence.** For every block, add a one-line note: *what
   discovery interview, prior-spend signal, competitor teardown, or public data
   point supports this?* Blocks with no source get flagged as **assumption** —
   that's fine, but you should be able to count them.
3. **Build the unit-economics sheet.** Fill the six inputs (CAC, ARPA, variable
   cost per unit, gross margin, churn rate, average customer lifetime), then
   derive LTV, LTV:CAC, and CAC payback. Use the template below. Cite the source
   or the assumption behind every number.
4. **Sanity-check with a bottom-up market size.** `number of segment members ×
   plausible ARPA × 12` gives you a first-year ceiling if you captured the whole
   segment. Enough to be a company? If not, the segment is probably too narrow
   — or the pricing is.
5. **Name the riskiest assumption.** Which single input, if it comes in at half
   what you assumed, kills the model? Willingness to pay? A working channel?
   Retention past month three? Gross margin (a real risk for AI-heavy products
   with per-request inference cost)?
6. **Design the cheapest experiment for it.** A landing page + paid-ad test for
   willingness-to-pay. A cold outbound sequence to 50 targets for channel. A
   concierge / manual-behind-the-curtain MVP to a handful of paying design
   partners for retention. Write down: what would you run this week, and what
   result would change your call?

## Lean canvas template (fill inline)

```
Customer Segments:
  Early adopter (be specific):
  Broader segment:

Problem:
  1.
  2.
  3.
  Existing alternatives:

Unique Value Proposition:
  One sentence:
  High-concept pitch (X for Y):

Solution:
  1. →  (maps to Problem 1)
  2. →  (maps to Problem 2)
  3. →  (maps to Problem 3)

Channels:
  Free / owned:
  Paid:
  Founder-driven:

Revenue Streams:
  Pricing model:
  Price point(s):
  Willingness-to-pay evidence:

Cost Structure:
  Fixed:
  Variable (per customer):
  Customer acquisition cost drivers:

Key Metrics:
  (3–5 numbers that tell you it's working)

Unfair Advantage:
  (empty is an honest answer)
```

## Unit-economics template (fill inline)

```
Inputs (cite source or mark ASSUMPTION):
  ARPA (avg revenue per account, $/mo):
  Variable cost per customer per month ($):
  Gross margin % = (ARPA - variable cost) / ARPA:
  Monthly churn rate (%):
  Avg customer lifetime (months) ≈ 1 / churn:
  CAC ($, blended across channels):

Derived:
  LTV ≈ ARPA × gross margin % × avg lifetime  =
  LTV : CAC =
  CAC payback (months) ≈ CAC / (ARPA × gross margin %) =

Sanity checks:
  Bottom-up TAM: segment size × ARPA × 12 =
  Which single input, halved, breaks the model?
```

## Rubric (self-assess, then compare to the exemplar)

<!-- needs-research: exemplar for mod-002 not yet authored; rubric-vs-exemplar comparison assumes future exemplars/mod-002-lean-business-modeling/. -->

| Dimension | Weak | Strong |
|---|---|---|
| Segment | "SMBs" / "developers" | Narrow early adopter, recognizable in one sentence |
| Problem block | Restated solution ("they need our tool") | Ripped from discovery, with existing alternatives named |
| UVP | Feature list | One-sentence, outcome-focused, aimed at the segment |
| Channels | "SEO + content" hand-wave | Named channels with a testable cost-to-reach |
| Revenue | "We'll figure out pricing later" | A price with willingness-to-pay evidence |
| Unit economics | Revenue-based LTV, no margin | Gross-margin LTV with cited variable costs |
| Riskiest assumption | "Getting distribution" | One specific input, named, with a cheap next test |

## Definition of done

A skeptical seed-stage investor reading your canvas and economics sheet would
agree that (a) the biggest risk in the business is the one you named, and (b)
the experiment you propose next would actually change your mind if it failed.
