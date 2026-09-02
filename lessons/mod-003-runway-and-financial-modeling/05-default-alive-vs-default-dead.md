# Chapter 05 — Default Alive vs Default Dead

> **Reads with:** module objective 5 — *apply Paul Graham's
> default-alive vs default-dead test (October 2015 essay) to decide
> whether the next move is to raise, cut, or grow into profitability.*

## The central seed-stage question

Paul Graham's October 2015 essay *Default Alive or Default Dead?*
poses the question that most seed-stage founders don't think to ask
themselves cleanly:

> *At your current growth rate and current cost trajectory, will you
> reach profitability before you run out of money?*

If yes, you are **default alive** — the current business, extrapolated
forward, gets to sustainability on its own. A raise is a *choice*, not
a rescue.

If no, you are **default dead** — the current trajectory ends with the
company running out of cash before it reaches profitability. Something
has to change: revenue must accelerate, costs must be cut, more
capital must arrive, or the company has to accept a smaller version
of the ambition.

<!-- needs-research: link to the primary Paul Graham essay at paulgraham.com/aord.html for canonical citation. -->

The test is short. It is deceptively easy to answer wrongly. And the
consequence of getting it wrong — usually by declaring default-alive
optimistically based on a growth curve you'd like to believe in — is
that the fundraising conversation you should have started in September
happens in February, from a weaker position, on worse terms.

This chapter is the discipline of applying the test honestly.

## The test is a projection, not a snapshot

The most common failure mode is treating the question as a snapshot:
"we have 11 months of runway and $14k/mo of revenue growing 20% a
month, therefore default alive." That is not the test. The test is
whether **the growth curve you're on crosses the cost curve you're on
before cash hits zero**.

Concretely: draw two curves on the same axes.

- **Revenue curve.** Current revenue in month 0. In each subsequent
  month, revenue = prior month × (1 + growth rate) — or a more
  explicit customer-by-customer model if you have one. Draw this out
  18 months.
- **Cost curve (gross burn).** Current gross burn in month 0. In each
  subsequent month, cost = prior month + step-ups for planned hires,
  tool upgrades, and rent changes. Draw this out 18 months.

Two things to look for on the chart:

1. **Do the curves cross before month 18?** If revenue crosses gross
   burn — meaning revenue >= gross burn, so net burn is zero or
   negative and the company is at least covering costs — before cash
   runs out, you are **default alive** on that growth trajectory. If
   they don't cross before your cash balance line hits zero, you are
   **default dead** on that trajectory.
2. **How aggressive is the growth curve?** A revenue curve that
   requires 20% month-over-month growth to catch cost is a *promise*,
   not a plan. If your current trailing three months has been growing
   at 6%/mo and the model needs 20%, you should not conclude
   default-alive; you should conclude *default-dead unless something
   changes*.

The honest test asks the second question as loudly as the first. A
growth rate you *hope for* is not evidence; a growth rate you *are
achieving* is.

## Two operational implications

Graham's essay isn't a diagnostic just to know where you sit. It
changes how you act in two specific ways:

### Default-alive founders raise from strength

If you're default alive, the fundraise is optional. You have the
option of continuing on your current trajectory without new capital,
which means:

- You can walk away from a bad term sheet. Investors can smell the
  difference between a founder who needs the money by Friday and one
  who is running a competitive process because they *chose* to raise
  now.
- You can pick investors on fit, not just check size. Speed becomes
  the negotiating lever; the founder who could close in two weeks
  without this specific investor negotiates a better structure.
- You can price the round higher. Default-alive founders raise on
  ambition and demonstrated traction; default-dead founders raise on
  urgency.

### Default-dead founders should know it earlier than they usually do

The most damaging thing about being default-dead is not the condition
— many great companies were default-dead at some point in their
seed-stage lives. It's the *lag* between when the founder should have
known and when they actually acknowledged it.

A default-dead founder who acknowledges it 12 months before zero cash
has real options:

- **Cut burn now** to extend runway and buy time to accelerate
  growth honestly.
- **Refocus on the smallest ambition that would work** — a narrower
  segment, a simpler product — that could get to profitability on
  the existing cash.
- **Start fundraising immediately** with the honest story that
  growth needs acceleration and this is the round that funds the
  team to do it.
- **Accept an acqui-hire or a wind-down** with severance and honor
  intact rather than being forced by a bank balance.

A default-dead founder who acknowledges it 3 months before zero cash
has none of those options. They have a fire.

The useful action, therefore, is not optimism about the growth curve.
It's **honest arithmetic** applied every month, and a decision made
in the calendar month it's cheapest — not the one it's easiest.

## Three ways to move from default-dead to default-alive

If the honest projection puts you in default-dead territory, four
levers can move you back:

