# Exercise 02 — Gross vs Net Burn Stress Test

**Module:** 003 Runway & Financial Modeling · **Stage:** SEED · **Time:**
~90 focused minutes · **Prereq exercise:**
[exercise 01](./exercise-01-eighteen-month-operating-plan.md) — you
need the operating model before you can meaningfully stress-test it.
· **Reads with:** chapter
[02](../02-gross-vs-net-burn-trap.md).

## Problem statement

Exercise 01 produced an 18-month operating model with a base-case
zero-cash date. That date was computed against **net burn** —
customer revenue subtracted from cash out — which is the honest
going-concern number when revenue is real.

But customer revenue isn't a constant. Anchor customers churn.
Contracts slip a quarter. Pipeline dries up for reasons the model
never contemplated. The most common way founders discover their
runway was shorter than they thought is by planning on net burn and
having the customer-revenue line vanish for a quarter — the
"we'll make it up in revenue" trap from
[chapter 02](../02-gross-vs-net-burn-trap.md).

This exercise applies that stress test to the model you built in
exercise 01. Ninety focused minutes here surfaces the concealed
2–4 months of risk hiding in most seed-stage plans.

## Deliverable (one artifact)

A **burn-stress-test memo** — one page — appended to your operating
model, containing:

- The **current three numbers** (cash, gross burn, net burn) stated
  from your operating model.
- **Two runway numbers**: runway on net burn (napkin), and runway on
  gross burn (floor). Both expressed as months *and* as a zero-cash
  date, per [chapter 01](../01-three-founder-numbers.md).
- The **one-quarter revenue-disappearance test**: what happens to the
  zero-cash date if customer revenue goes to zero for the next three
  months and then recovers to some plausible reduced level.
- A **specific named concentration risk** — the customer, contract,
  or channel whose loss would materially move the numbers.
- A **board-update-ready three-line burn block** in the format from
  [chapter 02](../02-gross-vs-net-burn-trap.md) that you would
  actually paste into your next board update.

## Scenario

Use the operating model from
[exercise 01](./exercise-01-eighteen-month-operating-plan.md). If you
chose the real-startup scenario there, use your real revenue and
customer concentration; if you chose the simulated scenario there,
assume that by month 6 you have signed **4 customers paying $3.5k/mo
each** (so $14k/mo of customer revenue), with **one of them
contributing $8k/mo** (the anchor). The remaining three each pay
$2k/mo. Concentration: anchor is 57% of revenue.

## Requirements

The memo has to satisfy each of the following:

