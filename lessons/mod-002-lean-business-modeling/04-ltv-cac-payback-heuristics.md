# Chapter 04 — Derived Metrics: LTV, LTV:CAC, and CAC Payback as Heuristics, Not Laws

> **Reads with:** module objective 4 — *derive LTV, LTV : CAC ratio, and
> CAC payback period, applying the SaaS heuristics (David Skok / For
> Entrepreneurs: LTV : CAC > 3× as a scale-signal, payback < ~12 months)
> as heuristics rather than laws.*

## What derived metrics tell you that raw inputs don't

The four raw inputs from [chapter 03](./03-unit-economics-four-numbers.md)
tell you how a single transaction and a single customer behave. The
three **derived** metrics — LTV, LTV:CAC, and CAC payback — tell you
whether the *shape of the model as a whole is fundable*. Fundable here
does not mean "will get funded"; it means "generates enough gross profit
per acquired customer, quickly enough, that scaling paid acquisition
compounds capital instead of burning it."

The rest of this chapter walks each metric, the widely-cited SaaS
heuristic attached to it, and — importantly — the ways the heuristic
misleads if you apply it without thinking.

## LTV — customer lifetime value

**Definition:** the total gross profit a typical customer generates
over their entire relationship with you.

For a subscription business with roughly constant monthly churn, a
common closed-form approximation is:

```
LTV ≈ ARPA × gross margin % / monthly churn rate
```

Equivalent form:

```
LTV ≈ ARPA × gross margin % × average customer lifetime (months)
```

where average lifetime `≈ 1 / monthly churn` under the same
constant-churn assumption.

**The gross-margin multiplier is not optional.** LTV computed on
*revenue* (ARPA × lifetime, with no margin term) overstates a
low-margin business dramatically. A $100/mo ARPA customer with 24-month
lifetime looks like $2,400 of LTV on a revenue basis. If gross margin
is 80% (clean SaaS), the true gross-profit LTV is $1,920 — the
overstatement is small. If gross margin is 30% (AI product with heavy
per-request inference cost), the true LTV is $720. That's a 3.3×
overstatement, and every downstream ratio inherits it.

**Three ways the constant-churn approximation misleads.**

- **Early churn is almost always higher than late churn.** Customers who
  survive the first 90 days retain much better than the average of the
  first 30 days. Using a blended churn number computed against a young
  book overstates lifetime for customers who make it past onboarding
  and understates it for the ones who don't.
- **Contract length and payment terms distort the "monthly" view.** An
  annual-prepaid customer has near-zero churn during the paid year and
  a lumpy renewal decision at month 12. Treating them as a monthly-churn
  cohort mis-models the actual decision points.
- **Segment mix.** If enterprise customers churn at 1% and SMB at 6%,
  a blended 3% is not the model of any actual customer. Segmented LTV
  computed per cohort is much more honest — but requires enough data
  per segment to be meaningful, which you usually don't have at
  IDEA→PRE-SEED.

At this stage the honest posture: pick the formula, mark every input
as ASSUMPTION or evidence, and know which one, if wrong, breaks the
number.

## LTV : CAC — the scale-signal ratio

**Definition:** the ratio of lifetime value to customer acquisition
cost.

```
LTV : CAC = LTV / CAC
```

The most widely-cited heuristic in SaaS unit economics — attributed to
David Skok on the *For Entrepreneurs* blog — is that a healthy
subscription business scaling paid acquisition should target
**LTV : CAC > 3×**.
<!-- needs-research: primary-source citation for the ">3x LTV:CAC" heuristic — Skok's "SaaS Metrics 2.0" post at forentrepreneurs.com; add stable URL and publication year. -->

The intuition behind 3× is that CAC is paid up-front and confidently
(you can measure it), while LTV is realised over years and
uncertainly (churn drifts, expansion doesn't materialise, gross
margin compresses). A 3× target builds margin for the LTV side to
underperform its projection and still leave the business making money.

**Landmarks around 3×:**

- **< 1×**: you lose money on every customer you acquire. Growth makes
  the loss bigger; this is not a business you can raise against
  without a plan to change one of the inputs.
- **1× – 3×**: the business breaks even on customers but doesn't
  compound. Acceptable for a mature, low-growth vertical; not enough
  margin for the risk-adjusted case a venture investor wants to
  underwrite.
- **> 3×**: the target for a subscription business scaling paid
  acquisition. Sustained > 5× on real numbers (not projected ones)
  is very strong.

**Three ways LTV:CAC misleads.**

- **It rewards low CAC via founder time.** A founder doing free
  outbound has CAC that looks like $50, LTV of $5,000 (against 3-year
  lifetime), and a ratio of 100×. The ratio evaporates when the
  founder tries to hire an SDR. Include founder time in CAC (see
  [chapter 03](./03-unit-economics-four-numbers.md)) or the ratio is
  fiction.
- **It's silent on cash timing.** A ratio of 4× with LTV realised
  over five years and CAC paid in month 1 requires you to fund the
  gap — potentially years of upfront burn before the LTV shows up.
  CAC payback (below) is the metric that catches this.
- **It's silent on absolute size.** LTV:CAC of 10× on a $10 LTV
  business is not fundable; the business isn't big enough to matter
  even if every customer's ratio is beautiful. Absolute scale is a
  separate question (chapter 06).

