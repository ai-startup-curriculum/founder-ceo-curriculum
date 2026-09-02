# Chapter 04 — Building the 18-Month Operating Model

> **Reads with:** module objective 4 — *build an 18-month operating
> model with three sections — cash in, cash out, cash balance — every
> input a named assumption, every hire on the calendar, the zero-cash
> date highlighted.*

## What an operating model is

An **operating model** is a month-by-month spreadsheet whose one job
is to answer, week over week, the question: **when does cash hit
zero, and what would change that?**

It is not a five-year forecast. It is not a fundraising deck's
"projections" page. It is not a valuation model. Those are all
adjacent artifacts with different jobs. The founder's operating model
is a short-horizon operational instrument — 18 months out, no further,
because 18 months is roughly the time between fundraises at seed and
Series A, and anything beyond that horizon is guessing dressed as
arithmetic.

Three properties define a useful founder operating model:

- **Three sections: cash in, cash out, cash balance.** Every founder
  operating model on the planet reduces to these three, and the third
  falls out of the first two.
- **Every input is a named assumption.** Not "$18k/mo in revenue"
  floating in a cell; a labelled row called "6 customers × $3k ARPA
  holding flat" that you can point to and say "this is the bet."
- **Every hire is on the calendar.** Not "we'll hire 4 engineers this
  year"; a row per person, each with a specific start month and a
  monthly fully-loaded cost from that month forward.

If your model has those three properties, the **zero-cash date** — the
month cash balance crosses zero — is a real output that will move when
you edit any assumption. That's the whole instrument.

## The three sections

### 1. Cash in

Cash in is every dollar you expect to receive in a given month.
Sources, in decreasing order of predictability:

- **Recurring customer revenue.** Monthly (or monthly-equivalent)
  subscription payments, contract billings, usage revenue that has
  landed. Model per customer if you have few enough to name them, or
  in cohorts if you have too many.
- **One-time customer payments.** Setup fees, professional services,
  one-off milestone payments. These are real cash but non-recurring;
  model them as one-time entries in the specific month they land,
  not as ongoing revenue.
- **Other operating inflows.** Grants (with actual timing of when the
  money lands), refunds, interest income if you're parking cash in a
  money-market account with meaningful balance.
- **Funding events.** SAFE closes, priced rounds, debt drawdowns.
  These are one-time cash events that step the cash balance up on
  the month they close. Model them at the *conservative* landing
  month — if a lead is "expected to close in November" and you have
  the option, model it as December, and know the model will improve
  if it lands earlier.

Two disciplines that keep this section honest:

- **Cash received, not invoiced.** A customer who signs in June for
  quarterly billing shows up as cash in July, October, January,
  April — not as $12k in June. If they pay late (they will), that's
  what actually goes in the model.
- **Model funding conservatively.** A signed term sheet is not cash;
  a wire is cash. Include a round in the model only when you're
  planning around it, and always show two versions of the model — one
  with the round, one without — so you know how sensitive the plan
  is to the raise.

### 2. Cash out

Cash out is every dollar leaving the account in a given month, in the
month it actually leaves. Rows worth carrying explicitly:

- **Payroll — one row per person, at fully-loaded cost.** Founders,
  each employee, each committed offer that hasn't started yet.
  Chapter 03 covered why base salary is the wrong number here; the
  row should be the fully-loaded monthly figure, and it should
  turn on in the person's actual start month, not before.
- **Contractors and fractional hires.** Fractional CFO, part-time
  designer, contract engineers. Model at their actual monthly cost;
  if the engagement ends on a specific month, model the row to zero
  out then.
- **Hosting and infrastructure.** Cloud spend, per-request LLM
  inference cost for AI products, third-party APIs. These often
  scale with usage; if usage is growing, so is this row.
- **Software and tooling.** All SaaS seats, per-seat or tier-based.
  A useful discipline: keep a subordinate sheet listing every tool,
  its per-seat cost, and the tier, so you can see when the next
  step-up hits.
- **Occupancy.** Rent, coworking, utilities. Zero for many fully
  remote seed-stage companies.
- **Professional services.** Legal (recurring counsel fee plus
  event-driven work), accounting, payroll processing, insurance.
- **Marketing and sales spend.** Ad spend, content, tools, events,
  contractors. If your CAC math is honest per `mod-002 chapter 03`,
  the founder-time in this row is nonzero even if you're not writing
  yourself a check.
- **Other operating spend.** Travel, offsites, benefits admin fees,
  bank fees, one-off legal or tax expenses.

