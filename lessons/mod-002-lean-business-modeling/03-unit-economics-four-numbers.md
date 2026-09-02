# Chapter 03 — Unit Economics: The Four Core Numbers

> **Reads with:** module objective 3 — *build a first unit-economics sheet
> naming and defending the four core numbers — CAC, ARPA/ARPU,
> gross/contribution margin, churn — with the founder-time trap in CAC
> called out.*

## What a unit-economics sheet answers

The canvas describes the model qualitatively. The unit-economics sheet
answers the two questions the canvas can't: **does one customer make you
money, and how quickly?** Every downstream financial artifact — the
operating plan (mod-003), the fundraising narrative (mod-004), the
sales-motion economics (mod-006) — is a scaled-up version of a
per-customer answer that lives here.

At IDEA→PRE-SEED you almost certainly do not have real numbers for any
of these inputs. That is fine. **The purpose of the sheet now is not to
be accurate; it is to be explicit.** Every input is either a source or
a marked assumption, and every derived number is a formula you could
show a skeptic. Wrong-but-explicit is far better than right-but-vague:
wrong-but-explicit shows you which input, if it comes in half of what
you guessed, breaks the business (see chapter 05).

## The four numbers, one at a time

Four inputs sit at the base of every unit-economics sheet.

### 1. CAC — Customer Acquisition Cost

**Definition:** total sales-and-marketing spend over a period, divided
by new customers acquired in that period.

```
CAC = (sales + marketing spend in period) / (new customers acquired in period)
```

Two design choices matter more than the formula.

**Choice A — which channels count.** The strictest version is
**paid CAC**: only spend attributable to paid channels, divided by
customers attributable to paid channels. The most honest version at
this stage is **blended CAC**: all sales and marketing spend, divided
by all new customers, across all channels. Paid CAC flatters the model
by hiding the organic-and-founder-time engine that's actually working.
Blended CAC is uglier and truer.

**Choice B — which time-window.** Use the same window for spend and for
customers acquired. If your marketing spend in Q1 produces customers in
Q2, either extend the window or you're going to report a CAC of zero
one quarter and infinity the next. For a subscription business at
early stage, a **rolling 90-day window** usually behaves.

### The founder-time trap in CAC

The single most common way founders lie to themselves about CAC is by
not counting their own time.

"Free" channels aren't free. A cold-outbound sequence, a content post,
a warm intro, a demo call — every one of those is founder-time. If your
CAC formula has founder time at zero, then any "free" channel makes CAC
look great, and the model appears to work at any price point. The moment
you try to scale (by hiring an SDR, an AE, or a content writer) that
zero becomes a real payroll number, and CAC quadruples overnight — the
model was never actually working; the founder was subsidising it with
uncompensated labour.

The fix: **value founder time at a fair-market replacement rate** — the
salary you'd pay to hire the person who would eventually take over that
work — and put those hours into CAC as a real cost. If you'd hire an
AE at $120K on-target-earnings to do the demo calls you're doing now,
then the demo calls cost roughly $60/hour of loaded time. Ten founder
demo-hours per closed customer, at that rate, is $600 of CAC before any
paid spend, before any onboarding, before any tooling.

This is not accounting-purity for its own sake. It's the difference
between knowing whether you have a business or a subsidy — and the
subsidy is running on a resource (your calendar) that has a hard cap
and no fungibility with capital.

### 2. ARPA / ARPU — Average Revenue Per Account/User

**Definition:** the revenue a typical customer pays per period.

```
ARPA = total recurring revenue in period / active accounts in period
```

For SaaS, the standard reporting cadence is monthly (**MRR-based
ARPA**); for annual-contract SaaS, annual (**ARR-based ARPA**). Pick
one and stay consistent — mixing monthly and annual bases silently
inflates or deflates every downstream number.

Two clean-up rules:

- **Exclude one-time fees** (setup, implementation, professional
  services) from ARPA unless the customer contract *guarantees* they
  recur. One-time revenue is real cash but is not a subscription
  input; treating it as ARPA overstates LTV.
- **Exclude paused or free accounts** from the denominator unless
  they meaningfully convert on a predictable timeline. A free-tier user
  is not an "average account."

ARPA differs from **ARPU** (per user) in seat-based products: an
account with 20 seats at $10/mo has ARPA of $200 and ARPU of $10.
Pick the unit that matches how you sell — accounts if you sell to
organisations, users if you sell to individuals. Don't average across
both.

### 3. Gross margin / contribution margin

**Definition:** revenue minus the *variable* cost to serve that
customer, expressed as a percentage of revenue.

```
gross margin % = (ARPA - variable cost per account per period) / ARPA
```

Variable costs are anything that scales with the number of customers:

- **Hosting and infrastructure** attributable to serving the account
  (compute, storage, bandwidth, per-request LLM inference costs).
- **Third-party APIs and per-seat SaaS you resell** (data providers,
  payment processing, embedded services).
- **Direct customer-support cost** if it scales per-account (a CSM
  quota of 30 accounts implies real per-account cost; a self-service
  product has near-zero).