- **Both burn numbers stated at the top**, with source ("from
  operating model, base case, month X").
- **Both runway numbers stated** as months *and* as calendar
  zero-cash dates. Not "about a year of runway" — specific numbers.
- **Revenue-disappearance test** run per
  [chapter 02](../02-gross-vs-net-burn-trap.md): drop customer
  revenue to zero for months X+1 through X+3, recover to a plausible
  reduced level (roughly half of prior revenue is a defensible
  starting point) from X+4, extend runway from there. The two
  zero-cash dates (with the stress vs without) sit side by side.
- **Named concentration risk.** Not "if a customer churns" — the
  specific customer, contract, or pipeline segment whose loss you
  are modeling. If revenue is truly diversified with no single
  contributor > 20%, say that and explain the alternative failure
  mode (channel-level or category-level concentration).
- **Delta computed explicitly.** How many months of runway does the
  stress test consume? Is that delta big enough to change any
  hiring, spending, or raise-timing decision on the model?
- **Board-update block ready to paste.** Three-line format from
  chapter 02, filled with your actual numbers.

## Starter guidance

**Session 1 (~15 min) — restate the numbers.** From your operating
model, pull cash, gross burn, and net burn as of the base-case
month. Write them at the top of the memo. Compute both runway
numbers and both zero-cash dates. This should take five minutes if
your model was built cleanly; if it takes longer, the model needs
more named-assumption discipline.

**Session 2 (~30 min) — run the disappearance test.** Copy your
operating model into a scenario tab (or a new file). Set customer
revenue to zero for the next three months. Set months 4+ to a
plausible reduced revenue level and defend that number (roughly half
of the prior level is a common starting point; use your own judgment
based on the specific concentration story). Rerun the cash balance.
Record the new zero-cash date.

**Session 3 (~30 min) — name the concentration risk.** Look at your
customer list. What's the ratio of your biggest customer's monthly
revenue to your total? What's the ratio of your top-3? If any
single customer is more than 30% of MRR, that's your named risk. If
it's channel concentration (e.g., "80% of new customers come from
one referral partner"), name that. If it's contract-length
concentration (e.g., "the two biggest customers are on 3-month
contracts renewing in Q1"), name that.

**Session 4 (~15 min) — write the board-update block.** Format the
three-line burn block from chapter 02 with your actual numbers.
This is what should appear in your next board update; check that
it fits and reads cleanly.

## Memo template (fill inline)

```
Current three numbers (from operating model, month ___):
  Cash on hand           : $______
  Gross burn ($/mo)      : $______
  Net burn ($/mo)        : $______   (customer revenue: $______/mo)

Two runway numbers:
  On net burn (napkin)   : ______ months → zero cash: ______ 20__
  On gross burn (floor)  : ______ months → zero cash: ______ 20__

One-quarter revenue-disappearance stress test:
  Assumption: customer revenue → $0 for months ___ through ___
              then recovers to $______/mo from month ___
  Reasoning for recovery level: ______________________________

  Cash at end of month ___ (last no-revenue month) : $______
  Net burn from month ___ onward                    : $______/mo
  Zero-cash date under stress                       : ______ 20__

  Delta from base case: ______ months earlier

Named concentration risk:
  Customer / contract / channel: ______________________________
  Size of concentration: ______% of MRR (or ______% of new-customer flow)
  Notice we would get before loss: ______

Decision-relevance:
  Does the stress-test zero-cash date change any decision I'd make
  this month? YES / NO — because ______________________________

Board-update burn block (ready to paste):
  Gross burn                     : $____ / mo
    Payroll                      : $____
    Non-payroll operating spend  : $____
  Net burn (gross − cash in)     : $____ / mo
  Cash                           : $____
  Runway on net burn             : ____ months (zero-cash ____ 20__)
  Runway on gross burn (stress)  : ____ months (zero-cash ____ 20__)
```

## Acceptance criteria

You are done — and this exercise has met the module's standard — when
*all* of the following are true:

- [ ] **Both burn numbers** (gross and net) are stated at the top,
      with source.
- [ ] **Both runway numbers** are stated as months **and** as
      calendar zero-cash dates.
- [ ] The **revenue-disappearance test** has been run with a
      defensible reduced-recovery assumption, and the stressed
      zero-cash date is reported alongside the base-case date.
- [ ] A **specific concentration risk** is named (customer,
      contract, or channel), not hand-waved.
- [ ] The **delta between the two zero-cash dates** is stated in
      months and its decision-relevance is answered YES / NO with a
      one-line reason.
- [ ] The **board-update three-line burn block** is filled and ready
      to paste.

## Self-assessment rubric

| Dimension | Weak | Strong |
|---|---|---|
| Both numbers reported | Only net burn appears | Gross and net burn stated at the top, unprompted |
| Runway framing | Runway in months only | Both months and calendar zero-cash date |
| Stress test | Not run | Revenue-disappearance test run with defensible recovery assumption |
| Concentration risk | "If we lose a customer" | Specific customer / channel named with % of MRR |
| Delta | Not computed | Stated in months, with decision-relevance answered |
| Board-update block | Buried in prose | Ready-to-paste three-line format from chapter 02 |

## Definition of done

A skeptical board member reading your memo would agree that (a) the
gross-vs-net distinction is honestly reported, (b) the stress test
uses a plausible not paranoid assumption, and (c) the delta between
base-case and stressed runway either justifies action *this* month
or has been shown not to. The output of this exercise is either a
reassurance that your operating plan survives the stress or a
specific list of things you'd change if the stress became reality —
either way, it's what you should have already thought through before
the next board meeting.

> Solutions are not provided in this repository; they live in the
> paired solutions repo.
