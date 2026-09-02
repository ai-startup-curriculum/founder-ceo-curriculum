# Chapter 03 — Fully-Loaded Hire Cost, Ramp Lag, and Knock-On Costs

> **Reads with:** module objective 3 — *model the fully-loaded cost of
> a hire (rough US-market rule of thumb: `base × 1.25–1.4×`) plus ramp
> lag (6–12 weeks to start, another quarter or two to productivity) and
> knock-on costs (management time, tooling, HR/finance step-functions).*

## Headcount is the lever

At seed stage, **people are usually 70–85% of cash burn** — payroll
dwarfs tools, hosting, and rent combined. That makes headcount the
single most consequential decision in the operating model. Every other
lever — cut a tool, renegotiate a contract, delay a launch — moves
burn at the margin. Adding or delaying a hire moves it in whole
percentage points of runway.

The problem is that founders overwhelmingly reason about hires in
**salary numbers**, not **cost-to-the-company numbers**. "We can afford
a $180k engineer" is not the same question as "we can afford the
$230k/year of cash a $180k engineer removes from the account," and the
gap between the two is exactly the mistake that turns a comfortable
runway into a scary one.

This chapter is the three corrections a founder has to apply before a
hiring decision can honestly be scored against the model:

1. **Fully-loaded cost** — the salary is not the number.
2. **Ramp lag** — the payroll starts on day one; the productivity
   doesn't.
3. **Knock-on costs** — the tenth hire is more than ten times the cost
   of the first.

## 1. Fully-loaded cost

A hire's **fully-loaded cost** is the total cash the company spends
per year to employ that person — not the offer letter's base salary.

The rough US-market rule of thumb is:

```
fully-loaded cost ≈ base salary × 1.25 to 1.40
```

So a `$180k` base is roughly `$225k–$252k/year` of actual cash out —
about `$19k–$21k/month`. The 25–40% loading covers, in roughly this
order of size:

- **Employer payroll taxes.** Social Security, Medicare, unemployment
  insurance (federal + state). In the US these run roughly 7.65% of
  wages up to the Social Security wage base, plus small state
  unemployment amounts. Small but not zero.
- **Healthcare and benefits.** Medical, dental, vision, life,
  disability, retirement match. The single largest line inside the
  loading multiplier; can be 8–15% of salary depending on plan
  generosity and family coverage.
- **Equipment and workspace.** Laptop, monitors, headphones, a desk
  if you're in an office, coworking if remote. Amortised — a
  $3k laptop is $1k/year over three years — but non-zero.
- **Software and tooling seats.** Every SaaS in your stack that's
  priced per-seat: Slack, GitHub, Notion, Linear, 1Password,
  observability, design tools. Adds up faster than founders expect.
- **Training, travel, and offsites.** Conferences, onboarding travel,
  quarterly offsites.
- **Recruiting cost, amortised.** Agency fees (if used, typically
  20–25% of first-year salary), the founder-time cost of interviews,
  contract-recruiter retainers.

<!-- needs-research: primary-source citation for the "1.25-1.4× fully-loaded cost" multiplier — commonly cited by MIT and SBA guidance but the exact ratio is context-dependent (benefits generosity, country, remote/office). SHRM publishes annual employer cost data through the Bureau of Labor Statistics' Employer Costs for Employee Compensation (ECEC) series. -->

Two important caveats on the multiplier:

- **It's a starting point, not a truth.** The 1.25× floor assumes lean
  benefits and no office; the 1.40× ceiling assumes generous benefits,
  an office, and rich equity refresh grants that require a 409A
  refresh. Companies with global remote teams, or teams in countries
  with mandatory contributions well above US norms (Germany, France,
  Nordics), can see the multiplier climb past 1.5×.
- **Build it from your line items, not the rule of thumb.** The right
  discipline is to compute your *actual* loading once — for a typical
  hire in your setup — by adding up the per-person cost lines above
  and dividing by base salary. If your number is 1.28, use 1.28. If
  it's 1.42, use 1.42. Then apply that number consistently.

