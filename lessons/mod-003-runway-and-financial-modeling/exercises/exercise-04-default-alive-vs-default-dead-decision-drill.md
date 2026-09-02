# Exercise 04 — Default Alive vs Default Dead Decision Drill

**Module:** 003 Runway & Financial Modeling · **Stage:** SEED · **Time:**
~2 focused hours · **Prereq exercises:**
[exercise 01](./exercise-01-eighteen-month-operating-plan.md) (you
need the operating model) and
[exercise 02](./exercise-02-gross-vs-net-burn-stress-test.md) (you
need the honest gross-burn view). · **Reads with:** chapters
[05](../05-default-alive-vs-default-dead.md) and
[06](../06-decision-months-on-the-runway-curve.md).

## Problem statement

Exercise 01 gave you a zero-cash date. Exercise 02 stress-tested it.
This exercise applies **Paul Graham's default-alive vs default-dead
test** (from his October 2015 essay *Default Alive or Default Dead?*)
to that same model — honestly, with the growth rate you're actually
achieving, not the one you'd like to be achieving — and produces the
memo that answers the seed-stage central question:

> *At our current growth rate and cost trajectory, will we reach
> profitability before we run out of money?*

And then, from the answer, the decision: **raise, cut, grow into
profitability, or shrink the ambition.** Two focused hours here is
the most valuable use of a founder's calendar in any month where
the question isn't already answered.

<!-- needs-research: link to the primary Paul Graham essay at paulgraham.com/aord.html for canonical citation. -->

## Deliverable (one artifact)

A **default-alive/dead memo** — one page — containing:

- The **current gross burn**, **current revenue**, and **trailing
  3-month revenue growth rate** — all pulled honestly from your
  operating model.
- The **projected month at which revenue crosses gross burn**, using
  that honest growth rate.
- The **projected zero-cash month** on the base-case operating
  model.
- The **diagnosis** — DEFAULT ALIVE or DEFAULT DEAD — with the
  supporting reasoning.
- The **two flip conditions** — the growth-rate threshold and the
  burn threshold that would flip the diagnosis.
- The **decision** — this month's action from the raise / cut /
  grow / redefine-ambition menu — and the specific evidence that
  would change it.
- The **updated raise-by, cut-by, and kill-by months** on the
  runway curve if the diagnosis is default-dead.

## Scenario

Use the same operating model you built in
[exercise 01](./exercise-01-eighteen-month-operating-plan.md) and
stress-tested in
[exercise 02](./exercise-02-gross-vs-net-burn-stress-test.md). Real
or simulated — same choice as before.

If you chose the simulated scenario throughout: by month 6, revenue
is $14k/mo with anchor concentration per exercise 02, and the
trailing 3-month growth rate has been **~8% per month** in aggregate.
Gross burn is post-hire (both engineers on payroll), so ~$81k/mo
depending on your loading. Apply the test to that state.

## Requirements

The memo has to satisfy each of the following:

- **Trailing 3-month growth is real, not aspirational.** If your
  actual trailing three months averaged 5%/mo, that's the number —
  even if the deck says 20%. If you have fewer than three months of
  revenue history, use whatever you have and label it (e.g.,
  "trailing 6 weeks: X%").
- **Revenue-crosses-burn projection uses the honest growth rate.**
  If revenue is $14k/mo growing 8%/mo and gross burn is $81k/mo
  (assumed flat), the crossover month is `log(81/14) / log(1.08) ≈
  23 months`. Show your work.
- **Compare to base-case zero-cash month.** From the operating
  model. If the crossover is at month 23 and the zero-cash date is
  month 12, the diagnosis is default-dead on this trajectory.
- **Both flip conditions computed.** What growth rate would make
  revenue cross gross burn by the zero-cash month? What flat burn
  level would make current growth catch up before zero cash? Both
  are simple math from the same inputs.
- **A decision from the four-lever menu.**
  Grow faster (with a specific mechanism), cut burn (with a
  specific list of what gets cut), raise (with a start date and a
  target), or redefine the ambition. Not "some combination of the
  above" — pick a primary lever and defend it.
- **Updated decision-months calendar.** If default-dead, the memo
  ends with the raise-by / cut-by / kill-by calendar from
  [chapter 06](../06-decision-months-on-the-runway-curve.md), updated
  against the zero-cash date. If default-alive, note that fundraising
  is a *choice* rather than a rescue and set a fresh raise-by month
  for when it would make sense to raise anyway.

## Starter guidance

**Session 1 (~30 min) — the honest growth rate.** From your revenue
records or operating model, compute revenue in each of the last
three complete months. Compute the month-over-month growth for each
transition, then average. That's your trailing 3-month growth rate.
If it's flat or negative, that's the answer — do not smooth it into
"about 10%."

