# Chapter 01 — The Three Founder Numbers: Cash, Net Burn, Runway

> **Reads with:** module objective 1 — *compute and state, from memory,
> the three founder numbers — cash on hand, monthly net burn, runway —
> for a given month, and explain the difference between gross and net
> burn.*

## Three numbers, one obligation

Every operating founder — every month, without opening a spreadsheet —
should be able to answer three questions:

1. **How much cash do we have?**
2. **How fast are we burning it?**
3. **How long until it hits zero?**

Those three numbers — **cash on hand**, **monthly net burn**, and
**runway** — are the founder's version of a pilot's fuel gauge. They
do not tell you where to fly. They tell you whether you can still land.
Every other question in this module (should we hire, should we raise,
should we cut, should we keep going) is a question about how these
three numbers change under a decision.

The obligation is to know them from memory. If a board member, a
partner at a firm you're raising from, or a co-founder at 9pm asks
"how long do you have?" and the answer is "let me open the sheet," you
have handed over the most consequential number in the company to
whatever your spreadsheet says next time you open it. Founders who
run companies successfully own these numbers the way pilots own the
fuel gauge — checked so often the check is automatic.

## Number 1 — Cash on hand

**Definition:** the dollars in your operating bank account today.

That's the whole definition. Not:

- A signed but uncleared SAFE. Wire not landed, cash not counted.
- Receivables from a contract. Invoice not paid, cash not counted.
- A promised term sheet from an investor. Signed but unwired, cash
  not counted.
- Committed spend that hasn't hit yet. That subtracts from the number
  going forward; it does not add.
- The gross figure across three accounts if one of them is a
  merchant-holding-account holdback you can't actually withdraw. Only
  cash you could move out of the account tomorrow counts.

**Cash is only cash when it's in the account.** This is the discipline
that separates a founder who survives a wire being 30 days late from
one who is caught by it. Every startup, at least once, learns that a
"guaranteed" wire from a lead investor takes six weeks longer than
promised because the fund's LP capital call got delayed. If you spent
the money on the assumption it had already landed, you have created a
crisis out of a paperwork delay.

Two operational rules keep this clean:

- **Reconcile weekly.** Not monthly. Not "when the accountant sends
  it." A five-minute weekly check of the bank balance is enough at
  seed stage.
- **Track "committed but not paid" separately.** Signed offers you
  haven't wired yet, invoices you owe but haven't paid, contract
  minimums you're locked into. This is a second number, not a
  subtraction from cash — cash is what's in the account, and this is
  what will come out of it next.

## Number 2 — Monthly burn

**Definition:** how much cash you're consuming per month. Two flavors,
and the distinction is one of the most important disciplines in this
module.

### Gross burn

**Gross burn** is total cash *out* per month. Every dollar that leaves
the account: payroll, employer taxes, benefits, rent, hosting, tools,
contractors, legal, accounting, insurance, travel, everything.

```
gross burn = total cash out in the month
```

Gross burn tells you what the business costs to *operate*. It is not
affected by whether customers are paying you this month. It's the
number that tells you what happens if revenue disappears for a quarter.

### Net burn

**Net burn** is gross burn minus cash *in* — customer revenue that
actually hits the account, plus any other recurring inflows (that are
not funding rounds; funding is a one-time cash event, not a burn
adjustment).

```
net burn = gross burn − cash in from customers (received, not invoiced)
```

Net burn is the number that determines **runway** on a going-concern
basis. If gross burn is $42k/mo and customers are paying you $14k/mo,
net burn is $28k/mo — that's what's actually leaving the account each
month.

### Why both matter

