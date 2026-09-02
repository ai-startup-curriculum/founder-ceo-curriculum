# Chapter 06 — Bottom-Up Market Sizing: The Sanity Check, Not the Pitch

> **Reads with:** module objective 6 — *size the market bottom-up (segment
> members × plausible ARPA) as a sanity check, and defend why top-down
> analyst reports are decorative at this stage.*

## What market sizing is for at IDEA→PRE-SEED

Founders reach for market sizing for two different jobs and confuse
them at their cost:

- **The sanity check.** *If the model works, is there enough
  addressable revenue for this to be a company?* This is the version
  a founder owes themselves before spending a year on the bet.
- **The pitch decoration.** *A big number to put on slide 7 of the
  deck so the market looks huge.* This is the version that turns
  into a $30B TAM slide with a "we only need 1%" footnote and quietly
  destroys the credibility of the rest of the deck.

This module is entirely about the first job. The market-size slide in
a fundraising deck is a downstream artifact (covered in mod-004), and
its main function is to *not lie*; the way you avoid lying is to build
it bottom-up here and carry that bottom-up number forward.

## Top-down sizing: why it's decorative at this stage

The classical vocabulary — **TAM / SAM / SOM** — comes from strategy
consulting:

- **TAM (Total Addressable Market)** — every dollar of spend on the
  broadest possible category the product touches.
- **SAM (Serviceable Addressable Market)** — the portion of TAM your
  product could serve given segment, geography, and language
  constraints.
- **SOM (Serviceable Obtainable Market)** — the portion of SAM you
  could plausibly capture in a defined time horizon.

