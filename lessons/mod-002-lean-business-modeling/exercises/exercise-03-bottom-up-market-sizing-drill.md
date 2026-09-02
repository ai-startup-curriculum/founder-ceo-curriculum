# Exercise 03 — Bottom-Up Market Sizing Drill

**Module:** 002 Lean Business Modeling · **Stage:** IDEA→PRE-SEED · **Time:**
~90 focused minutes · **Prereq exercise:**
[exercise 01](./exercise-01-canvas-and-unit-economics.md) — you need the
segment definition and ARPA choice from the canvas before you can size
bottom-up defensibly. · **Reads with:** chapter
[06](../06-bottom-up-market-sizing.md).

## Problem statement

Founders reach for market sizing for two different jobs — the sanity
check and the pitch decoration — and confuse them at their cost. This
drill trains the sanity-check muscle: you take the segment definition
and ARPA choice from your exercise-01 canvas, size the addressable
revenue *bottom-up* from cited sources, and read the resulting ceiling
against the funding model you actually want the business to fit.

Ninety minutes here saves you from either building a lifestyle business
under venture-scale expectations or, more commonly, from talking
yourself into a decorative $30B TAM slide that a sophisticated audience
will silently discount the rest of your pitch against.

## Deliverable (one artifact)

A **bottom-up sizing worksheet** — one page — with:

- Your **segment definition** (from exercise 01, verbatim) and
  **plausible ARPA** (from the Revenue block of the canvas).
- A **segment-member count**, each source cited (LinkedIn filter query,
  Crunchbase / Carta report, industry-association directory,
  government occupational statistics, published company financials —
  something a reader could open in a tab).
- The **first-year addressable revenue ceiling** if the entire segment
  converted, computed as `segment members × ARPA × 12`.
- A **funding-model read** — is this ceiling big enough for
  bootstrapped, angel/seed, or Series A+ ambitions? — with a
  one-sentence justification.
