# Chapter 02 — Gross vs Net Burn: The "We'll Make It Up in Revenue" Trap

> **Reads with:** module objective 2 — *recognise the "we'll make it
> up in revenue" trap and stress-test runway against gross burn as if
> customer revenue disappeared for a quarter. Report both numbers in
> board updates and internal reviews.*

## Why one number isn't enough

Chapter 01 introduced two flavors of burn — gross (all cash out) and
net (gross minus customer revenue that hits the account) — and told
you to quote both. This chapter is why. The single most common way
seed-stage founders discover they had less runway than they thought is
by planning against **net burn** as if it were a fixed number, and
then having customer revenue evaporate for a quarter for reasons the
model never contemplated.

The gap between gross and net burn is not a rounding error. At early
stage it's often 30–50% of the total, and it moves *up and down every
month* as customers churn, contracts start late, or one anchor account
delays a wire. Founders who treat net burn as the only real number
end up on a runway calendar that lies to them by three to six months.

## The trap, stated plainly

Consider a founder with:

- **$310k in the bank**
- **$42k/month gross burn**
- **$14k/month in customer revenue**, giving **$28k/month net burn**

The napkin runway on net burn is `$310k / $28k ≈ 11 months`. The
napkin runway on gross burn is `$310k / $42k ≈ 7.4 months`. That's the
same company, the same day, two very different windows of time.

"We'll make it up in revenue" is the internal story that lets a
founder plan against the 11-month number. It says: revenue is going to
grow, the $14k/mo is going to be $25k/mo by month 6, so the net-burn
window will actually extend as time passes.

Sometimes that story is true. Very often it's not. Three specific ways
it fails, each of them common enough to have taken down real
companies:

1. **Anchor-customer concentration.** The $14k/mo is one customer
   paying $12k and three paying $700 apiece. The anchor churns in
   month 3. Revenue collapses to $2k/mo; the "11-month runway" was
   really a 7-month runway all along, and the founder finds this out
   with 4 months to react instead of the 8 they thought they had.
2. **Contract-start slippage.** Two of the four customer contracts
   were signed in July for an August start; procurement at the customer
   pushes them to October. Two months of expected revenue simply
   doesn't arrive, and the model that assumed steady-state was quietly
   optimistic by $28k of cash.
3. **A quarter of nothing new.** The pipeline dries up for a quarter —
   because the market shifts, because a competitor launches, because
   the founder was busy raising, because summer is summer. Existing
   revenue continues but no new revenue lands. The model that assumed
   continued growth has now underestimated burn for three months
   running.

In each case, the founder who planned on net burn has to make a
harder decision from a weaker position, three months later than they
would have, because the model concealed the risk.

## The stress test: recompute runway on gross burn

The fix is a single discipline: **whenever you quote net burn, also
quote runway on gross burn as the floor.**

The gross-burn runway answers a specific question:

> *How long do I have if customer revenue goes to zero for a quarter?*

That is not a paranoid question. It's the honest question. The
customer revenue you have this month is a live variable, not a
constant. Modeling it as constant is what the trap is.

Concretely, the discipline is:

- **Every board update reports both.** "Net burn is $28k, gross is
  $42k. Runway is 11 months on net, 7.4 months on gross." No board
  member should have to ask.
- **Every internal review computes both.** When a founder is deciding
  whether to hire, both numbers are the input, not just one. Net-burn
  runway is what you have; gross-burn runway is what you have if
  things go sideways.
- **Every fundraising conversation is honest about both.** Investors
  who take a serious look will ask for the gross-burn stress test.
  Founders who volunteer it look like operators; founders who have to
  be walked to it look like they haven't done the work.

## The one-quarter revenue-disappearance test

A stronger version of the stress test — the one that turns "know your
gross burn" into "have a plan for it" — is the **one-quarter
revenue-disappearance test**:

> *If customer revenue went to zero starting next month and stayed
> there for a full quarter, when would we run out of cash?*

The mechanic is simple. Take current cash, subtract gross burn ×
three (the three months of no revenue), then extend the remainder at
whatever revenue you'd realistically recover to.