The trouble with top-down TAM is the source. It usually comes from an
analyst report ("the global marketing-software market was $X billion
in 2024, growing at Y% CAGR"). Analyst reports are aggregations of
prior categories; they encode last decade's segmentation, not this
year's product, and their numbers are almost always designed to be
big — a large TAM sells more reports.

Two failure shapes:

- **"$300B TAM, we only need 1%."** The "we only need 1%" framing
  works arithmetically but not economically. Every incumbent already
  owns some of that 1%, and no company has ever built distribution
  by mailing 1% of a $300B market with the hope that they answer.
  Investors have seen this slide too many times; it lowers rather
  than raises confidence.
- **TAM that includes markets you can't touch.** A $50B "developer
  tools" TAM is not addressable by a company that sells only to
  Python data-science teams at Series B+ companies in the US. The
  fraction of TAM that is actually SAM for that segment is a
  hundredth of the headline number, and no one on the call believes
  the number anyway.

The correct posture at IDEA→PRE-SEED is: **top-down sizing does not
tell you anything the model needs to know**. It looks impressive on a
slide, and the sophisticated audience discounts it precisely because
it's easy to inflate. Bottom-up sizing does the actual work.

## Bottom-up sizing: the formula and the discipline

**The formula.**

```
first-year addressable revenue ≈ segment members × plausible ARPA × 12
```

For a subscription business, "plausible ARPA" is the price you would
charge, multiplied by 12 for the annualised view. For a transactional
business, replace `ARPA × 12` with `annual spend per customer`.

This number tells you the **ceiling** if you captured the whole
segment for a year. Actual capture will be a small fraction of this
ceiling in year one and a larger fraction over time; the ceiling
being high enough to matter is the sanity check.

**The discipline.**

Bottom-up sizing is done right when it does three things:

1. **Cites where the segment-member count comes from.** LinkedIn
   filter counts, Crunchbase queries, industry-association member
   directories, government occupational statistics, published
   company financials. Not "estimated." Not "roughly." A defensible
   source you could open in a tab.
2. **Uses an ARPA anchored in willingness-to-pay evidence.** From
   competitor pricing pages, from prior-spend answers in discovery,
   from LOI / signed pilot numbers. Not a hopeful guess.
3. **States assumptions explicitly.** Segment membership shifts;
   ARPA depends on packaging; capture is a percentage that will be
   argued about. Naming the three inputs and their sources lets a
   skeptic replace any of them and re-run the arithmetic themselves.

### Worked example (from the module exemplar)

- **Segment members.** *First-time technical founders who
  incorporated and started raising a pre-seed in the last 12 months.*
  Rough source: Y Combinator batch sizes plus reasonable multipliers
  for non-YC pre-seed activity in the US and Europe. Order-of-magnitude:
  ~10,000–20,000 people per year meeting that filter.
  <!-- needs-research: primary-source citation for annual first-time-founder / pre-seed volume — Crunchbase or Carta data on pre-seed formation counts. -->
- **Plausible ARPA.** Discovery buyers named $50–$200/mo as
  comparable spend on YC-adjacent courses, advisor time, and
  founder-community memberships. Anchor: $99/mo → $1,188/yr.
- **First-year addressable revenue if entire segment converted.**
  ~15,000 × $1,188 ≈ **$17.8M** as a first-year ceiling.

That number is not a projection — it's the ceiling. Realistic
first-year capture is a percentage of it; even 5% capture would be
~$900K of first-year ARR, which is above the "is this a business?"
threshold for a bootstrapped model and below the "is this
venture-scale?" threshold. Bottom-up sizing has done exactly its
job: it has surfaced that the segment as narrowly defined here is
too small to be a venture-scale bet on its own and needs a broader
segment for that outcome — a real strategic finding, not a slide.

## How "big enough" depends on the funding model

Different funding paths tolerate different addressable-revenue
ceilings. The three main shapes:

- **Bootstrapped / lifestyle.** $1–10M/yr of first-year ceiling on
  a narrowly defined segment can be enough — the founder captures
  a meaningful fraction, the business supports a small team, and
  no external capital is required. Under $1M and even the founder
  can't earn a living from it.
- **Angel / pre-seed / seed venture.** The ceiling on the first
  segment should support the *ambition to grow into adjacent
  segments*. If bottom-up on segment #1 shows $10M and the plan is
  "then expand to segment #2 at $80M and #3 at $200M," that's a
  legitimate seed story if the adjacent segments are argued for.
- **Late-seed / Series A venture.** The eventual $1B+ TAM story
  needs to be defensible from the bottom-up ladder. A common
  informal threshold is that the *addressable* market — not
  aspirational TAM — must plausibly support at least $100M in
  annualised revenue for a company inside a reasonable time
  horizon.
  <!-- needs-research: primary-source citation for the "$100M ARR / $1B TAM" venture threshold — commonly cited from a16z / Bessemer / First Round writing on venture scale; specific origin varies. -->

At IDEA→PRE-SEED, being on the small end of one of these buckets is
not automatic bad news — it's information about which funding path
this business can honestly pursue. A founder who confuses "not
venture-scale" with "not a business" leaves real bootstrappable
opportunities on the table; a founder who confuses "not a business"
with "venture-scale" burns real money.

## Common bottom-up mistakes

Four ways bottom-up sizing goes wrong:

- **Over-narrow segment.** The segment definition is so tight that
  bottom-up membership is 300 people, and the ceiling is a
  lifestyle business. Real finding — but sometimes the segment was
  narrowed for a discovery reason and is not the right *market*
  segment. Check that the narrow segment is your **early-adopter
  carve-out** (chapter 01), not the whole market.
- **Over-broad ARPA.** Enterprise-scale ARPA applied to a
  small-business segment. If the segment members can't credibly pay
  $10K/mo, don't put $10K/mo in the formula.
- **Segment × ARPA with no time dimension.** `segment members ×
  ARPA` (missing the ×12 for annualised revenue) understates the
  business by a factor of 12 in the annual view and produces a
  ceiling that looks alarming when it isn't. Or, ARPA is monthly and
  the analyst assumes annual — same category, opposite direction.
- **Ignoring segment shift over time.** A first-year segment
  membership of 15,000 for "founders who incorporated this year" is
  a *recurring* population, not a one-time addressable pool — new
  cohorts appear annually. LTV-based sizing (bottom-up ceiling ×
  average lifetime × capture percentage) is a more honest long-view
  number.

## From bottom-up sizing to the pitch — and the boundary

This chapter is about the sanity check. Once bottom-up sizing tells
you the model is capable of supporting the ambition you have for it,
the *presentation* of that number in a fundraising deck — how to
frame TAM/SAM/SOM defensibly, how to sequence adjacent-segment
expansion in the story, how to argue for growth rate — is a
mod-004 topic (Fundraising Pre-seed to Seed). The deep craft of
**pricing, packaging, and per-channel economics** — how to size the
addressable market of a specific channel, how to defend a specific
price point against willingness-to-pay research, how to model
freemium-to-paid conversion — belongs to the
**`startup-product-gtm-curriculum`** track (see chapter 07 for the
boundary).

Founder-CEO owes the bottom-up ceiling and the honest read of what
funding path it can support. The deeper craft of turning it into a
defended pricing tier and a defended channel-specific CAC belongs
to the peer track.

## Summary

- Market sizing at IDEA→PRE-SEED is a **sanity check**, not a
  pitch. Bottom-up (`segment members × plausible ARPA × 12`) does
  the actual work; top-down TAM is decorative and often
  counterproductive.
- Bottom-up sizing is done right when the **segment-member count is
  cited**, the **ARPA is anchored in willingness-to-pay evidence**,
  and the **assumptions are stated**.
- Whether the resulting ceiling is "big enough" depends on the
  **funding model** — bootstrapped, seed venture, or
  Series-A-and-up. Small ceilings are information, not failure.
- Deep pricing / packaging / channel-economics craft is deferred to
  the **`startup-product-gtm-curriculum`** peer track; this chapter
  owns the founder-level sanity check.

**Next:** the boundary itself — where this module's work stops and
the startup-product-gtm track picks up the deeper GTM craft — in
[chapter 07](./07-boundary-gtm-pricing-channels.md).