**Session 2 (~30 min) — the projection.** With current revenue,
current gross burn, and the honest growth rate, project revenue
month-by-month forward. In each month, does revenue exceed gross
burn? The first month it does is the crossover month. Compare to
the operating model's zero-cash month. Diagnose DEFAULT ALIVE
(crossover before zero cash) or DEFAULT DEAD (crossover after zero
cash or never at current trajectory).

**Session 3 (~30 min) — the flip conditions.** What growth rate
would make revenue cross burn one month before zero cash? What
burn level would make current growth catch up before zero cash?
Both are one-line computations, and the pair converts the
diagnosis from a label into a decision menu.

**Session 4 (~30 min) — the decision.** Pick the primary lever
(grow faster, cut, raise, redefine). Write the specific mechanism
(what grows faster, what gets cut, what raise, what smaller
ambition). Write the specific evidence that would change the call.
If default-dead, update the raise/cut/kill calendar per chapter 06.

## Memo template (fill inline)

```
Diagnosis inputs (from operating model, base case, month ___):
  Cash on hand                              : $______
  Gross burn ($/mo)                         : $______
  Revenue ($/mo)                            : $______
  Trailing 3-month revenue growth rate (%)  : ______%
    Month ___ revenue: $______
    Month ___ revenue: $______
    Month ___ revenue: $______
    (or state honestly if <3 months of history)

Projection:
  Revenue crosses gross burn at month ______ (or NEVER if growth < ___)
    Math: revenue × (1 + ______%)^n = gross burn
          → n = ______
  Base-case zero-cash month                 : month ______

Diagnosis:
  [ ] DEFAULT ALIVE — revenue crosses gross burn in month ______,
      before zero cash in month ______.
  [ ] DEFAULT DEAD — revenue crosses gross burn in month ______,
      but zero cash is in month ______.

Flip conditions:
  Growth rate that would flip to default-alive   : ______%/mo
    (would need to sustain this for ______ months)
  Gross burn level that would flip to default-alive: $______/mo
    (would need cuts of $______/mo)

Decision (pick one primary lever):
  [ ] GROW FASTER — specific mechanism: ____________________________
                                        ____________________________
  [ ] CUT — specific cuts (with monthly savings):
             _____________________________________ $______/mo
             _____________________________________ $______/mo
             _____________________________________ $______/mo
  [ ] RAISE — target size $______, start ______, close by ______
  [ ] REDEFINE AMBITION — smaller version: ____________________________
                                            ____________________________

  Evidence that would change this call: ____________________________
                                        ____________________________

Runway calendar (updated per chapter 06):
  Zero-cash date                : ______ 20__
  Raise by                      : ______ 20__  override: ______
  Cut by                        : ______ 20__  override: ______
  Kill by                       : ______ 20__  override: ______
```

## Acceptance criteria

You are done — and this exercise has met the module's standard —
when *all* of the following are true:

- [ ] The **trailing 3-month growth rate is stated honestly** (real
      numbers, not the deck's promise) with the month-by-month
      breakdown shown.
- [ ] The **revenue-crosses-burn projection is computed** with math
      shown, using the honest growth rate.
- [ ] The **diagnosis (DEFAULT ALIVE or DEFAULT DEAD) is named
      explicitly**, with the supporting month numbers.
- [ ] **Both flip conditions** — growth-rate threshold and burn
      threshold — are computed and stated.
- [ ] A **specific primary lever** (grow / cut / raise / redefine)
      is chosen, with a specific mechanism.
- [ ] The **override evidence** — what would change the call — is
      named.
- [ ] The **raise / cut / kill calendar** is present, updated to
      the current zero-cash date.

## Self-assessment rubric

| Dimension | Weak | Strong |
|---|---|---|
| Growth rate | "About 15%" or "we're growing well" | Trailing 3-month rate with monthly breakdown |
| Crossover projection | "Revenue will catch burn eventually" | Specific month, math shown |
| Diagnosis | Hedged ("kind of default alive") | Named unambiguously, with supporting numbers |
| Flip conditions | Not computed | Both growth-rate and burn-cut thresholds stated |
| Decision | "We need to raise soon" | Primary lever with specific mechanism, plus override evidence |
| Decision calendar | Missing | Raise / cut / kill months against current zero-cash date |

## Definition of done

A skeptical seed-stage investor or a co-founder reading your memo
would agree that (a) the diagnosis follows from the arithmetic
rather than from optimism, (b) the flip conditions convert the
diagnosis into an actionable decision menu, and (c) this month's
action is the right one given the diagnosis and the calendar. If
you're default-alive, the memo names the raise-by date at which
raising would be a *choice*; if you're default-dead, the memo names
the specific lever you're pulling this month and the evidence that
would change it. Either way, the memo is what you'd hand to the
board or a lead investor if they asked.

> Solutions are not provided in this repository; they live in the
> paired solutions repo.