At early stage, founders overwhelmingly quote **net burn** ("we're only
burning $28k a month") because it's the smaller, more flattering number.
That's fine — but only if you also know the gross number and would say
it just as fast if asked. Chapter 02 covers the trap in detail: if you
plan your runway on net burn and the customer revenue disappears
(churned anchor, delayed contract, single-customer concentration), your
"14 months" turns into "9 months" overnight — and the fact that you
never modeled the gross-burn floor is the reason you didn't see it
coming.

The discipline is: **quote both, plan against both, report both.**

### One accounting subtlety worth naming

"Cash in" for net-burn purposes is **cash received**, not invoiced. A
$60k annual contract that gets signed in January but paid quarterly is
$5k/month of cash in over the year — not $60k in January. And if the
customer pays late (they will), the cash landed in February is what
counts for February's net burn.

This is not GAAP revenue recognition; that's a different exercise
handled by an accountant. The founder's operating question is "what
actually hit the bank account this month," and that's what feeds burn.

## Number 3 — Runway

**Definition:** how many months until cash hits zero at your current
net burn rate.

The simplest form:

```
runway (months) = cash on hand / monthly net burn
```

If you have $310k in the bank and net burn is $42k/month, runway is
`$310k / $42k ≈ 7.4 months`. You can state that in your head. You
should be able to.

This is the **napkin runway**. It assumes burn stays constant, revenue
stays constant, and no big cash events (hires, funding, contract
starts, contract losses) happen. In reality, none of those hold — that's
why you build an operating model (chapter 04) rather than trusting the
napkin. But the napkin number is the one you carry in your head between
model updates.

Two derivative numbers worth knowing:

- **Runway on gross burn** — same calculation with gross burn in the
  denominator. This is your **floor**: how long you'd survive if
  customer revenue went to zero tomorrow. In the example above,
  `$310k / $42k gross ≈ 7.4 months`; if the customers had been paying
  $14k/mo and you were quoting `$310k / $28k net ≈ 11 months`, then
  the floor is 7.4 months, not 11. Chapter 02 makes this the primary
  stress test.
- **Zero-cash date** — the calendar month that runway lands you in.
  Runway in months is abstract; a date is not. If today is September
  and runway is 7.4 months, the zero-cash date is roughly April of
  next year. Founders who talk in months mentally push the deadline
  around; founders who talk in dates hold it fixed.

## The three-numbers monthly ritual

Every month, on a fixed date (the first business day works well), a
seed-stage founder should sit down for ten minutes and update the
three numbers:

1. **Cash on hand** — the actual bank balance, reconciled.
2. **Gross and net burn** — this month's cash out, and this month's
   cash out minus cash in.
3. **Runway** — both flavors (napkin runway and floor runway), plus
   the current zero-cash date.

Written on a single line in a shared doc or Slack, it looks like:

```
2026-09-01: $310k cash · $42k gross / $28k net · 7.4mo floor / 11.0mo
runway · zero-cash April 2027 (floor: April 2027 without customers).
```

That line is what board members read first. It is what a partner asks
about in a fundraising meeting first. It's what you defend to a
co-founder when a big spend decision is on the table.

If those three lines change materially between months (they will) the
change itself is the meeting agenda: **what got us from last month's
line to this month's?** Every big decision — a hire, a contract
signed, a contract lost, a rent bump, a tools consolidation — should
be traceable to a specific movement in one of those three numbers.

## The four common wrong versions

Four ways founders get these numbers wrong, in decreasing order of
frequency:

- **Cash includes uncleared inflows.** A signed SAFE, a promised wire,
  an invoiced-but-unpaid contract. The cash is not real yet. Do not
  spend against it, do not include it in runway math.
- **Burn quoted as net-only, without knowing gross.** The founder can
  say "$28k a month" but has to open the sheet to answer "what if the
  customer stops paying?" The gross number is the one that answers
  that question in the head.
- **Runway calculated on a stale burn number.** The last big hire
  landed a month ago, burn is now $56k not $42k, and the founder is
  still quoting last quarter's runway. The napkin only works if the
  napkin is fresh.
- **Runway held in months, not in a date.** Months are elastic in the
  head ("still plenty of runway"); dates aren't ("we run out in
  April"). Convert one to the other and use the date.

## Summary

- The three founder numbers are **cash on hand, monthly net burn,
  runway** — and every founder should be able to state them from
  memory, updated at least monthly.
- **Cash on hand** is cash *in the account* — not committed, not
  promised, not receivable.
- **Gross burn** (all cash out) tells you what the business costs to
  operate; **net burn** (gross minus cash in from customers) is what
  determines runway on a going-concern basis. Quote both.
- **Runway** in its simplest form is `cash / net burn`, but always
  paired with **runway on gross burn** as the floor, and expressed as
  a **zero-cash date**, not just a month count.
- Update the three numbers on a fixed monthly ritual. The delta from
  last month is the meeting agenda.

**Next:** why net burn alone lies to you, and how to stress-test the
model on gross burn, in
[chapter 02](./02-gross-vs-net-burn-trap.md).