The row-per-person, row-per-tool granularity is what makes the model
actionable. If you keep payroll as one line item ("$34k/mo"), you
cannot answer "what if we delay the next hire by two months?" without
rebuilding. If every hire has their own row, that scenario is a
one-cell edit.

### 3. Cash balance

Cash balance is not an input — it's a derived row that falls out of
the first two:

```
end-of-month cash = prior-month cash + cash in − cash out
```

Starting cash (month 0) is your current bank balance. Each subsequent
month is the prior month plus that month's inflows minus that month's
outflows. This row is what you watch, and the month it crosses zero is
the **zero-cash date** — the single most important number the model
produces.

## Named assumptions: every input has a label

The property that separates a working operating model from a
spreadsheet is that **every input line is a named, editable
assumption**. Not a hard-coded number buried inside a formula — a
labelled row you can point to, argue about, and edit without breaking
anything else.

At the top of the sheet (or in a separate assumptions tab), a good
operating model has a block that looks like:

```
Assumptions (edit these to run scenarios):
  Starting cash (month 0)                   : $310,000
  Founder salary ($/mo, fully loaded)       : $12,000
  Engineer salary base ($/yr)               : $180,000
  Fully-loaded multiplier                   : 1.30
    → Engineer fully-loaded ($/mo)          : $19,500
  Hire dates:
    Engineer #1 start month                 : 3
    Engineer #2 start month                 : 6
  Hosting / infra base ($/mo)               : $2,500
  Hosting growth rate (%/mo)                : 5%
  Tools & software ($/mo, current)          : $1,200
  Legal & accounting ($/mo, blended)        : $2,000
  Other operating ($/mo)                    : $1,500
  Marketing spend ($/mo)                    : $0
  Revenue at month 0 ($/mo)                 : $0
  Revenue growth assumption ($/mo added)    : $0
```

Every downstream row is a formula that references those cells. If you
edit "Engineer #2 start month" from 6 to 9, the model recalculates
end-to-end without you touching payroll rows, and the zero-cash date
shifts accordingly.

This isn't spreadsheet-engineering aesthetics. It's the mechanism by
which the model *stays true over time*. Without it, every edit is a
copy-paste-and-hope; with it, every edit is a decision.

### The two "types" of assumption to flag

Not all assumptions are equally uncertain. A useful convention:

- **Facts** — numbers you know, from a signed contract, an actual bank
  balance, or a committed offer. Label these with the source (e.g.,
  "per bank as of 2026-09-01," "signed offer Eng #1 2026-08-14").