## CAC payback period

**Definition:** the number of months of gross-margin dollars needed to
earn back the acquisition cost.

```
CAC payback (months) ≈ CAC / (ARPA × gross margin %)
```

The widely-cited SaaS venture heuristic — associated with SaaS-metrics
posts from Bessemer, David Skok, and a16z — is **payback < ~12 months**
as a signal that the growth engine self-funds within a reasonable
horizon.
<!-- needs-research: primary-source citation for the "<12 months payback" benchmark — commonly attributed to Bessemer's SaaS metrics posts and a16z's B2B SaaS analyses; specific origin varies by source. Add authoritative URL. -->

**Why payback matters even when LTV:CAC is healthy.** LTV:CAC tells
you whether the eventual math works. Payback tells you *how much
capital you need in the meantime*. A business with 4× LTV:CAC and
36-month payback needs three years of gross-margin dollars per
customer to break even on that customer's acquisition — during which
you're funding the gap out of your last raise. A business with 4×
LTV:CAC and 9-month payback funds its own next customer inside a
year and burns much less.

**Landmarks around 12 months:**

- **< 12 months**: fast payback; growth compounds inside a normal
  fundraising cycle. Strong signal.
- **12–24 months**: acceptable if the LTV is durable and the raise
  is sized appropriately. Common range for mid-market SaaS.
- **> 24 months**: only defensible for very-high-LTV businesses
  (enterprise contracts, long expected life, dominant expansion
  motion). At this length, payback is more a strategic assumption
  than a metric.

**Two ways payback misleads.**

- **Segment-blind.** If enterprise CAC is $50k with 24-month payback
  and SMB CAC is $500 with 4-month payback, a blended 14-month
  number hides two totally different economics. Report per-segment
  as soon as you have segment data.
- **Ignores expansion.** A customer whose seat count grows over time
  pays back CAC faster than a static customer at the same starting
  ARPA. Payback formulas that don't credit expansion are pessimistic
  on land-and-expand businesses.

## The heuristics are heuristics, not laws

The three numbers above — 3× LTV:CAC, 12-month payback, LTV formula
with constant churn — are **decision-making heuristics for the SaaS
subscription business shape**. They earn their durability by being
right often enough to be useful, and they mislead in predictable ways
when applied outside that shape.

Four common mis-applications:

- **Transactional / marketplace businesses.** LTV in a marketplace is
  a function of take-rate and repeat-transaction frequency, not
  monthly ARPA. The 3× heuristic can transfer, but the underlying
  LTV formula must be re-derived from the marketplace's own economics.
- **Consumer / freemium.** Free-to-paid conversion, activation, and
  virality change the shape of the CAC calculation entirely (the
  "channel" is the product's own referral loop). Heuristics from
  paid-B2B-SaaS transfer poorly.
- **Enterprise with multi-year contracts.** Prepaid multi-year deals
  make monthly-churn math meaningless during the paid period; use
  cohort retention curves and renewal-rate math instead.
- **Very-early-stage numbers.** With 15 customers and 4 months of
  data, any calculated LTV or churn number has confidence intervals
  wider than the number itself. Report the number, but treat it as
  directional; the heuristic ranges apply to *models built on
  meaningful data*, not to arithmetic dressed up as one.

The correct way to use the heuristics at IDEA→PRE-SEED: **treat them
as thresholds your projected model should clear, and check whether the
inputs that produce that clearance are the ones you can most credibly
defend.** A 5× LTV:CAC that requires an assumed 1% monthly churn on a
segment you've never tested is not a strong number; a 2.5× LTV:CAC
grounded in observed retention from real design partners is.

## Reading the four inputs against the derived metrics

The value of the derived metrics is diagnostic. When one of them falls
below the heuristic threshold, you know *which raw input to attack*:

- **LTV:CAC too low → CAC too high.** Fix by finding a working channel
  (chapter 05's riskiest-assumption territory) or by raising price.
- **LTV:CAC too low → LTV too low.** Fix by extending lifetime (reducing
  churn) or by improving gross margin (reducing per-account variable
  cost, especially inference cost).
- **Payback too long → CAC too high or ARPA × margin too low.** Fix by
  compressing the sales cycle, raising price, or removing variable cost
  per unit.

A model where you can't diagnose which input to attack is a model that
hasn't done its job.

## Summary

- **LTV** is *gross-profit* lifetime value: `ARPA × gross margin ÷
  monthly churn`. Revenue-based LTV overstates low-margin businesses;
  always include the margin term.
- **LTV : CAC > 3×** is the widely-cited SaaS heuristic for scaling
  paid acquisition. Below 1× you lose money per customer; between 1×
  and 3× you break even but don't compound.
- **CAC payback < ~12 months** is the SaaS venture heuristic for a
  self-funding growth engine. It catches cash-timing problems that
  LTV:CAC is silent on.
- **All three are heuristics for the paid-B2B-SaaS shape**, and they
  transfer poorly to marketplaces, consumer, enterprise multi-year,
  and pre-data early-stage. Use them to *point at which input to
  attack*, not as laws.

**Next:** the discipline that keeps the whole sheet honest — naming
the single input that, if wrong, kills the model, and designing the
cheapest experiment to test it — in
[chapter 05](./05-riskiest-assumption-experiment.md).