### 1. Grow faster (make the revenue curve steeper)

If the reason cost catches revenue too slowly is that revenue is
growing at 4%/mo instead of the 12%/mo the model needs, the
default-alive path is a growth-rate change. That's a real strategic
project — usually a channel discovery, a segment change, or a pricing
change — and one that takes months to prove, not weeks. Concluding
that "we just need to grow faster" without a specific mechanism is
optimism, not a plan.

### 2. Cut burn (flatten or lower the cost curve)

Reducing gross burn — delayed hires, cut tools, contractor
consolidation, sometimes layoffs — is the fastest lever the founder
directly controls. A 20% cut in burn can extend runway by months, and
often moves the default-dead projection past cash-out. But cuts have
their own knock-on effects: reduced execution capacity often *also*
slows the revenue growth rate, so the model has to reflect both sides
of the cut, not just the cost side.

### 3. Raise more capital (push out the cash-out date)

A raise doesn't fix default-dead — it delays the date the diagnosis
becomes fatal. If underlying unit economics don't work, more cash
just buys a longer, more expensive version of the same failure (this
is the `mod-002` chapter 04 point about heuristic checks). But if the
unit economics do work and the company just hasn't accumulated enough
customers yet, more capital is exactly the right move — and it works
best precisely when the founder started it early enough to close
before default-dead becomes visible to investors.

### 4. Redefine the ambition

The fourth lever is under-discussed and often the honest answer.
Growing into profitability from a smaller base — a smaller team, a
narrower product, a specific segment — is what many companies
actually do when the "big" version of the business isn't fundable.
This is often called "going lifestyle" pejoratively, but it's simply
the recognition that the ambition and the capital available are not
aligned, and the ambition is the more flexible input.

## What to run monthly

The default-alive/dead test isn't a one-time exercise. It's a monthly
diagnostic that runs off the operating model from
[chapter 04](./04-eighteen-month-operating-model.md):

1. **Current gross burn**, from the model.
2. **Current revenue**, from the model.
3. **Trailing 3-month revenue growth rate**, honest — not the growth
   you hope for.
4. **Projected month revenue crosses gross burn**, using that honest
   growth rate.
5. **Projected zero-cash month**, from the model's cash-balance row.
6. **Diagnosis**: does the crossover happen before zero cash?
   *Default alive* or *default dead*.

Written as one line at the top of a monthly founder review, it looks
like:

```
2026-09: gross burn $42k/mo, revenue $14k/mo, trailing 3mo growth 8%/mo,
revenue crosses gross burn in month 19, zero cash April 2027 (month 7).
DEFAULT DEAD on trailing growth. Would flip default-alive at ~14%/mo
growth OR at $30k/mo gross burn.
```

That last clause — *the two conditions under which the diagnosis
flips* — is the most useful piece of the exercise. It converts the
diagnosis from a label into a **decision menu**: either the growth
rate has to reach X, or the burn has to drop to Y, and if neither is
plausible in the time available, a raise (or a smaller ambition) is
the remaining lever.

## Common wrong applications

Three ways founders misapply this test:

- **Using the growth rate you want, not the one you have.** Modeling
  20% MoM growth because "that's what a seed-stage startup should do"
  when the trailing three months are 5% is fiction. The test is only
  useful if the growth rate is the one actually observed.
- **Ignoring gross vs net.** Applying the test to net-burn and
  net-of-revenue projections without the gross-burn stress test from
  [chapter 02](./02-gross-vs-net-burn-trap.md) means an anchor-customer
  churn could flip default-alive to default-dead in a single month
  you didn't see coming.
- **Declaring default-alive because a raise is coming.** A signed but
  not-yet-closed round makes you default-alive *if it closes*. Until
  the wire lands, the diagnosis should be run *without* the round,
  and the round should be modeled as an upside scenario rather than
  a base assumption.

## Summary

- **Default alive** — current growth and cost trajectory reaches
  profitability before cash runs out; a raise is optional.
- **Default dead** — current trajectory doesn't; something has to
  change (grow, cut, raise, or shrink the ambition).
- The test is a **projection**, not a snapshot — draw the revenue and
  cost curves forward and see whether they cross before cash hits
  zero.
- Use the **honest** growth rate (trailing three months), not the one
  the deck promises.
- Run the test **monthly**; report the diagnosis plus the two
  conditions (growth-rate threshold, burn threshold) that would flip
  it. That's the decision menu.
- Default-alive founders **raise from strength**; default-dead
  founders should acknowledge the diagnosis **early**, because the
  options available at 12 months from zero don't exist at 3 months
  from zero.

**Next:** the specific calendar months on the runway curve where the
"raise," "cut," or "kill" decision has to be made — before it makes
itself — in
[chapter 06](./06-decision-months-on-the-runway-curve.md).
