---
stage: PRE-SEED
stages: [IDEA, PRE-SEED]
pillar: strategy
requires: [mod-001-customer-discovery]
role_pathways: [founder-ceo, startup-product-gtm]
---

# Module 002 — Lean Business Modeling & Unit Economics

> **Stage:** IDEA→PRE-SEED · **Pillar:** Strategy / Economics · **Prereq:** mod-001

## Why this module

Discovery told you a problem is real. A **business model** is your bet on *how the
company that solves it makes money and survives*: who it's for, how they find you,
what you charge, what it costs to deliver, and what one customer is worth compared
to what one customer costs. Every downstream module — runway, fundraising, sales
— reduces to numbers that live on this page.

A model is not a plan; it's an **explicit set of assumptions you can test**. The
canvas exists so that the assumptions are visible, one place, and small enough to
attack one at a time. Unit economics exists so that when you scale, you scale a
business, not a subsidy.

The most expensive mistake at this stage is a model that only works if a single
heroic number — a magic CAC, a magic conversion rate, a magic price — comes in.
The point of this module is to find that number **before** you spend a round
chasing it.

## Learning objectives

After this module you can:

1. Turn discovery findings into a **lean canvas** — problem, customer segments,
   unique value proposition, solution, channels, revenue streams, cost structure,
   key metrics, and unfair advantage — with each block traceable to evidence, not
   opinion.
2. Build a first **unit-economics sheet** that states, per customer: what they
   cost to acquire (CAC), what they're worth over time (LTV / contribution
   margin), and how long until they pay you back (CAC payback period).
3. Identify the **single riskiest assumption** in the model — the one that, if
   wrong, kills the business — and design the cheapest experiment that would tell
   you whether it holds.

## Core concepts

### 1. Lean canvas vs. business model canvas