## 2. Ramp lag: payroll starts before productivity does

The second correction founders underweight is **ramp lag**: the gap
between the day the payroll clock starts and the day the hire is
contributing at the level the org planned for.

Two phases, both of which are real cash events for the company:

### Time-to-start

From "we decide to hire" to "they start" is typically:

- **6–12 weeks for engineers and generalist roles** who accept quickly
  and have short notice periods.
- **3–6 months for senior specialists** (staff/principal engineers,
  design leads, first VP of X hires) who take longer to source,
  interview, and close, and often have longer notice periods at their
  current employer.
- **Longer for regulated hires or specific geographies** where visas,
  reference checks, or non-competes add weeks.

This time is spent by the founder or a recruiter, not the hire — but
it's the time between when the model *needs* the person and when the
person can actually start. If you decide in January that you need a
senior engineer for a Q2 launch, and the average time-to-start is 10
weeks, then the decision needed to be made in November — and the
person joins in April, not February.

### Time-to-productivity

From start date to fully productive is *another* period:

- **6–12 weeks for a well-scoped IC role** (an experienced backend
  engineer joining a well-documented codebase to own a defined
  feature area).
- **A quarter or two — 3–6 months — for a role that requires learning
  the business** (a first PM, a first designer, a first sales rep, a
  first CSM).
- **Six months to a year for a leadership hire** (a VP whose first
  quarter is largely diagnosis and relationship-building before they
  can shape the function).

The full ramp — start plus productivity — for many senior hires is
therefore a *quarter or two*. A hire made in January often doesn't
move a metric until Q2 at the earliest, and often Q3 for a leadership
role. But the payroll starts on day one.

### The two consequences for the model

Ramp lag has two operational consequences the model has to reflect:

- **The offer date, not the start date, is when planning starts.**
  Once an offer is out and accepted, the payroll obligation is
  locked in even before the person is on the calendar. Model the
  monthly cost from the *start date*, but treat any committed offer
  as effectively booked headcount.
- **Don't credit revenue against ramp.** A common founder mistake is
  to model a new sales hire as producing pipeline in month 1. The
  honest model gives a sales hire zero pipeline for a quarter,
  ramping pipeline through the second quarter, and full quota
  production starting somewhere in month 6–9. If your model assumes
  faster than that, the model is optimistic in the exact place that
  matters most.

## 3. Knock-on costs: the tenth hire

The third correction is the one founders discover the hard way. Every
new hire is not an independent cost line — hires interact.

Three kinds of knock-on cost:

### Founder / manager time

Every hire pulls management time — from the founder, from the tech
lead, from whoever they report to — for onboarding, 1:1s, code review,
context-transfer, career conversations. At seed stage the founder is
often the manager, which means the founder's calendar, which is
already the scarcest resource in the company, gets even scarcer with
every hire.

The naïve model treats this at zero. The honest model values founder
time at a **fair-market replacement rate** — the salary you'd pay a
VP of Engineering or a Head of Product to do the management work — and
attributes some fraction of that back to each report. This mirrors the
founder-time-in-CAC discipline from `mod-002` chapter 03: uncounted
founder hours are the biggest single lie in early-stage cost
modeling.

### Tooling step-functions

Some tools have per-seat pricing that scales cleanly with headcount.
Others have tier-based pricing that jumps discretely at specific
headcount thresholds — e.g., Slack, GSuite, Notion, and many
observability and HR tools have "up to 10" or "up to 25" tiers that
step up when you cross the boundary.

The tenth hire that crosses one of those tier boundaries costs the
company its own fully-loaded number *plus* the step-up on every
tool that just changed tier. That's often a few hundred to a few
thousand dollars a month of hidden burn attributable to that hire.

### HR, finance, and legal step-functions

There are three headcount ranges where administrative burden
step-functions kick in, and each one is a step-change in fixed cost:

- **~10 employees.** You start needing real HR practice —
  compliance-grade employment agreements, an actual employee handbook,
  a benefits broker, dedicated payroll software rather than a
  founder-run spreadsheet.
