# Chapter 06 — Decision Months on the Runway Curve: Raise-By, Cut-By, Kill-By

> **Reads with:** module objective 6 — *name the decision months on
> the runway curve — the "raise by" month (6–9 months before zero
> cash), the "cut by" month (before severance and wind-down costs eat
> the runway you thought you had), and the "kill by" month (before
> continuing costs more than winding down).*

## From zero-cash date to decision calendar

Chapter 04 introduced the zero-cash date — the month cash balance
crosses zero in the operating model. Chapter 05 introduced the
default-alive/dead diagnosis you run against that date. This chapter
is about the *other* dates on the runway curve: the calendar months
before zero cash at which specific decisions get made — or, if you
miss them, get made *for* you.

A good operating plan doesn't just show the zero-cash date. It marks
three earlier months in advance:

- **The "raise by" month** — start fundraising by this month or you'll
  raise from weakness.
- **The "cut by" month** — cut spend by this month or the cut can't
  meaningfully extend runway anymore.
- **The "kill by" month** — decide to wind down by this month or
  continuing costs more than closing.

Naming these months in advance is what separates a model from a
spreadsheet. The model tells you *when* the decision has to be made,
so it doesn't get made *for* you by the bank balance.

## The "raise by" month

**Rule of thumb: 6–9 months before zero cash.**

Fundraising takes longer than founders remember. From "first meeting
with a partner" to "wire in the bank," seed and Series A processes
routinely take 3–6 months, and that assumes the process runs cleanly
— first-choice lead says yes, term sheet signed, diligence and legal
finish on schedule.

Real processes have friction:

- **First meetings slip.** Partners are traveling, other deals get
  prioritised, calendars shift by weeks.
- **The first lead sometimes says no.** A common seed pattern is that
  your top 2–3 target funds pass and the fund that leads is the 6th
  or 10th meeting. Every reset adds weeks.
- **Diligence takes longer than promised.** References, customer
  calls, technical review, legal review — each is a small delay that
  compounds.
- **Legal closes take weeks after handshake.** Term sheet signed does
  not mean money in the account. The wire lands 4–8 weeks later.

<!-- needs-research: primary-source citation for seed / Series A process length norms — Y Combinator's Guide to Seed Fundraising describes typical timing; more recent data appears in Carta and PitchBook reports. -->

Add all of that up and 3–6 months is the *fast* path. Building in a
buffer for the "no" from the first choice takes you to 6–9 months of
process from first partner meeting to close. That is why the "raise
by" month is **6–9 months before your zero-cash date**, not "when we
notice we need to."

Two consequences:

- **The raise-by month is a hard deadline in the model.** Not "when we
  feel ready," not "when the metrics look good enough." A calendar
  date, backed off the zero-cash date, marked in the model, and
  reviewed monthly.
- **If you can't hit the raise-by month, you have to move up the
  cut-by month instead.** The raise-by and cut-by dates are linked;
  slipping one shortens the window on the other.

The strong founders in this game start meeting investors *before* the
raise-by month — building relationships in the year before they need
capital, so that when the process opens the top-of-funnel is already
warm. That's a separate topic (mod-004 covers fundraising process),
but it's why sophisticated founders treat "raise by" as the latest
acceptable start, not the intended one.

## The "cut by" month

**Rule of thumb: at least 2–3 months before you'd need to have cut
already, because the cut doesn't take effect immediately.**

The naïve model of a cost cut is: "we decide to cut in month 10, burn
drops in month 10, runway extends." That's not how it works. Cuts
have their own lag between "decide" and "cash actually stops
leaving," and severance often *increases* burn in the cut month
before it decreases burn in subsequent months.

Two specific reasons for the lag:

### Severance and wind-down costs

Cuts that involve layoffs cost cash up front. Standard practice
varies (by country, by policy, by individual contract), but a common
US-market severance for a seed-stage cut is 2–4 weeks of base plus
benefits continuation for a similar window. For a $180k engineer,
that's roughly $7k–$14k of cash out *in the cut month*, on top of
whatever the payroll obligation was.

If you cut three engineers in month 10, month 10's burn is *higher*
than a normal month by ~$20k–$40k of severance and PTO payouts, and
subsequent months' burn is lower by ~$60k. The runway extension is
real but starts in month 11, not month 10.

Contract terminations behave similarly:

- **Office lease.** Breaking a lease early often costs a lump-sum
  penalty or forces you to keep paying rent until you find a
  sub-tenant.
- **Software commitments.** Annual SaaS contracts prepaid for the
  year cannot be recovered by cancelling early.
- **Contractor engagements.** Many contractor SOWs have a notice
  period (2–4 weeks common) during which they keep billing.
- **Vendor minimums.** Any monthly minimum in a contract you're
  under continues until the term ends.

### Notice periods, PTO payout, and other statutory lags

- **Notice periods** vary; in the US at-will many are zero, but in
  many international geographies 30–90 days is standard and legally
  required.
- **PTO payout** — accrued but unused vacation — is a cash obligation
  in states/countries that require it.
- **COBRA subsidies** — if you're offering continued healthcare, this
  is a cash line for months after the departure.

### What the "cut by" month actually means

Put together, the "cut by" month is the last month at which a decision
to cut can *meaningfully* extend runway. It's roughly:

```
cut-by month = zero-cash month − (2 to 3 months for severance + lag)
              − (however many months of extension you'd need to justify
                 the cut in the first place)
```