The **Business Model Canvas** (Alexander Osterwalder, *Business Model Generation*,
2010) is the nine-block reference for describing any business — well-suited to
established companies mapping what they already do. **Ash Maurya's Lean Canvas**
(*Running Lean*, O'Reilly) adapts it for early-stage startups by replacing four
blocks that presume you already have a business (Key Partners, Key Activities,
Key Resources, Customer Relationships) with four that matter when you don't:
**Problem**, **Solution**, **Key Metrics**, and **Unfair Advantage**.

Use the lean canvas at this stage. It forces you to write down the problem *first*
and treat the solution as one of many possible bets — which is the discipline
mod-001 exists to build.

### 2. The nine blocks (and the order to fill them)

Fill in **problem-first**, not left-to-right. The Ash Maurya recommended order:

1. **Customer Segments** — who exactly, with an **early adopter** carve-out. Not
   "SMBs"; *"seed-stage two-person technical teams who ship weekly."*
2. **Problem** — top 1–3 problems this segment has, plus **existing alternatives**
   (spreadsheets, competitors, doing nothing). Ripped straight from discovery.
3. **Unique Value Proposition** — the single-sentence promise. The test: it
   sounds specific, it's aimed at the segment, and it names the *finished-story*
   outcome, not a feature list.
4. **Solution** — the smallest thing that would deliver the UVP. One line each,
   mapped 1:1 to the problems.
5. **Channels** — how you reach the segment. Free vs. paid; inbound vs. outbound.
   Founders under-invest here; a great product on a broken channel is a dead
   product.
6. **Revenue Streams** — pricing model, willingness to pay, lifetime value.
   Charging for the thing is a discovery instrument, not just a monetization step.
7. **Cost Structure** — customer acquisition cost, distribution cost, hosting,
   people, anything that scales with the business.
8. **Key Metrics** — the small set of numbers that tell you the model is working
   (activation, retention, referral, revenue — pick the few that matter *now*).
9. **Unfair Advantage** — something a competitor can't easily copy or buy.
   Networks, proprietary data, hard-won regulatory positions, distribution.
   *Not* "we work harder" or "our team is great." If this box is empty, that's a
   real finding, not a failure of the exercise.

The canvas should fit on one page. If yours doesn't, you're describing, not
choosing.

### 3. Unit economics: the four numbers

A unit-economics sheet answers: **does one customer make you money, and how
quickly?** The four numbers you must be able to name and defend:

- **CAC** (Customer Acquisition Cost) — total sales + marketing spend over a
  period, divided by new customers acquired in that period. Founder-time counts;
  free channels aren't free.
- **ARPA / ARPU** (Average Revenue Per Account/User) — what a typical customer
  pays per period (usually per month for SaaS).
- **Gross margin / contribution margin** — revenue minus the *variable* cost to
  serve that customer (hosting, payment fees, support-per-seat, third-party APIs).
  A dollar of revenue at 20% margin is not the same business as a dollar at 80%.
- **Churn** — the rate at which customers leave in a period. In a subscription
  business, `1 / monthly churn` is a rough average customer lifetime in months.

From these you derive:

- **LTV** (customer lifetime value) — for a subscription business, a common
  approximation is `ARPA × gross margin % / churn rate`. The gross-margin
  multiplier matters: LTV computed on revenue overstates a low-margin business.
- **LTV : CAC ratio** — a widely-cited SaaS heuristic (David Skok / *For
  Entrepreneurs*) is **> 3×** to justify scaling paid acquisition. Below 1×,
  you lose money on every customer.
- **CAC payback period** — months of gross-margin dollars needed to earn back
  CAC. A common venture-scale rule of thumb is **< 12 months** for SaaS;
  transactional and consumer businesses vary.
  <!-- needs-research: primary-source citation for the "12 months" payback benchmark; commonly attributed to Bessemer / a16z SaaS posts but exact origin varies. -->

These numbers are heuristics, not laws. Their job is to tell you which one, if
it doesn't hold, breaks the business.

### 4. The riskiest-assumption test

Every canvas is a stack of assumptions. Most of them are safe — they'd have to be
strange for the business to fail on them (people use email, credit cards work,
software can be deployed). One or two are load-bearing: if they're wrong, nothing
downstream matters.

Common load-bearing assumptions at this stage:

- **Willingness to pay** — they'll pay $X/mo for this outcome.
- **A working channel** — you can reach the segment for less than they're worth.
- **Retention** — they still use it in month 3.
- **Cost to serve** — the thing you're building doesn't have a 20% gross margin
  hidden in it (an AI product with large per-request inference costs, for example).

The move is: **name the single assumption that would kill the business if wrong,
then design the cheapest experiment that would tell you.** A landing page and a
paid-ad test can validate a channel and a price point for the cost of a lunch.
Building the product is the *most* expensive test of an assumption; use it last,
not first.

### 5. Sizing the market — a sanity check, not a pitch

At this stage, TAM/SAM/SOM (Total / Serviceable / Serviceable-Obtainable market)
is a sanity check: is there enough here that if the model works, it's a company?
Prefer **bottom-up** sizing (`number of segment members × plausible ARPA`) over
top-down analyst reports. Bottom-up is testable; top-down is decorative.

## The exercise

Turn your mod-001 discovery findings (or the simulated segment) into a **lean
canvas** and a first **unit-economics sheet**, and flag the single riskiest
assumption. See **[exercise-01-canvas-and-unit-economics](./exercise-01-canvas-and-unit-economics)**.

## Live-lab note

If you're an operating founder: do this on your **actual** business this week.
Fill the canvas from your own discovery notes, build the economics sheet with
your real (or best-guess) numbers, and name the assumption you're most afraid to
test. That last one is usually the one worth testing next.

## Further reading

- Ash Maurya, *Running Lean* (O'Reilly, 3rd ed.) — the canonical lean canvas book.
- Alexander Osterwalder & Yves Pigneur, *Business Model Generation* — the original
  Business Model Canvas.
- David Skok, *For Entrepreneurs* blog — canonical SaaS metrics posts on CAC, LTV,
  and the LTV:CAC ratio.
- Steve Blank, *The Startup Owner's Manual* — customer development and business
  model discovery.
- Bill Gurley, *All Revenue is Not Created Equal* — why revenue quality (margin,
  retention, defensibility) matters as much as revenue size.

> ⚠️ AI-assisted content under ongoing human review. Cross-reference primary
> sources; this is a learning resource, not advice for a specific situation.