- **~25 employees.** You start needing an HR generalist (or a
  fractional one), a real onboarding process, and often a first
  finance hire or fractional CFO because the founder can no longer
  reasonably reconcile spend across 25 people.
- **~50 employees.** You cross thresholds that trigger federal HR
  reporting in the US (EEO-1) and typically need in-house HR, a
  finance manager, and a real controller function. Many companies
  hire a first People Operations person here.
  <!-- needs-research: primary-source citation for US EEO-1 reporting threshold — currently 100 employees for private employers under Title VII, or 50 for federal contractors under Executive Order 11246. Verify current thresholds via EEOC. -->

None of these are the *tenth engineer's* fault. But if the tenth
engineer is what crosses the 10-employee threshold, the cost the
company pays in the following months (broker fees, payroll upgrade,
handbook drafting) is reasonably attributed to that hire in an honest
model. That's why "the tenth hire is more than 10× the cost of the
first" is a rule of thumb: the first hire adds one salary; the tenth
hire adds one salary *plus* forces the step-function.

## Putting it together: what a hire really costs

The naïve version of a hiring decision:

> *"Can we afford a $180k engineer? Runway is 11 months at $28k/mo net
> burn; adding $15k/mo of salary drops it to 7 months. That's tight but
> workable."*

The honest version:

> *"$180k base × 1.30 loading = $234k/year fully-loaded, or $19.5k/mo.
> Ramp lag: 8 weeks to start (payroll from month 3), another 12 weeks
> to full productivity (contribution from month 6). Founder-time cost:
> ~2 hours/week of my time at $150/hr loaded = $1.3k/mo. Tooling
> step-up: crossing 10 employees, ~$500/mo. Total marginal burn from
> month 3: ~$21k/mo. Runway on net burn drops from 11 months to
> ~6 months once they're on payroll. Runway on gross burn drops from
> 7.4 to 5.0. Am I willing to bet the delta on this hire producing
> before month 6?"*

Those are different decisions. The naïve one hires; the honest one
often waits a month, negotiates the offer differently, or delays the
next non-critical hire to make room.

## The four common wrong versions

Four ways this decision gets modeled wrong, in decreasing order of
frequency:

- **Using base salary as the burn number.** The most common lie. A
  $180k hire is not a $15k/mo burn increase; it's closer to $19–20k
  once loaded, and closer to $21–22k once knock-ons are included.
- **Assuming productivity from month 1.** The offer letter says "start
  date March 1" and the model says "revenue impact March 1." No.
  Assume ramp; if you're wrong on the upside, the model just aged
  well.
- **Ignoring founder-time cost.** The tenth report is the founder's
  entire management week. That is a real cost, and modeling it at
  zero conceals a step-change in the founder's capacity that will
  eventually force a management hire.
- **Ignoring tier step-functions.** The tenth hire that crosses the
  Slack tier, the HR-broker threshold, or the payroll-software band
  is more expensive than the ninth by more than one salary.

## Summary

- **Fully-loaded cost** — `base × 1.25–1.4×` for a US hire on typical
  benefits — is the number that hits the account, not the salary. The
  right multiplier for your company comes from summing your actual
  benefit and overhead lines, not from the rule of thumb.
- **Ramp lag** — 6–12 weeks to start and another quarter or two to
  productivity — means the payroll clock and the contribution clock
  are not the same clock. Model both.
- **Knock-on costs** — founder-management time, per-seat tool tiers,
  and HR / finance / legal step-functions at ~10, ~25, and ~50
  employees — are why the tenth hire is more than 10× the first.
- Together these three corrections turn a hiring decision from a
  salary question ("can we afford it?") into a **runway-and-timing**
  question ("what does this cost the model, when does the cost start,
  and when does the contribution catch up?").

**Next:** how all of this comes together into a month-by-month
operating model with a zero-cash date, in
[chapter 04](./04-eighteen-month-operating-model.md).
