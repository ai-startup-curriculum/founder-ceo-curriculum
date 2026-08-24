---
stage: SEED
stages: [PRE-SEED, SEED, SERIES-A]
pillar: finance
requires: [mod-002-lean-business-modeling]
role_pathways: [founder-ceo, startup-finance-fundraising]
---

# Module 003 — Runway & Financial Modeling

> **Stage:** SEED · **Pillar:** Finance · **Prereq:** mod-002

## Why this module

Your canvas and unit economics said the business *could* work. This module is
where you find out how long you have to prove it. Every downstream decision — who
to hire, when to raise, what to cut, whether to keep going — reduces to three
numbers: **cash on hand, monthly burn, and the runway that falls out of the
two**. A founder who can't state those from memory is flying blind.

The most expensive mistake at this stage is *discovering* your runway instead of
*deciding* it. Founders who don't model their spend end up on a schedule set by
their bank balance: hiring in the good months, panic-cutting when the number
gets scary, starting to raise the month they realize they should have started
six months ago. A model is how you get in front of the calendar instead of
chasing it.

The operating plan is not a forecast — it will be wrong. Its job is to make the
**cost of being wrong visible in advance**, so that when reality diverges from
the plan (it will), you already know which lever to pull.

## Learning objectives

After this module you can:

1. Compute and state, from memory, the three founder numbers — **cash, net
   burn, runway** — for a given month, and explain the difference between
   *gross* and *net* burn.
2. Build an **18-month operating model** that ties headcount, spend, and (if
   any) revenue to a month-by-month cash balance, and identify the **zero-cash
   date**.
3. Model the impact of a **hiring decision** (fully-loaded cost, ramp lag,
   knock-on costs) on burn and runway *before* making the offer.
4. Apply Paul Graham's **default-alive vs default-dead** test to decide whether
   the next move is to raise, cut, or grow into profitability.
5. Identify the **decision points** on the runway curve — the "raise by,"
   "cut by," and "kill by" months — and what evidence would change them.

## Core concepts

### 1. The three founder numbers

Every operating founder should be able to answer these three questions without
opening a spreadsheet:

- **Cash on hand** — the dollars in your bank account today. Not committed
  spend, not receivables, not a promised wire from a signed SAFE that hasn't
  cleared. Cash is only cash when it's in the account.
- **Monthly burn** — how much cash you're consuming per month. Two flavors,
  and the distinction matters:
  - **Gross burn** — total monthly cash out (payroll, rent, tools, hosting,
    contractors, everything).
  - **Net burn** — gross burn minus cash *in* (customer revenue that actually
    hits the account). Net burn is the number that determines runway.
- **Runway** — how many months until cash hits zero at current net burn.
  The simplest form is `cash on hand / net burn`. If you have $310k in the
  bank and net burn is $42k/month, runway is `$310k / $42k ≈ 7.4 months`.

The simplest form assumes burn stays constant. It rarely does. That's why you
build a model.

### 2. Gross vs net, and the trap of "we'll make it up in revenue"

