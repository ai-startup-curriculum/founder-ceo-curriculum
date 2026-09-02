# Exercise 03 — Fully-Loaded Hire Cost & Ramp-Lag Drill

**Module:** 003 Runway & Financial Modeling · **Stage:** SEED · **Time:**
~2 focused hours · **Prereq exercise:**
[exercise 01](./exercise-01-eighteen-month-operating-plan.md) — you
need the operating model so this drill lands on real cash and runway
numbers, not abstractions. · **Reads with:** chapter
[03](../03-fully-loaded-hire-cost.md).

## Problem statement

Exercise 01 put two engineers on the calendar at a fully-loaded
multiplier. Most founder hiring decisions get made against the
**salary** number rather than the **cost-to-the-company** number,
which is the single most consequential distortion in seed-stage
planning: a $180k engineer is not a $15k/mo burn increase, it's
closer to $19–21k once loading is honest and $21–22k once knock-ons
are included, and the ramp between "start date" and "productive"
is another quarter or two of payroll before contribution begins.

This exercise makes that arithmetic concrete for a *specific hire
you're contemplating*, so that the runway consequence is visible
*before* the offer goes out.

## Deliverable (one artifact)

A **hire-decision memo** — one page — for a single specific role,
containing:

- The **role** (title, level, base salary, expected start month) and
  why you're hiring it.
- The **fully-loaded monthly cost** with the multiplier defended
  either by line-item breakdown or by explicit reference to a
  US-market rule of thumb.
- The **ramp lag**: time-to-start (from decision-to-hire to actual
  start date) and time-to-productivity (from start to full
  contribution).
- The **knock-on costs**: founder-management time, tooling
  step-functions, HR/finance/legal step-functions if applicable.
- The **runway impact** stated in months: what your operating model's
  zero-cash date is before and after this hire, on both net burn and
  gross burn.
- A **go / delay / no-go recommendation** with the specific evidence
  that would change it.

## Scenario

Pick one:

- **Your real next hire.** If you have a specific role you're
  contemplating or have just opened, use it. Real numbers, real
  start month, real defensible reasoning.
- **Simulated.** From the exercise-01 simulated scenario, run the
  drill on **Engineer #2** — planned start month 6, $180k base. The
  question the memo answers is: given the operating model already
  includes this hire, is the timing right? Would it be better to
  pull it forward, push it back, or cancel it in favor of a
  different role?

## Requirements

The memo has to satisfy each of the following:

- **A single specific role.** Not "our next 3 hires." One hire, one
  memo. If you have three you're contemplating, run three memos —
  each stands on its own.
- **Fully-loaded cost computed and defended.** Either an itemised
  line-by-line breakdown (payroll taxes, benefits, equipment,
  software, recruiting-amortised, other) or the rule-of-thumb
  multiplier with a specific defence for why 1.25 / 1.30 / 1.40 fits
  your setup.
- **Ramp lag explicitly stated in two parts.** Weeks to start
  (source: your actual pipeline for the role, or a defensible
  category norm), and weeks/months to full productivity (defensible
  from role type per chapter 03).
- **Knock-on costs named specifically.** Not "there will be some
  overhead" — the specific tools that will step up in tier, the
  specific fraction of founder-time this hire consumes, the
  specific HR / finance / legal step-function if this hire crosses
  the 10, 25, or 50-employee threshold.
- **Runway impact stated in months on both burn numbers.** From your
  operating model's base case, the zero-cash date before and after
  this hire, on both net burn and gross burn.
- **A specific decision.** Go / delay by N months / no-go. Not "we
  should think about it." Every day the memo sits open without a
  decision is a day the runway calendar assumes you already made
  it.

## Starter guidance

**Session 1 (~20 min) — the role and the base.** Write the role
title, level, base salary, and the reason for the hire in 2–3
sentences. Not a job description — the reason: "we need engineer #2
to own the backend so I (founder) can go full-time on GTM," or "we
need a second-in-command engineer because I'm the only one who can
merge to main and it's blocking the team." The reason is what the
runway cost is buying.