If zero cash is month 12 and you're contemplating cuts that would
buy you 3 months of extended runway, you can't wait until month 11 to
make the call — the severance-inclusive cut month is a *worse* cash
month, and the extension only kicks in from month 13 onward. By the
time you'd have made up the cost, you've run out.

The practical rule: **decide by month 8 or 9 in a 12-month runway
scenario**, so the cut lands cleanly and the extension is real.

## The "kill by" month

**Rule of thumb: before continuing costs more than winding down.**

This is the least-discussed and most-avoided decision on the runway
curve. It's the month at which you should stop trying to raise, stop
trying to grow, and start honorably closing the company — because
continuing another month costs more than the wind-down costs would.

Wind-down is not free. To close a company honorably you owe:

- **Final payroll and severance.** All remaining employees, per your
  severance policy.
- **PTO payouts.** Accrued but unused vacation cashed out.
- **Contract terminations.** Any early-termination fees on office
  leases, vendor contracts, software commitments.
- **Return of refundable cash.** In some structures (SAFEs, notes
  with specific terms) or specific investor agreements, remaining
  cash may need to be returned to investors on wind-down; check your
  documents.
- **Filing and legal costs.** Formal dissolution filings, final tax
  returns, employment tax closures, C-corp/D&O tail insurance.

For a seed-stage company with 5–10 people, wind-down costs
realistically run **$50k–$200k**, and take **2–4 months** of
calendar time to execute cleanly. That's cash you have to *reserve*
for a controlled shutdown; if you burn through it, the shutdown
becomes uncontrolled — bounced payroll, unhonored severance,
reputation damage that follows every founder to their next thing.

The "kill by" month is therefore:

```
kill-by month = zero-cash month − (2 to 4 months of wind-down runway)
              − (a buffer for last-effort raise or cut attempts)
```

If zero cash is month 12, kill-by is typically month 8–10. Beyond
that, if the raise hasn't landed and cuts haven't restored
default-alive status, continuing to spend against the shrinking
balance takes options off the table and eventually forces an
uncontrolled shutdown.

### Why founders identify this too late

Almost every founder who runs a company to an uncontrolled shutdown
identifies the kill-by month with hindsight. Two reasons:

- **Optimism.** The founder believes the raise will land, the
  customer will sign, the launch will hit — and each month that it
  doesn't is one more month of hoping instead of deciding.
- **Cost of admission.** Deciding to wind down is admitting the
  company won't be what the founder promised employees, investors,
  and themselves. That admission is genuinely hard. Founders defer
  it, sometimes past the month at which honorable closure was still
  possible.

The best defense against this is **naming the kill-by month in
advance, in writing, in the operating model, when the runway is
comfortable.** Marked six months before it hits, the decision is a
line on a spreadsheet you can look at coolly. Marked in the month it
happens, it's a crisis. The former produces controlled exits and
gracefully honored obligations; the latter does not.

## What evidence would change the call

For each of the three decision months, the discipline is to write —
now, in the model — the specific evidence that would *change* the
call. Without that, the dates become superstitions ("we said we'd
raise by month 5, so we're raising"). With it, they're operational:

- **Raise-by month override:** "Would push out if we sign 2 anchor
  customers at $10k+/mo ARR each by month 4, extending runway past
  the natural raise-by."
- **Cut-by month override:** "Would push out if the raise lead-
  investor gives verbal by month 7, since a term sheet in month 7
  makes the cut moot."
- **Kill-by month override:** "Would push out if we have a signed
  acqui-hire LOI in hand, since the wind-down is happening either
  way and the deal timing changes the sequencing."

These override conditions convert the dates from arbitrary rules into
decisions that respond to evidence. A month that arrives with the
override condition met is a month you get to push out; a month that
arrives without it is a month you have to act.

## Where these live in the model

The three decision months belong in the assumptions block at the top
of the operating model, right beside the zero-cash date:

```
Cash-runway calendar (from operating model):
  Zero-cash date            : April 2027 (month 12)
  Raise by                  : October 2026 (month 6) — earliest OK to start
  Cut by                    : January 2027 (month 9) — later cuts are cash-in-cost only
  Kill by                   : February 2027 (month 10) — need 2mo wind-down runway

Override conditions:
  Raise by can push to Dec if: 2 new anchor customers > $10k/mo ARR by Nov
  Cut by can push to Feb if:   Series A term sheet signed by Dec
  Kill by can push to Mar if:  Acqui-hire LOI signed by Jan
```

Every monthly review, look at that block. If today's month has
passed the raise-by trigger without the override condition met, the
next thing on your calendar this week is investor outreach — not
optional. If it's past the cut-by month without the override, cuts
happen this month. If it's past the kill-by month without the
override, the wind-down decision is on the table.

## Summary

- The **raise-by month** is 6–9 months before zero cash — the latest
  moment to start fundraising without doing it from weakness.
- The **cut-by month** is 2–3 months before the moment when a cut
  could still meaningfully extend runway. Severance and contract
  wind-down costs mean cuts don't take effect immediately.
- The **kill-by month** is 2–4 months before zero cash — the moment
  after which continuing costs more than winding down. Wind-down
  itself takes real cash and calendar time.
- **Name the override conditions** for each date in advance. Without
  them, the dates are superstition; with them, they're operational.
- Put the three dates in the operating model as first-class outputs,
  right beside the zero-cash date. Review them monthly.

**Next:** the boundary that determines what this module owns and what
belongs to a full FP&A discipline — in
[chapter 07](./07-boundary-startup-finance-fundraising.md).