Runway math is honest only if you're honest about which burn number you're
using. Early-stage founders often quote **net burn** ("we're only burning $28k
a month") when their gross burn is $42k and they're leaning on customer
revenue that hasn't landed yet, might churn, or is a one-time deal.

Two disciplines that keep this honest:

- Report **both** numbers in board updates and internal reviews. Gross burn
  tells you what the business costs to operate; net burn tells you how much
  the customers are subsidizing that cost this month.
- Recompute runway on **gross burn** as a stress test. If revenue disappears
  for a quarter (a churned anchor customer, a delayed contract), how long do
  you have? That's your real floor.

### 3. Headcount is the dominant lever

At seed stage, **people are usually 70–85% of cash burn** — payroll dwarfs
tools, hosting, and rent combined. That makes headcount the single most
consequential decision in the model.

The number to plan against is not the salary; it's the **fully-loaded cost**
of a hire. A rough US-market rule of thumb is **base salary × ~1.25–1.4** to
cover employer payroll taxes, benefits, equipment, software, and overhead — so
a $180k engineer costs closer to **$220k–$255k/year** in actual cash out.
Exact loading varies by country, benefits generosity, and remote/office mix,
so build the number from your own line items rather than trusting the
multiplier blindly.
<!-- needs-research: primary-source citation for the "1.25–1.4× fully-loaded cost" multiplier — commonly cited by MIT and SBA guidance but the exact ratio is context-dependent (benefits generosity, country, remote/office). -->

Two more things the naive salary number misses:

- **Ramp lag.** Hiring is not instant. From "we need someone" to "they start"
  is typically 6–12 weeks for engineers, longer for senior specialists. From
  start to fully productive is another quarter or two. A hire made in
  January often doesn't move a metric until Q2 — but the payroll starts on
  day one.
- **Knock-on costs.** Each new hire pulls management time from the founder,
  adds tooling seats, and (past a certain size) forces a step function in
  HR, finance, and legal support. The tenth hire is more than 10× the cost
  of the first.

### 4. The operating model — what it is and isn't

An **operating model** is a month-by-month spreadsheet with three sections:

1. **Cash in** — revenue by month (contracts signed × billing cadence),
   plus one-time cash events (funding rounds, grants, refunds).
2. **Cash out** — payroll (per person, per month, fully loaded), plus
   non-payroll spend (hosting, tools, rent, contractors, legal).
3. **Cash balance** — starting cash + cumulative net cash flow, month by
   month. The month this line crosses zero is your **zero-cash date**.

A useful operating model has three properties:

- **Every input is a named assumption.** Not "$18k/mo in revenue" but "6
  customers × $3k ARPA, holding flat." The named assumption is what you
  update when reality changes.
- **The hires are on the calendar.** Not "we'll hire 4 engineers this year"
  but "Engineer #3 starts March 1; Engineer #4 starts June 1." The month of
  the offer is when burn changes.
- **The zero-cash date is visible.** Highlight the month cash goes negative.
  Every decision — raise, cut, hire, launch — is a decision about *this
  cell*.

What it isn't: a forecast anyone should believe. Revenue in month 12 is a
guess. The plan's job is to make the *cost of being wrong* visible early
enough to act.

### 5. Default alive vs default dead

Paul Graham's essay *Default Alive or Default Dead?* (October 2015) frames
the central seed-stage question: **at your current growth rate and cost
trajectory, will you reach profitability before you run out of money?** If
yes, you're **default alive** — you have optionality, and a raise is a
choice, not a rescue. If no, you're **default dead** — the current trajectory
ends with the company failing, and something has to change (faster growth,
lower burn, more cash, or a smaller ambition).

The test isn't a snapshot; it's a projection. You draw the growth curve
forward, draw the cost curve forward, and see which one wins first — cash
running out, or revenue crossing burn.

Two operational implications:

- **Default-alive founders raise from strength.** They can walk away from a
  bad term sheet because they don't need the money.
- **Default-dead founders should know it earlier than they usually do.** The
  useful action isn't optimism; it's honest arithmetic and a plan (cut, pivot,
  or accelerate raise).

<!-- needs-research: link to the primary Paul Graham essay at paulgraham.com/aord.html for canonical citation. -->

### 6. What a raise buys you

A round buys **time to hit the next milestone** — nothing more. Two rules
of thumb worth internalizing:

- **Target 18–24 months of runway post-close.** Less than 12 and you'll be
  raising again as soon as the ink dries. More than 30 and you're probably
  over-diluted or under-ambitious for the check.
  <!-- needs-research: primary-source citation for the 18–24 month post-raise runway norm; widely repeated in YC and Sequoia guidance but exact origin varies. -->
- **Start raising 6–9 months before zero cash.** Seed and Series A processes
  routinely take 3–6 months from first meeting to money in the bank, and you
  need slack for a "no" from your top choice. Starting at 3 months of runway
  means raising from weakness — investors can smell it, and terms reflect it.

A raise does not fix a broken business model. If unit economics don't work
(mod-002), more cash just buys a longer, more expensive version of the same
failure. The right question before a raise is: *what specifically will 18
months of runway let us prove that we can't prove now?*

### 7. Decision points on the runway curve

A good operating plan doesn't just show the zero-cash date — it marks the
**decision months** in advance:

- **The "raise by" month.** Six to nine months before zero cash. If you
  haven't started fundraising by then, you're now raising from weakness.
- **The "cut by" month.** The month after which cutting spend can no longer
  extend runway meaningfully (severance costs, wind-down costs, and the lag
  between deciding to cut and cash actually stopping mean you can't wait
  until month 11 to reduce burn in month 12).
- **The "kill by" month.** The point at which continuing costs more than
  winding down — including honoring severance, closing contracts, and
  returning any refundable cash. Founders almost always identify this too
  late.

Naming these months in advance is what separates a model from a spreadsheet.
The model tells you *when* the decision has to be made, so it doesn't get
made *for* you by the bank balance.

## The exercise

Build an 18-month operating plan for a founder with **$310k in the bank,
$42k/month current burn, and a plan to hire two engineers**. Produce a
month-by-month cash model, a post-hire burn number, a zero-cash date, and a
named set of raise/cut decision points. See
**[exercise-01-eighteen-month-operating-plan](./exercise-01-eighteen-month-operating-plan)**.

## Live-lab note

If you're an operating founder using this as a live lab: build the model on
**your** current bank balance, **your** current payroll, and **your** actual
hiring pipeline. The scenario numbers are calibrated to a realistic pre-seed
situation, but the point of the exercise is a plan for a real business —
yours or the simulated one — not an academic sheet.

## Further reading

- Paul Graham, *Default Alive or Default Dead?* (October 2015) — the canonical
  framing of the seed-stage central question.
- Y Combinator, *A Guide to Seed Fundraising* — includes runway-length and
  timing norms for founders raising their first institutional round.
- David Sacks, *The SaaS Adventure* — dashboards and metrics that turn a
  static operating model into an ongoing instrument.
- Brad Feld & Jason Mendelson, *Venture Deals* — the mechanics of a round and
  what different runway targets imply for dilution and control.
- Bill Janeway, *Doing Capitalism in the Innovation Economy* — the longer
  argument for why cash-cycle discipline is what separates surviving startups
  from clever ones.

> ⚠️ AI-assisted content under ongoing human review. Cross-reference primary
> sources; this is a learning resource, not advice for a specific situation.