Worked example:

- Cash today: **$310k**
- Gross burn: **$42k/mo**
- Current revenue: **$14k/mo** (drops to $0 for months 1–3, recovers
  to $10k/mo — not $14k, because a quarter of nothing new has
  degraded the base — from month 4)

The math:

- End of month 3 cash: `$310k − 3 × $42k = $184k`
- Month 4 onward net burn: `$42k − $10k = $32k/mo`
- Remaining runway from month 4: `$184k / $32k ≈ 5.8 months`
- Total runway: `3 + 5.8 = 8.8 months`

Compare that to the "11 months" the founder was quoting. The delta
(about 2 months) is the size of the concealed risk. If that gap is
large enough to change a hiring decision, a raise-timing decision, or
a spend-cut decision, the founder must plan against the stress-test
number, not the napkin.

The stress test isn't a prediction. It's an insurance claim you're
running mentally: *if this happens, what do I do?*

## Board-update and internal-review format

The reporting discipline that makes this a habit rather than a fire
drill:

**In board updates**, the burn slide should always show three lines,
not one:

```
Gross burn                     : $42k / mo
  Payroll                      : $34k
  Non-payroll operating spend  :  $8k
Net burn (gross - cash in)     : $28k / mo
Cash                           : $310k
Runway on net burn             : 11.0 months (zero-cash Aug 2027)
Runway on gross burn (stress)  :  7.4 months (zero-cash Apr 2027)
```

**In internal reviews** (co-founder weekly, department monthly, or
whatever cadence you keep), the same three lines belong on the top of
the doc. Every decision proposed in the meeting — hire, contract,
tool, launch, cut — should be answered in terms of how it moves those
three lines.

## The two disciplines together

Two disciplines, applied together, are what keep the gross-vs-net
distinction honest:

- **Always report both numbers.** Not because gross burn is more
  "true" than net — it isn't; net is what actually leaves the account
  in a normal month. But the pair together is more informative than
  either alone. Net tells you the going-concern rate; gross tells you
  the floor.
- **Always compute runway on gross burn as a stress test.** The
  question the gross-burn number answers — *what if revenue
  disappears for a quarter?* — is one of the two or three most
  important questions a seed-stage founder can answer. Do not defer
  it to the day it happens.

## What this changes in practice

A founder who internalises this chapter behaves differently in three
identifiable ways:

1. **They quote both numbers, unprompted.** No "we're burning $28k
   a month" without the "on $42k gross" that follows. It becomes
   automatic; it also becomes noticed by investors and board members
   as a signal of operating maturity.
2. **They make hiring and spend decisions against the stressed
   runway.** A hire that pushes runway from 11 months to 9 months on
   net burn but from 7.4 to 5.8 on gross burn is a very different
   decision from what the net number suggests. The stress test is
   the veto.
3. **They start conversations about revenue concentration earlier.**
   If a single customer is 60% of revenue, the gross-burn stress test
   is essentially the runway if that customer walks. Naming that
   concentration explicitly — to the board, to a co-founder, to
   yourself — is how you avoid discovering it in the churn moment.

## Summary

- **Net burn** (cash out minus cash in from customers) determines
  runway on a going-concern basis; **gross burn** (all cash out) is
  the floor if customer revenue disappears.
- The "we'll make it up in revenue" trap is planning against net burn
  as if customer revenue were a constant. It is not — anchor churn,
  contract slippage, and dry pipeline quarters routinely erase months
  of assumed inflow.
- The discipline is to **compute and report both**: net-burn runway
  and gross-burn runway, every board update, every internal review,
  every fundraising conversation.
- The **one-quarter revenue-disappearance test** — "what if revenue
  goes to zero for a quarter?" — is a stronger version of the gross
  stress test, and often reveals a 2–4 month gap the napkin missed.

**Next:** the single biggest input to gross burn — headcount — and
what a hire actually costs when you count the fully-loaded number, in
[chapter 03](./03-fully-loaded-hire-cost.md).