**Session 2 (~30 min) — fully-loaded cost.** Read
[chapter 03](../03-fully-loaded-hire-cost.md). Either compute the
loading from your actual per-person cost lines (payroll taxes,
benefits per your broker's quote, equipment, per-seat SaaS, etc.)
and divide by base salary — that's your loading — or defend the
1.25 / 1.30 / 1.40 you're using with a specific reference to your
setup. Multiply base by loading, divide by 12, that's the monthly
fully-loaded cost.

**Session 3 (~30 min) — ramp lag.** Write time-to-start based on
where you are in the pipeline (a signed offer with start-date =
weeks to that date; a role still in interviewing = your typical
pipeline length; a role not yet posted = your typical
post-to-close length). Write time-to-productivity based on the
role's category per chapter 03 (well-scoped IC: 6–12 weeks; role
requiring business learning: 3–6 months; leadership: 6–12 months).
Add them: that's when the hire actually starts contributing at the
level assumed in the operating model.

**Session 4 (~20 min) — knock-ons.** For each of the three
categories from chapter 03: is founder-time increasing (by roughly
how much per week?), are any tool tiers stepping up (name them),
does this hire cross a 10/25/50-employee HR/finance/legal
threshold?

**Session 5 (~20 min) — runway impact and decision.** Look at your
operating model. What's the base-case zero-cash date? Now edit the
model to reflect the hire at the corrected fully-loaded cost —
what's the new zero-cash date on net burn and on gross burn? Is
the delta acceptable given the reason for the hire? Write the
go / delay / no-go call, and the specific evidence that would
change it (e.g., "would push start month 6 → 8 if the fundraise
lead hasn't given verbal by month 4").

## Memo template (fill inline)

```
Role: ___________________________________________________________
Level: __________  Base salary: $______ /yr  Start month: ______
Reason: _________________________________________________________
        _________________________________________________________

Fully-loaded cost:
  Loading multiplier used: ______   defended by:
    (a) line-item breakdown attached, OR
    (b) US-market rule of thumb, defended because ______
  Fully-loaded annual: $______   → monthly: $______

Ramp lag:
  Time-to-start: ______ weeks  (from where I am in pipeline: ______)
  Time-to-productivity: ______ weeks  (role category: ______)
  Total ramp: ______ weeks  (contributes at model-assumed level from
                             month ______)

Knock-on costs:
  Founder-management time added: ~___ hr/wk  at $___/hr loaded
                                 = $______ /mo
  Tooling step-ups (name tools):
    _______________________________________________________ +$___/mo
    _______________________________________________________ +$___/mo
  HR/finance/legal step-function crossed? (10 / 25 / 50 employees):
    _________________________________________________ estimated $___/mo

  Total marginal monthly burn from month ______: $______

Runway impact (from operating model, base case):
  Zero-cash date before this hire: ______ 20__
  Zero-cash date after this hire  : ______ 20__
    On net burn                   : ______ 20__
    On gross burn (stress)        : ______ 20__
  Delta: ______ months

Decision:
  [ ] GO — as planned
  [ ] DELAY — push start month from ______ to ______ because ______
  [ ] NO-GO — kill this hire and instead ______
  Reason: __________________________________________________________
  Evidence that would change this call: ____________________________
```

## Acceptance criteria

You are done — and this exercise has met the module's standard — when
*all* of the following are true:

- [ ] A **single specific role** is named, with a two-to-three
      sentence reason.
- [ ] **Fully-loaded cost is computed** using either an itemised
      breakdown or a defended multiplier (not just base salary).
- [ ] **Ramp lag is stated in two parts** (time-to-start,
      time-to-productivity) with defensible sources.
- [ ] **Knock-on costs are named specifically** — founder time,
      tooling tiers, HR/finance/legal step-functions.
- [ ] **Runway impact is stated in months on both burn numbers**,
      before and after the hire, from your operating model.
- [ ] A **specific go / delay / no-go decision** is made, with the
      evidence that would change it.

## Self-assessment rubric

| Dimension | Weak | Strong |
|---|---|---|
| Cost basis | Base salary used | Fully-loaded, with defended multiplier or line-item breakdown |
| Ramp | "Should be productive quickly" | Weeks-to-start and weeks-to-productivity both stated |
| Knock-ons | Not addressed | Founder-time, tools, and HR/finance step-functions all considered |
| Runway impact | "Reduces runway a bit" | Zero-cash date before/after on both burn numbers, in months |
| Decision | "Let's think about it" | Go / delay / no-go with specific override evidence |

## Definition of done

A skeptical co-founder or investor reading your memo would agree
that (a) the true cost of this hire is not the salary, and you've
counted the true cost, (b) the ramp lag is realistic and the
operating model has been updated to reflect it, and (c) the
go/delay/no-go decision follows honestly from the runway impact and
would flip only on the named evidence. When the offer goes out —
if it does — the runway consequence should not surprise you or the
board.

> Solutions are not provided in this repository; they live in the
> paired solutions repo.
