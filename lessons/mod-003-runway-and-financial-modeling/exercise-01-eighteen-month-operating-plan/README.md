# Exercise 01 — 18-Month Operating Plan

**Module:** 003 Runway & Financial Modeling · **Stage:** SEED · **Time:** ~1
week (≈6–8 focused hours)

## Deliverables (two founder artifacts, plus one call)

1. **An 18-month operating model** (spreadsheet or table): month-by-month
   payroll, non-payroll spend, revenue (if any), net burn, and running cash
   balance. The **zero-cash month** is marked.
2. **A one-page narrative** stating: current cash, current gross and net burn,
   post-hire burn, zero-cash date, and whether the business is currently
   **default alive or default dead** with the reasoning shown.
3. **A named set of decision points** — the "raise by," "cut by," and
   "kill by" months on the runway curve, each with the trigger that would
   confirm or override the decision.

## Scenario

Pick one:

- **Your real startup** (recommended if you're an operating founder): use
  your actual cash balance, current payroll, and near-term hiring plan.
- **Simulated:** You have **$310k in the bank**, are burning **$42k/month**
  gross (with **~$0/mo** revenue for the purposes of this exercise, so gross
  and net burn are the same today), and plan to **hire two engineers**. The
  first engineer starts in **month 3**, the second in **month 6**. Assume a
  **$180k base** per engineer and a **1.3× fully-loaded cost multiplier**
  unless you have better numbers to plug in; defend any change you make.

## Steps

1. **State the three founder numbers today.** Cash on hand, gross burn, net
   burn. Compute simple runway (`cash / net burn`). Write the answer as one
   line at the top of the sheet.
2. **Lay out the calendar.** Columns: month 1 → month 18. Rows: each person on
   payroll (with their monthly fully-loaded cost), each non-payroll expense
   category (hosting, tools, contractors, rent, legal, other), and any revenue
   line items. A hire that starts in month 3 has a zero in months 1–2 and their
   fully-loaded monthly cost from month 3 onward.
3. **Add the two engineers to the calendar.** Engineer #1 starts month 3,
   engineer #2 starts month 6. Show what monthly gross burn becomes in month 3
   and again in month 6. That is the **post-hire burn** number you'll cite in
   the narrative.
4. **Compute running cash.** Row: starting cash in month 0 = $310k. For each
   month, `end-of-month cash = prior-month cash + revenue − gross burn`.
   Highlight the month this line crosses zero. That is your **zero-cash date**.
5. **Stress-test the model.** Recompute the zero-cash date if either: (a)
   revenue never appears (default in the simulated scenario), (b) the second
   engineer is delayed by 3 months, (c) you *don't* make either hire. Which
   version buys the most time? Which is the honest baseline?
6. **Apply the default-alive/dead test.** Draw the growth and cost curves
   forward for 18 months. Under a plausible growth assumption, does revenue
   cross gross burn before cash hits zero? If yes, you're default alive on
   this trajectory; if no, default dead. Say which, and show the number.
7. **Name the decision points.** On the runway curve, mark:
   - The **"raise by"** month — 6–9 months before zero cash.
   - The **"cut by"** month — the latest month a cost cut can still buy
     meaningful runway.
   - The **"kill by"** month — the point at which continuing costs more than
     winding down.
   For each, write one sentence: *what evidence would change this call?*
8. **Write the one-paragraph narrative.** What does the model tell you to do
   this month? Hire on schedule, delay a hire, start raising, cut spend,
   something else? The narrative should read like a memo a co-founder or
   investor could act on.

## Operating-model template (fill inline)

```
Assumptions (cite source or mark ASSUMPTION):
  Starting cash (month 0):
  Current gross burn ($/mo):
  Current net burn ($/mo):
  Fully-loaded cost per engineer ($/mo):
  Hire dates: Eng #1 start month =   Eng #2 start month =
  Revenue assumption (per month or growth curve):
  Non-payroll spend categories:

Monthly grid (months 1 → 18):
  | Month              |  1  |  2  |  3  | ... | 18 |
  | Founder(s) payroll |     |     |     |     |    |
  | Eng #1             |  0  |  0  |  X  |     |    |
  | Eng #2             |  0  |  0  |  0  |     |    |
  | Other payroll      |     |     |     |     |    |
  | Hosting / tools    |     |     |     |     |    |
  | Contractors        |     |     |     |     |    |
  | Other              |     |     |     |     |    |
  | GROSS BURN         |     |     |     |     |    |
  | Revenue            |     |     |     |     |    |
  | NET BURN           |     |     |     |     |    |
  | End-of-month cash  |     |     |     |     |    |

Outputs:
  Post-hire monthly gross burn (from month 6 onward):
  Zero-cash month:
  Runway from today (months):
  Default alive or default dead? (with reasoning):

Decision points:
  Raise by (month):        Trigger to override:
  Cut by (month):          Trigger to override:
  Kill by (month):         Trigger to override:
```

## Narrative template (fill inline)

```
As of today we have $___ in the bank, gross burn of $___/mo and net burn of
$___/mo, giving us ___ months of runway on today's cost base.

After the planned hires (Eng #1 in month 3, Eng #2 in month 6), monthly gross
burn steps up to $___ and cash reaches zero in month ___.

Under our current growth assumption of ___, revenue does / does not cross
gross burn before cash runs out. We are therefore currently DEFAULT ALIVE /
DEFAULT DEAD.

The next action is to ___ by month ___, because ___. The specific evidence
that would change this call is ___.
```

## Rubric (self-assess, then compare to the exemplar)

<!-- needs-research: exemplar for mod-003 not yet authored; rubric-vs-exemplar comparison assumes future exemplars/mod-003-runway-and-financial-modeling/. -->

| Dimension | Weak | Strong |
|---|---|---|
| The three numbers | Only "runway" quoted; can't separate gross vs net | Cash, gross burn, net burn all stated and defended |
| Hire cost | Base salary used | Fully-loaded cost with multiplier or itemized line items |
| Timing | Hires "this year" | Specific start months, ramp lag acknowledged |
| Zero-cash date | Simple `cash / burn` division | Falls out of a month-by-month model with step changes |
| Stress test | Single scenario | At least one alternative (no revenue / delayed hire / no hire) |
| Default alive/dead | Not addressed | Named, with the projected curves that support the call |
| Decision points | "We'll raise when we need to" | Specific months with named override triggers |
| Narrative | Restates the numbers | Names the next action and the evidence that would change it |

## Definition of done

A skeptical seed-stage investor or co-founder reading your model and narrative
would agree that (a) the zero-cash date is correct given the assumptions,
(b) the default-alive/dead call is honest, and (c) the decision points are
actionable — not aspirational.
