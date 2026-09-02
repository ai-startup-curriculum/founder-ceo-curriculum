# Chapter 05 — The Riskiest Assumption: Naming It and Testing It Cheaply

> **Reads with:** module objective 5 — *identify the single riskiest
> assumption in the model — the load-bearing bet that, if wrong, kills
> the business — and design the cheapest experiment that would tell you
> whether it holds.*

## Every canvas is a stack of assumptions

A filled lean canvas plus a unit-economics sheet is a **stack of
assumptions**. Some are safe: people use email, credit cards work,
software can be deployed to the internet. If those assumptions are
wrong, you have bigger problems than your startup. Some are testable
but low-consequence: whether the button on the pricing page is blue or
green will not decide the business. And one or two are **load-bearing**:
if they're wrong, nothing downstream matters.

The founder's most valuable move at IDEA→PRE-SEED is separating the
load-bearing assumptions from the rest, naming the *single* riskiest
one, and designing the cheapest experiment that would tell them
whether it holds. The rest of this chapter is that discipline.

This is the practical form of Eric Ries's **validated learning** —
*The Lean Startup* (2011) — and the direct descendant of Steve Blank's
customer-development idea that startups exist to **discover an untested
model**, not to execute a known one.
<!-- needs-research: primary-source citations for The Lean Startup (Ries, 2011) and The Four Steps to the Epiphany / The Startup Owner's Manual (Blank, 2005 / 2012). -->

## What "load-bearing" means

An assumption is load-bearing when *its failure alone* kills the
business — no adjacent tweak recovers the model. Two properties define
it:

- **Consequence.** If it comes in half of what you assumed, the
  numbers on the sheet don't work. Not "the model is stressed" —
  they don't work.
- **Uncertainty.** You genuinely don't know if it's true. If you have
  strong evidence one way or the other, it's not the riskiest bet;
  something else is.

An assumption that's high-consequence but well-evidenced is not the
riskiest — you've already tested it. An assumption that's uncertain
but low-consequence isn't either — it doesn't matter what the answer
is. The intersection is where the load-bearing bet lives.

## The four assumptions that are usually load-bearing at IDEA→PRE-SEED

Across most first-time founder situations, one of four assumptions
turns out to be the load-bearing bet.

### 1. Willingness to pay

*They will pay $X/mo for this outcome.*

The most common load-bearing assumption. Discovery in mod-001 tests
whether the *problem* is real; it usually does not close a *price*.
A founder can leave discovery certain the pain is severe and still be
wrong about how much a buyer will trade for it — pain does not
mechanically translate into budget. The right test is a real
price-based commitment (a signed pilot, a Stripe transaction, a
credit card on file for a beta) rather than a stated intent.

### 2. A working channel

*You can reach the segment for less than they're worth.*

The second most common. A great product on a broken channel is a dead
product; there is no product-quality lever that recovers a business
whose CAC exceeds LTV, no matter how much users love it. The test is
whether at least one channel — outbound, paid, community, content,
partnership — can reliably produce segment-fit conversations at a cost
per conversation that scales into a CAC below LTV.

### 3. Retention

*They still use it in month 3.*

The third. A high-conversion product that customers churn out of in
30 days is not a subscription business; the LTV formula collapses to
one month of margin. The test is a real retention curve on a real
cohort, even if the cohort is small (5–15 design partners is enough
to see if the shape is a cliff or a plateau).

### 4. Cost to serve

*The gross margin holds at scale.*

The one that catches a specific class of business: **AI products with
per-request inference costs**, marketplaces with unfavourable take-rate
economics, hardware-with-software plays, and anything with a large
per-account third-party dependency. The test is running the product at
realistic usage volumes for a small handful of paying customers and
measuring actual per-account variable cost against the ARPA target.

## Naming your riskiest assumption

The mechanical procedure:

1. **List every assumption on the canvas and the unit-economics sheet.**
   Every line item; every block. Ten to twenty lines is normal.
2. **Rate each on consequence and uncertainty**, high or low. A
   two-by-two.
3. **Circle the high-consequence, high-uncertainty cell.** Usually
   two or three assumptions land here.
4. **Pick the single one whose failure would kill the business
   fastest and hardest.** Ties are broken by "which one, if we're
   wrong, would we not be able to recover from with any adjacent
   pivot."

Write it as one sentence, in the form:

> *"The business fails if [assumption] is wrong, because [downstream
> consequence]. We would notice it's wrong if [observable signal]."*

Example:

> *"The business fails if first-time technical founders are unwilling
> to pay $99/mo for a structured curriculum, because our discovery
> insight was about need, not about budget, and every channel and
> retention assumption downstream assumes a paying customer. We would
> notice it's wrong if a smoke-test landing page with a $99 checkout
> converts below 1% of segment-fit visitors, or if design partners
> refuse to convert from free access to paid access at month 3."*

If you can't write that sentence, you don't yet know your riskiest
assumption. Keep reducing.

## The cheapest-experiment principle

Once the assumption is named, the design principle is: **the cheapest
experiment that would meaningfully change your belief is the right
one**. Cheap means dollars, days, and calendar.

Two subordinate rules.

### Rule 1: The product is the most expensive experiment.

Building the product to test the assumption is almost always the
wrong test, because it takes the longest and costs the most, and if
the assumption fails you've spent months learning something a
landing page could have told you in a week. Reserve the product build
for after the load-bearing bets have held up under cheaper tests.