The distinction from **contribution margin** is subtle: contribution
margin includes *all* variable costs, including variable sales cost
(commissions, per-close bonuses); gross margin conventionally excludes
sales cost. In practice, for early-stage founders, use gross margin
and be explicit about whether you've folded sales commission in. The
purpose is not GAAP compliance; the purpose is to know how much of
each revenue dollar remains after the direct cost of delivering it.

**Why this matters more than founders expect.** A dollar of revenue
at 20% margin is not the same business as a dollar at 80%. A pure-SaaS
company routinely runs 75–85% gross margin. An AI product with
per-request LLM inference costs can run 20–40% depending on model
choice, caching, and usage patterns. A services-heavy hybrid runs
50–65%. Ignoring margin and computing everything from revenue *lets
you flatter a low-margin business into looking like a SaaS business*
until you try to justify a SaaS valuation multiple and the mismatch
gets caught.
<!-- needs-research: primary-source citation for typical SaaS gross-margin ranges — commonly cited from KeyBanc / Bessemer SaaS surveys and OpenView Benchmarks reports. -->

The two most common margin traps at IDEA→PRE-SEED:

- **AI-inference costs treated as fixed.** They're not. Per-token or
  per-request pricing scales linearly with usage. If your typical
  customer runs 100k tokens/day at $X/1M tokens, that is a per-account
  variable cost you must model.
- **Free-tier costs unallocated.** If free users cost real money to
  serve, and only a fraction convert, the *effective* variable cost
  per paid customer includes the free-user overhead they subsidise.
  Ignoring this lets a paid-tier margin look 20 points better than it
  really is.

### 4. Churn

**Definition:** the fraction of customers who leave in a period.

```
monthly logo churn = customers lost in month / customers at start of month
```

Three distinctions that matter:

- **Logo churn vs revenue churn.** Logo churn counts customers who
  cancel. Revenue churn counts dollars that walk out. In a segmented
  book (some big customers, many small), losing your biggest logo can
  be 3% logo churn and 20% revenue churn. Report both.
- **Gross vs net revenue churn.** Gross revenue churn counts only
  losses. Net revenue churn subtracts *expansion* revenue (upsells,
  seat additions) from losses; a healthy SaaS book with strong
  expansion can have **negative** net revenue churn, meaning the
  average existing customer grows faster than churn erodes.
- **Time to measure.** A three-month-old company can't defensibly
  report annual churn. State the window and the sample size honestly;
  a churn rate computed on 12 customers is directional, not a metric.

For a rough LTV approximation, **`1 / monthly churn` is the average
customer lifetime in months** — the geometric-series result assuming
constant churn each month. That assumption is wrong (early churn is
almost always higher than late churn), so the resulting lifetime is
optimistic. Treat it as a first-pass number; a cohort curve is more
honest once you have data.

## The sheet as a whole

Written out, the four inputs and the derived numbers they produce:

```
Inputs (cite source or mark ASSUMPTION):
  ARPA (avg revenue per account, $/period)     :
  Variable cost per account per period ($)     :
  Gross margin % = (ARPA - variable cost)/ARPA :
  Monthly churn rate (%)                       :
  Avg customer lifetime (months) ≈ 1/churn      :
  CAC ($, blended, founder time included)      :

Derived (chapter 04 covers these):
  LTV ≈ ARPA × gross margin % × avg lifetime   :
  LTV : CAC                                    :
  CAC payback (months) ≈ CAC / (ARPA × margin) :
```

Every input line carries a **source** or the label **ASSUMPTION**. At
IDEA stage, most lines are ASSUMPTION and that is fine. What matters
is that you know which ones. When you fill this from real data six
months later, the lines that flipped from assumption to evidence, and
the ones that came in worse than assumed, are exactly the input to
the pivot conversation.

## The four common wrong versions

Four ways this sheet gets built wrong, in decreasing order of frequency:

- **CAC excludes founder time.** Covered above. The most consequential
  distortion at this stage.
- **LTV computed on revenue, not margin.** ARPA × lifetime, no margin
  multiplier. A 20-margin business looks like an 80-margin business at
  5× the actual value. Chapter 04 walks through the correct formula.
- **Churn measured on too small a sample.** "Our churn is 2%" on 15
  customers means "one person cancelled and we called that a rate."
  State the sample size and window.
- **ARPA computed with one-time fees folded in.** Setup and pro-services
  revenue inflates the recurring number and every downstream ratio.

## Summary

- The four core numbers — **CAC, ARPA/ARPU, gross margin, churn** —
  define whether one customer makes you money. Every downstream
  finance artifact scales up from here.
- **CAC must include founder time** at a fair-market replacement rate.
  Zero-cost founder hours are the biggest single lie in early-stage
  unit economics.
- **ARPA excludes one-time fees**; report on a consistent monthly-or-
  annual base.
- **Gross margin, not revenue,** drives LTV. A low-margin business is
  not the same business as a high-margin one at the same revenue.
- **Churn** distinguishes logo from revenue, gross from net; a rate
  computed on 12 customers is directional, not a metric.

**Next:** the derived metrics — LTV, LTV:CAC, and CAC payback — and
the SaaS heuristics that decide whether the model is fundable, in
[chapter 04](./04-ltv-cac-payback-heuristics.md).
