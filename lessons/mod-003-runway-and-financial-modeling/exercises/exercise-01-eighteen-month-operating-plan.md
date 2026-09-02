# Exercise 01 — 18-Month Operating Plan

**Module:** 003 Runway & Financial Modeling · **Stage:** SEED · **Time:**
~6–8 focused hours (one working week for an operating founder) · **Reads
with:** chapters [01](../01-three-founder-numbers.md),
[03](../03-fully-loaded-hire-cost.md), and
[04](../04-eighteen-month-operating-model.md).

## Problem statement

You have a canvas and unit-economics sheet (from `mod-002`) and no
operating model — only a rough sense of how much cash is in the account
and a vague conviction that "we probably have about a year." This
exercise turns that vague conviction into a real, month-by-month
operating model: three sections (cash in, cash out, cash balance),
every input a named assumption, every hire on the calendar, and the
**zero-cash date** as a first-class output.

The exercise is not to produce the "right" plan. It's to produce a
plan **specific enough to be wrong**, so that when reality diverges
from it — it will — you already know which lever to pull. Exercises
02, 03, and 04 all extend this model, so getting the structure right
now is what makes them work.

## Deliverables (two founder artifacts, plus one call)

1. **An 18-month operating model** (spreadsheet or table): three
   sections (cash in, cash out, cash balance), month 1 through month
   18, one row per person on payroll, one row per major spend
   category, and a highlighted **zero-cash month**.
2. **A one-page narrative** stating: current cash, current gross and
   net burn, post-hire burn, zero-cash date, and whether the business
   is currently **default alive or default dead** with the reasoning
   shown.
3. **A named set of decision points** — the "raise by," "cut by," and
   "kill by" months on the runway curve, each with the trigger that
   would confirm or override the decision (see
   [chapter 06](../06-decision-months-on-the-runway-curve.md)).

## Scenario

Pick one:

- **Your real startup** (recommended if you're an operating founder):
  use your actual cash balance, current payroll, and near-term hiring
  plan. This is what the model exists for.
- **Simulated:** You have **$310k in the bank**, are burning
  **$42k/month** gross (with **~$0/mo** revenue for the purposes of
  this exercise, so gross and net burn are the same today), and plan
  to **hire two engineers**. The first engineer starts in **month 3**,
  the second in **month 6**. Assume a **$180k base** per engineer and
  a **1.30× fully-loaded cost multiplier** unless you have better
  numbers to plug in; defend any change you make per
  [chapter 03](../03-fully-loaded-hire-cost.md).

## Requirements

The model has to satisfy each of the following, checkably, by the
end of the exercise:

- **Three sections labelled explicitly:** cash in, cash out, cash
  balance. Not one monolithic block.
- **18-month horizon** (month 1 through month 18). Not 12, not 24.
- **Every input line is a named assumption** at the top of the sheet,
  and every downstream row references those assumptions rather than
  hard-coding the number in a formula. Editing "Engineer #2 start
  month" from 6 to 9 should re-run the model end-to-end without any
  other edit.
- **Every person on payroll is a row.** Founders, current employees,
  each committed offer that hasn't started, each planned hire. Each
  row shows zeros before the start month and the fully-loaded monthly
  cost from the start month forward.
- **Fully-loaded cost, not salary**, for every payroll row. State the
  multiplier you're using and defend it (a line item breakdown counts
  as defence; the rule of thumb "we're using 1.30 as US-market
  typical" counts as defence).
- **Non-payroll spend broken into at least five categories:**
  hosting/infra, software/tools, contractors, legal/accounting, other
  operating. Add rows for marketing spend or occupancy if either
  applies to your scenario.
- **The cash-balance row falls out of a formula**, not from
  hard-coded numbers — it's `prior month cash + cash in − cash out`,
  every month.
- **The zero-cash month is visually highlighted** on the sheet
  (conditional formatting, a colour, or a summary cell at the top).
- **Post-hire burn is stated as an explicit line at the top.** Not
  buried in the model — a labelled cell that reads "post-hire monthly
  gross burn (from month 6 onward): $X."
- **Three scenarios run**, per
  [chapter 04](../04-eighteen-month-operating-model.md): base
  (current plan), downside (revenue disappears for a quarter, or a
  hire is delayed and no revenue lands), upside (a specific plausible
  positive scenario you name). Report the zero-cash date under each.

## Starter guidance

**Session 1 (~1 hr) — the three founder numbers today.** Read
[chapter 01](../01-three-founder-numbers.md). Write, at the top of the
sheet, the three numbers today: cash on hand, current gross burn, and
current net burn. Compute simple runway (`cash / net burn`) and
runway on gross burn (`cash / gross burn`). That single line at the
top is the anchor for everything below.

**Session 2 (~2–3 hr) — build the calendar.** Read
[chapter 04](../04-eighteen-month-operating-model.md). Lay out the
grid: columns month 1 → month 18, rows for the three sections. Fill
in the named-assumptions block at the top. Then fill in each row so
its values are formulas that reference those assumptions. Take the
time to make this real — an operating model built once, well, is an
instrument you'll edit weekly for the next year.

**Session 3 (~1–2 hr) — hires on the calendar.** Read
[chapter 03](../03-fully-loaded-hire-cost.md). Add the two engineers
(or your real planned hires) as named rows, each with a start month
and a fully-loaded monthly cost. Compute post-hire gross burn as an
explicit cell. State the ramp-lag assumption for any revenue you're
crediting the hires with (spoiler: at these dates, none).

**Session 4 (~1–2 hr) — scenarios and decision points.** Run the
three scenarios (base, downside, upside), reporting the zero-cash
date under each. Then, per
[chapter 06](../06-decision-months-on-the-runway-curve.md), name the
raise-by, cut-by, and kill-by months on the base-case runway curve,
each with an override condition.

**Session 5 (~1 hr) — narrative.** Write the one-page memo. What
does the model tell you to do this month? Hire on schedule, delay a
hire, start raising, cut spend, something else? The narrative should
read like a memo a co-founder or investor could act on this week.

## Operating-model template (fill inline)

```
Assumptions (cite source or mark ASSUMPTION):
  Starting cash (month 0)                     : $______
  Founder salary ($/mo, fully loaded)          : $______
  Engineer base salary ($/yr)                  : $______
  Fully-loaded multiplier                      : ______  source: ______
    → Engineer fully-loaded ($/mo)             : $______
  Hire dates:
    Engineer #1 start month                    : ______
    Engineer #2 start month                    : ______
  Hosting / infra ($/mo)                       : $______
  Software / tools ($/mo)                      : $______
  Legal / accounting ($/mo)                    : $______
  Other operating ($/mo)                       : $______
  Marketing spend ($/mo)                       : $______
  Revenue at month 0 ($/mo)                    : $______
  Revenue growth assumption                    : ______  source/ASSUMPTION

Monthly grid (months 1 → 18):
  | Month                        |  1  |  2  |  3  | ... | 18 |
  | CASH IN                      |     |     |     |     |    |
  |   Customer recurring         |     |     |     |     |    |
  |   Customer one-time          |     |     |     |     |    |
  |   Funding events             |     |     |     |     |    |
  |   TOTAL CASH IN              |     |     |     |     |    |
  | CASH OUT                     |     |     |     |     |    |
  |   Founder(s) payroll         |     |     |     |     |    |
  |   Engineer #1 (start mo 3)   |  0  |  0  |  X  |     |    |
  |   Engineer #2 (start mo 6)   |  0  |  0  |  0  |     |    |
  |   Other payroll              |     |     |     |     |    |
  |   Hosting / infra            |     |     |     |     |    |
  |   Software / tools           |     |     |     |     |    |
  |   Contractors                |     |     |     |     |    |
  |   Legal / accounting         |     |     |     |     |    |
  |   Marketing                  |     |     |     |     |    |
  |   Other                      |     |     |     |     |    |
  |   TOTAL CASH OUT (GROSS)     |     |     |     |     |    |
  | DERIVED                      |     |     |     |     |    |
  |   Net burn (out − in)        |     |     |     |     |    |
  |   End-of-month cash          |     |     |     |     |    |

Outputs:
  Post-hire monthly gross burn (from month 6 onward): $______
  Zero-cash month (base case)                       : month ___ / ______ 20__
  Zero-cash month (downside)                        : month ___ / ______ 20__
  Zero-cash month (upside)                          : month ___ / ______ 20__

Decision points (base case):
  Raise by (month)    : ______  Override condition: ______
  Cut by (month)      : ______  Override condition: ______
  Kill by (month)     : ______  Override condition: ______
```

## Narrative template (fill inline)

```
As of today we have $____ in the bank, gross burn of $____/mo and net
burn of $____/mo, giving us ____ months of runway on net burn and ____
months on gross burn.

After the planned hires (Eng #1 in month 3, Eng #2 in month 6),
monthly gross burn steps up to $____ and cash reaches zero in month
____ (base case) / month ____ (downside).

Under our current growth assumption of ____, revenue does / does not
cross gross burn before cash runs out. We are therefore currently
DEFAULT ALIVE / DEFAULT DEAD.

The next action is to ____ by month ____, because ____. The specific
evidence that would change this call is ____.
```

## Acceptance criteria

You are done — and this exercise has met the module's standard — when
*all* of the following are true:

- [ ] The model has **three sections** (cash in, cash out, cash
      balance) laid out over **18 months**.
- [ ] Every input line is a **named assumption** editable in one
      place, and downstream rows are formulas that reference it.
- [ ] Every person on payroll is a **row of their own**, at
      **fully-loaded cost**, with a specific start month.
- [ ] The **cash-balance row is a formula**, not hard-coded.
- [ ] The **zero-cash month is visually highlighted** and stated
      explicitly at the top of the sheet.
- [ ] **Post-hire gross burn** is a labelled cell.
- [ ] **Three scenarios** (base, downside, upside) have been run and
      the zero-cash date is reported under each.
- [ ] The **raise-by, cut-by, and kill-by months** are named, each
      with an override condition.
- [ ] The narrative names **this month's next action** and the
      **evidence that would change the call**.

## Self-assessment rubric

<!-- needs-research: exemplar for mod-003 not yet authored; the rubric-vs-exemplar comparison assumes future exemplars/mod-003-runway-and-financial-modeling/. -->

| Dimension | Weak | Strong |
|---|---|---|
| The three numbers | Only "runway" quoted; can't separate gross vs net | Cash, gross burn, net burn all stated at the top of the sheet |
| Hire cost | Base salary in the payroll row | Fully-loaded cost with a defended multiplier or itemised breakdown |
| Timing | Hires "this year" | Specific start months, ramp lag acknowledged for revenue |
| Model structure | One block; edits require rebuilding | Three sections; named assumptions; every scenario is a one-cell edit |
| Zero-cash date | `cash / burn` in the founder's head | Falls out of a month-by-month formula with step changes; highlighted on the sheet |
| Scenarios | Single base case | Three scenarios (base / downside / upside) with distinct zero-cash dates |
| Default alive/dead | Not addressed | Named, with the projected curves that support the call |
| Decision points | "We'll raise when we need to" | Specific months for raise-by, cut-by, kill-by, each with an override condition |
| Narrative | Restates the numbers | Names this month's next action and the evidence that would change it |

## Definition of done

A skeptical seed-stage investor or co-founder reading your model and
narrative would agree that (a) the zero-cash date is correct given
the assumptions, (b) the default-alive/dead call is honest, and (c)
the decision points are actionable — not aspirational. The model is
now the instrument you'll use for exercises 02, 03, and 04, and for
every hiring / spend / raise decision this month.

> Solutions are not provided in this repository; they live in the
> paired solutions repo.