### Rule 2: A pass condition must be defined in advance.

An experiment without a pre-declared pass/fail rule is not an
experiment — it's a demo you'll rationalise afterwards. Define
"this passes if X happens; this fails if Y happens" *before* you
run it. If both X and Y feel like acceptable outcomes when you write
them down, the experiment isn't sharp enough.

## A menu of cheap experiments matched to load-bearing assumptions

Different load-bearing assumptions call for different experiments.
The mapping is not unique — often two experiments can test the same
assumption — but the ranges below are a useful default menu.

### For willingness-to-pay

- **Landing page + paid-ad smoke test.** A one-page site describing
  the UVP, an explicit price, and a "join the beta" / "buy now"
  checkout button. Drive segment-fit traffic through 2–3 paid ad
  variants. Success signal: a defensible conversion rate to
  checkout-attempt from segment-fit visitors. Cost: a lunch, plus
  ad spend in the low hundreds of dollars for enough data.
  <!-- needs-research: primary-source citation for smoke-test / landing-page validation as a discovery method — commonly associated with Alberto Savoia's Pretotyping and Ash Maurya's Running Lean. -->
- **Letter-of-intent / signed pilot.** For enterprise / higher-ACV
  buyers, ask 3–5 discovery contacts to sign a paid pilot LOI at
  the target price. Success signal: at least two sign.
- **Concierge MVP at price.** Deliver the outcome manually, behind
  the scenes, at a real price, to 3–5 buyers. Success signal: they
  pay a second time.

### For a working channel

- **50-target cold outbound test.** One channel (LinkedIn DM,
  cold email against a public signal, a targeted community post).
  Success signal: a plausible funnel — response rate × book-a-call
  rate × qualified-conversation rate — that projects to a
  channel-CAC below LTV at scale.
- **Search-intent-keyword ad test.** For a channel that maps to
  buyer search intent. Success signal: cost-per-click and
  click-to-signup rates that yield a plausible CAC.
- **Community-post test.** Post one genuine, non-promotional piece
  in a segment community and measure reply / DM / follow rate.
  Success signal: at least two segment-fit conversations arise
  organically.

### For retention

- **Design-partner cohort with weekly usage capture.** 5–15 real
  users on a working prototype (or a concierge equivalent) for 8–12
  weeks. Success signal: the retention curve plateaus, not cliffs;
  active use in week 8 for at least half the cohort.
- **Manual re-engagement check-in.** Not an experiment on the
  product — an experiment on whether the *need* recurs. Success
  signal: buyers want the follow-up call, or bring their own
  agenda.

### For cost to serve

- **Real-usage-load pilot.** Run 3–5 paying customers on production
  infrastructure at realistic volumes for a full billing cycle.
  Measure per-account variable cost. Success signal: gross margin
  clears the target on the sheet. This is the test class most
  founders skip and most AI-product founders regret skipping.
- **Cost model with published-price inputs.** For pre-launch
  products, model per-account cost against published API prices,
  observed inference token counts, and observed session shapes.
  Not a substitute for a real-usage pilot, but useful as an
  order-of-magnitude sanity check before you commit engineering
  time.

## Ordering: cheapest first, product build last

The right sequencing of experiments is by **cost of running the test**,
not by **which is most interesting**. The intuition is Bayesian:
information is most valuable when you have the least of it, and cheap
tests give you meaningful information per dollar early in the process
when your beliefs are widest. Expensive tests earn their keep after
the model has been narrowed enough that only they can add signal.

A defensible sequencing at IDEA→PRE-SEED:

1. **Landing-page smoke test** for willingness-to-pay. Days.
2. **Cold-outbound / paid-ad channel test.** One week.
3. **Concierge / manual MVP** with 3–5 paying design partners.
   Two to six weeks.
4. **Real-usage pilot on production infra** for cost-to-serve.
   One billing cycle.
5. **Full product build** for the design-partner cohort. Only after
   1–4 have not disqualified the model.

Founders who invert this order — building the product first and
testing the assumptions afterward — spend most of a round learning
things a landing page would have told them in three days.

## Writing the assumption call

The output of this chapter is one paragraph in the canvas artifact —
call it the **riskiest-assumption call**. It has four parts:

- **The single assumption**, one sentence, in the form above.
- **Why it's the riskiest**: the two-property test (consequence,
  uncertainty).
- **The cheapest experiment**, one sentence.
- **The pass/fail condition**, pre-declared.

That paragraph is the input to exercise 02 in this module and, at the
right scale, becomes a recurring cadence: every meaningful shift in
the model produces a new riskiest-assumption call and a new
experiment. Discovery ends; assumption-testing does not.

## Summary

- Every filled canvas is a stack of assumptions; **one or two are
  load-bearing** (high-consequence, high-uncertainty).
- The four most common load-bearing bets at IDEA→PRE-SEED are
  **willingness to pay, a working channel, retention past month 3,
  and cost to serve**.
- Name the single riskiest bet in one sentence, then **design the
  cheapest experiment** that would tell you whether it holds — with
  a pre-declared pass/fail condition.
- **The product build is the most expensive test**; use it last, not
  first. Landing pages, cold outbound, concierge MVPs, and
  real-usage pilots earn their keep earlier.

**Next:** the sanity check that keeps the whole model tethered to a
real market — bottom-up sizing — in
[chapter 06](./06-bottom-up-market-sizing.md).