- **Two adjacent-segment ladders** (if the winning ambition needs more
  scale than segment #1 alone provides), each with a segment-member
  count and an ARPA anchor.
- A **top-down decoration check** — if you were tempted to include a
  top-down TAM in a deck, what number would you have used, and why is
  the bottom-up number more honest?

## Scenario

Use the same scenario as exercise 01. This drill is only meaningful
against a specific segment and ARPA — abstract sizing is the exact
failure mode this exercise exists to prevent.

## Requirements

The worksheet has to satisfy each of the following:

- **Segment definition is the one from exercise 01, verbatim.** If you
  find yourself wanting to widen it here, that's information about
  either the canvas segment being too narrow *or* the sizing exercise
  being conducted on the wrong scale — resolve one way or the other,
  don't quietly widen for the sizing calculation.
- **Segment-member count is cited from a real source.** Not "roughly."
  Not "estimated." A filter, query, or report that a reader could
  reproduce. If the exact filter is unavailable, cite the closest
  proxy (industry association total × subset percentage) and name the
  proxy step.
- **ARPA is the one from the Revenue block**, or a defended alternative
  with a one-sentence reason for the change. "I raised the price to
  make the number bigger" is not a legitimate reason.
- **Arithmetic includes the ×12 for annualisation.** Bottom-up ceiling
  is annual, not monthly, and mistakes here shift the number by an
  order of magnitude.
- **Funding-model read is honest.** A $5M-ceiling business is a
  legitimate bootstrapped opportunity; it is not a defensible seed
  venture story on its own. A $200M-ceiling business is a legitimate
  seed venture story; it may or may not be a defensible Series A story
  depending on the adjacent-segment ladder.
- **Adjacent-segment ladder is real.** If segment #1 doesn't support
  the funding ambition, name segment #2 and segment #3 with their own
  segment counts and ARPA anchors — not "then we expand." Concrete
  adjacent segments, or the honest admission that they aren't yet
  identifiable.
- **Top-down decoration check is written.** Name the top-down TAM you
  *would* have put on the pitch slide, and articulate in one sentence
  why the bottom-up number is the one you'll actually defend.

## Starter guidance

**Step 1 — Copy the segment definition and ARPA from exercise 01**
(~5 min). Verbatim. No editing.

**Step 2 — Count the segment members** (~30 min). Try in order:
- LinkedIn filter (paid subscription helps for exact counts; a free
  account gives you order-of-magnitude by page count).
- Crunchbase or Carta queries for company-based segments.
- Industry-association directories or membership counts.
- Government occupational statistics (BLS OCC codes for US roles;
  equivalents in other geographies).
- Published company financials for competitor-customer-count proxies.

Whichever source you use, write down the exact filter or query — you
should be able to reopen it in a week and get the same number.

**Step 3 — Compute the annual ceiling** (~5 min).
`segment members × ARPA × 12 = first-year addressable revenue if you
captured the whole segment`. This is a ceiling, not a projection.

**Step 4 — Write the funding-model read** (~15 min). Use the ranges
from [chapter 06](../06-bottom-up-market-sizing.md) as a starting
point:
- Under $10M ceiling → likely bootstrapped territory.
- $10M–$100M ceiling → seed venture story if the adjacent-segment
  ladder is credible.
- $100M+ ceiling → Series A story if capture percentage is
  argued for.

Say which bucket the number falls in and why you find the fit
honest.

**Step 5 — Build the adjacent-segment ladder if needed** (~20 min).
If the funding ambition requires more scale than segment #1 provides,
name segment #2 and segment #3 with their own segment counts and ARPA
anchors. If they aren't yet identifiable, say so — an honest gap is
better than a fake ladder.

**Step 6 — The top-down decoration check** (~15 min). What would the
top-down TAM slide have said? A number from a Gartner report, an
analyst headline, a "developer tools is a $50B market" line. Write it
down. Then, in one sentence, articulate why the bottom-up number is
the one you'll defend to a sophisticated audience.

## Worksheet template (fill inline)

```
FROM EXERCISE 01:
  Segment definition (verbatim): ___
  ARPA ($/month): $___

SEGMENT-MEMBER COUNT:
  Count: ___
  Primary source (filter, query, report): ___
  Secondary / proxy source (if needed): ___
  Confidence: high / medium / low (why: ___)

BOTTOM-UP CEILING:
  Formula: segment members × ARPA × 12
  = ___ × $___ × 12
  = $___ (first-year addressable revenue if fully captured)

FUNDING-MODEL READ:
  Bucket: bootstrapped / angel or seed venture / Series A+
  Why this bucket is honest for this ceiling: ___

ADJACENT-SEGMENT LADDER (if needed):
  Segment #2 (name, count, ARPA anchor): ___
  Segment #3 (name, count, ARPA anchor): ___
  Or: adjacent segments not yet identifiable — honest gap (why: ___)

TOP-DOWN DECORATION CHECK:
  Top-down TAM I would have written: $___ (source: ___)
  Why the bottom-up number is the one I'll actually defend:
  ___
```

## Acceptance criteria

You are done when *all* of the following are true:

- [ ] The segment definition is **copied verbatim** from exercise 01.
- [ ] The **segment-member count cites a specific source** (filter,
      query, or report) that a reader could reopen.
- [ ] The arithmetic includes **×12 for annualisation** and produces a
      first-year ceiling in dollars.
- [ ] The **funding-model read** is one of the three named buckets and
      justified in one sentence.
- [ ] The **adjacent-segment ladder** is either populated with real
      segment #2 and #3 candidates *or* an honest admission that they
      aren't yet identifiable.
- [ ] The **top-down decoration check** names the number you would
      have used and, in one sentence, why bottom-up is more defensible.
- [ ] A skeptical co-founder reading the worksheet would agree that
      the ceiling is a defensible sanity-check number — not a pitch
      number and not a fantasy.

## Self-assessment rubric

| Dimension | Weak | Strong |
|---|---|---|
| Segment | Widened from exercise 01 to make the number bigger | Verbatim from exercise 01 |
| Segment-member count | "Estimated" or "roughly" | Real filter / query / report, reproducible |
| ARPA | Bumped up to hit a ceiling target | Same as canvas, or defended change with reason |
| Arithmetic | Missing ×12 or wrong unit | Explicit formula, correct annualisation |
| Funding-model read | Confuses bootstrapped with venture-scale | Correctly reads ceiling against funding ambition |
| Adjacent ladder | "Then we expand" hand-wave | Named segment #2 and #3 with counts and ARPAs, or honest gap |
| Top-down check | Puts a $30B TAM in the pitch anyway | Names it, defends bottom-up as the more honest number |
| Skeptic pass | Co-founder rolls eyes at the number | Co-founder agrees it's a defensible sanity check |

## Definition of done

A skeptical co-founder reading your worksheet would agree that the
number is a defensible sanity check — big enough to matter for the
funding path you want, or *honestly not big enough* and thus
redirecting you toward a different funding path (bootstrapped instead
of venture; venture instead of lifestyle). If the number is too big,
the segment or ARPA was inflated; if too small, the segment was
narrowed past the point of representing your actual market ambition.
Either way, the exercise has done its job: it has turned a private
guess into a public artifact that the next strategic decision has to
account for.

> Solutions are not provided in this repository; they live in the paired
> solutions repo.