- **Assumptions** — numbers you're guessing at, however
  intelligently. Label these **ASSUMPTION** with a short note on
  what would change them (e.g., "ASSUMPTION: hosting growth 5%/mo,
  update after Nov usage").

A model with 15 facts and 5 assumptions is a very different
instrument from one with 5 facts and 15 assumptions. Being able to
count is what tells you which one you're running.

## Every hire on the calendar

The single biggest source of runway surprises is hires that were
approved "sometime this year" showing up in the payroll row three
months earlier than the model expected. The fix is administrative,
not intellectual: **every hire has a specific start month, and that
start month is in the model as a named assumption.**

Two mechanical rules:

- **A hire's cost starts in their start month, at zero before that.**
  A row for "Engineer #2, start month 6" has zeros in months 1–5 and
  the fully-loaded monthly cost from month 6 onward. When you edit
  the start month, the row's zeros extend or contract.
- **A committed offer counts as booked headcount for planning
  purposes.** Once an offer is out and accepted, budget as if it's
  starting on the accepted date. Delays and reneges do happen, but
  planning against them is optimism, not prudence.

The calendar view of hires is what makes the model useful for the
core question in the founder's head: "if I move this hire by a month,
what happens?" With the calendar visible, that question is a two-cell
edit. Without it, it's a rebuild.

## Zero-cash date, highlighted

The **zero-cash date** — the calendar month cash balance crosses zero
— should be visually obvious on the sheet. Conditional formatting on
the cash-balance row: highlight the first month with a negative value
in red; ideally, freeze a summary cell at the top of the sheet that
reads back "zero-cash date: April 2027" so it's the first thing you
see when you open the model.

Two things follow from making the zero-cash date primary:

- **Every proposed action is scored against it.** A hire that moves
  the date from April to February is a very different decision from
  one that moves it from April to March. A contract that moves it
  from April to June extends the window in a way the founder should
  celebrate loudly.
- **The date is what you brief investors and board members with.**
  "Zero-cash April 2027" is a fact; "about a year of runway" is a
  vibe. The date carries more information and does not degrade over
  time — you and the reader can both check whether it's still true
  next month.

## The three-scenario minimum

A single operating model is a single set of assumptions. But real
decisions are made against a *distribution* of possible futures. The
minimum discipline is to run three scenarios and report the
zero-cash date under each:

1. **Base case.** Your best current guess for revenue, hires, and
   spend. This is the plan you're currently executing.
2. **Downside case.** Revenue disappears for a quarter (per
   [chapter 02](./02-gross-vs-net-burn-trap.md)'s one-quarter
   revenue-disappearance test), or a key hire is delayed, or an
   assumed round doesn't close on time. This is the floor.
3. **Upside case.** A named opportunity — a big customer signs, a
   contract you're expecting to lose renews — hits. This is the
   ceiling.

Report all three zero-cash dates in every review. The base case tells
you the plan; the downside tells you when the plan breaks; the upside
tells you which upside would meaningfully change the decision
calendar. If the upside doesn't shift the zero-cash date by at least
3 months, it's a nice-to-have, not a load-bearing outcome.

## A minimum viable operating model

The smallest sheet that satisfies everything above has ~20 rows and
~20 columns. Rows by section:

```
CASH IN                     | mo1 | mo2 | mo3 | ... | mo18 |
  Customer recurring        |     |     |     |     |      |
  Customer one-time         |     |     |     |     |      |
  Funding events (if any)   |     |     |     |     |      |
  TOTAL CASH IN             |     |     |     |     |      |

CASH OUT
  Founder(s) payroll        |     |     |     |     |      |
  Employee #1               |     |     |     |     |      |
  Employee #2               |     |     |     |     |      |
  Engineer #1 (start mo 3)  |  0  |  0  |  X  |     |      |
  Engineer #2 (start mo 6)  |  0  |  0  |  0  |     |      |
  Contractors               |     |     |     |     |      |
  Hosting / infra           |     |     |     |     |      |
  Software / tools          |     |     |     |     |      |
  Legal / accounting        |     |     |     |     |      |
  Occupancy                 |     |     |     |     |      |
  Marketing                 |     |     |     |     |      |
  Other                     |     |     |     |     |      |
  TOTAL CASH OUT (GROSS)    |     |     |     |     |      |

DERIVED
  Net burn (out - in)       |     |     |     |     |      |
  End-of-month cash         |     |     |     |     |      |
```

The end-of-month-cash row, with the zero-crossing highlighted, is the
output. Everything above it is the input.

## What the model does not tell you

A month-by-month operating model is powerful for one class of
question — *when does cash hit zero, and how does that date change if
I move a lever?* — and misleading for others. It does not tell you:

- **Whether the plan is a good idea.** The model runs whatever
  assumptions you feed it. Revenue growing 20% a month with no
  supporting evidence gives you a rosy zero-cash date and no signal
  that the assumption is fantasy. The riskiest-assumption discipline
  from `mod-002` chapter 05 is what pressure-tests the assumptions.
- **What to spend money on.** The model tells you cost and timing; it
  does not tell you *which* hire, which tool, or which contract is
  the right one to invest in. Strategy is not modeled here.
- **Long-horizon financial statements.** Full three-statement models
  (P&L, balance sheet, cash flow with proper accruals) are the
  province of a real FP&A discipline — see
  [chapter 07](./07-boundary-startup-finance-fundraising.md) for the
  boundary with the `startup-finance-fundraising-curriculum` peer
  track. The founder's operating model is a cash-forward instrument;
  the CFO's model is the audited financial picture.

## Summary

- The founder operating model has three sections — **cash in, cash
  out, cash balance** — and one primary output: the **zero-cash
  date**.
- Every **input is a named assumption** you can edit in one place, so
  scenarios are a one-cell change rather than a rebuild.
- Every **hire is on the calendar** with a specific start month and a
  fully-loaded monthly cost.
- **Run three scenarios minimum** — base, downside, upside — and
  report all three zero-cash dates in every review.
- The model does not tell you whether the plan is good or what to
  spend on. It tells you *when the plan breaks* — which is the input
  to those bigger decisions.

**Next:** the framework for deciding what the model's zero-cash date
means for the current decision — Paul Graham's default-alive vs
default-dead test — in
[chapter 05](./05-default-alive-vs-default-dead.md).
