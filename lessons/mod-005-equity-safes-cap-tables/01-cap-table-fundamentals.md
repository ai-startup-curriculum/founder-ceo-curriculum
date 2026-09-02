# Chapter 01 — What a Cap Table Actually Is: Issued, Fully Diluted, and Ownership Arithmetic

> **Reads with:** module objective 1 — *read a cap table (common,
> preferred, options (issued and reserved), SAFEs and convertibles
> on the stack) and compute ownership through a round on a
> fully-diluted basis.*

## A ledger of every promise about ownership

A capitalization table — the "cap table" — is the company's
ledger of **every equity claim on the business**. It answers a
single question, per stakeholder, at a single instant in time:
*if the company were to distribute all of its ownership right
now, what percentage would you get?*

That sounds simple until the cap table has a mix of issued shares,
reserved options, and SAFEs sitting on the stack — three
categorically different things that all show up in the same
denominator when it matters. Founders who read only the "who
holds shares today" view will over-report their own ownership by
a wide margin and miss the dilution baked in by the promises the
company has already made.

The rest of this chapter is the shortest working definition of a
cap table that leaves no room for that mistake.

## Issued vs fully diluted — the two views that matter

Every cap table has (at least) two views:

- **Issued.** Shares that a person or entity actually holds
  *today*. Founders' common, options actually granted and
  outstanding (whether vested or not), preferred stock from
  priced rounds, any warrants exercised. Issued shares are what a
  cap-table service like Carta or Pulley shows at the top; they
  are the number that appears on the stock certificate.
- **Fully diluted (FD).** Every share that *would* exist if every
  reserved-but-not-granted option were granted, every SAFE and
  convertible note converted at its expected terms, and every
  warrant exercised. FD is the number an investor cares about,
  because it is the denominator that determines ownership after
  the next round closes.

The **fully-diluted share count** is the load-bearing number for
founder decisions in this module. Every percentage in the rest of
the module is `owner FD shares / total FD shares`, unless the text
explicitly says otherwise.

Two subtleties trip founders reading their own cap table for the
first time:

- **Reserved options count.** The un-granted portion of the option
  pool sits in the FD share count even though no employee holds
  it yet. Investors will not let you exclude it; the pool exists
  precisely so you *can* grant it, and the moment you do, those
  shares are outstanding.
- **SAFEs and notes count — but at their *expected* conversion.**
  A post-money SAFE at a $5M cap for $500k contractually converts
  to 10% of the pre-new-money FD table at the next priced round.
  Prior to that round, well-run cap-table software shows the SAFE
  either as an off-table stack (with the fixed ownership it will
  claim at conversion) or as a modelled row in a "next-round
  scenario" view. Either way, the founder cannot pretend the
  10% doesn't exist just because the shares haven't been
  issued yet.

## Ownership arithmetic — the one formula

The universal rule is:

```
ownership % = owner FD shares / total FD shares
```

Applied consistently, it is enough to walk a company from founding
through a Series A. Applied *inconsistently* — pool sometimes
included, sometimes not; SAFEs counted at conversion in one row
and ignored in the next — it produces numbers that don't sum to
100% and a founder who can't defend their own dilution.

A useful sanity check after every step: **sum every stakeholder's
FD % across the table.** It must sum to `100.0%` (up to rounding
in the last decimal place). If it doesn't, someone is miscounted
or an instrument is missing. Do this after every row change,
before moving on. The discipline is the price of getting the walk
right the first time.

## Dilution is arithmetic, not punishment

When the FD share count grows — a pool refresh, a SAFE conversion,
a new priced round — every non-purchaser's percentage moves *down*
even though their share count didn't change. That movement is
**dilution**, and it is not optional. Every share issued to
someone new dilutes everyone else.

The founder-important corollary: **dilution is only meaningful in
context of what the new shares bought.** Selling 20% of the company
for $2M to a Series Seed lead who buys 18 months of runway and
opens the Series A door is a good trade. Selling 20% for $2M to a
party round of angels who add nothing beyond the check is the same
arithmetic and a worse trade. The cap table records both
identically; the founder's judgement about which is which is what
this module is really trying to build.

## The four instruments you have to be able to read

At seed stage, four instruments cover virtually every cap-table
row. Chapter 02 goes through them in depth; here they exist as
labels so the arithmetic in this chapter has referents:

- **Common stock** — what founders and employees hold.
- **Preferred stock** — what priced-round investors get.
- **Options** — issued (granted) and reserved (unallocated pool).
- **Convertibles on the stack** — SAFEs and notes, off the table
  today but with a fixed claim at conversion.

Occasional additional rows — **warrants** (rights to buy shares at
a stated price, typically issued to venture-debt lenders or as
part of an advisor grant), **secondary common** (from a founder
tender to a later-stage investor), various stock-plan mechanics —
appear at Series A and later. This module treats them as
exceptions to be flagged, not as first-class rows.

## What a first cap table actually looks like

At founding, the simplest possible FD cap table has one row per
founder, one row for the option pool (usually zero shares
reserved at incorporation), and a total.

```
| Stakeholder      | Shares (issued) | Shares (FD) | FD %  |
| Founder A        | 5,000,000       | 5,000,000   | 50.0% |
| Founder B        | 5,000,000       | 5,000,000   | 50.0% |
| Option pool      | 0               | 0           |  0.0% |
| Total FD                                          100.0% |
```

Absolute share counts are arbitrary at founding. The convention
is to issue **10,000,000 shares total** so that later grants have
enough fractional granularity — a 0.25% advisor grant is 25,000
shares, which is easier to talk about than 250. The percentages
are what matter; the raw share counts are just a scaffold that
lets you do integer arithmetic without decimals.

Even at founding, add the **option pool row with 0 shares** so it
is on the table when the refresh lands. Every seed-stage cap table
has a pool row; better to see it as a zero than to add it under
time pressure at the round.

## The five errors that break a cap table

Five specific mistakes cause almost every "why doesn't my cap
table sum to 100%?" scramble the night before a term sheet lands:

- **Issued-only counting.** Founder computes ownership as `my
  common / total common issued`, ignoring the pool and any
  converted SAFEs. Fix: switch to FD every time.
- **Pool double-counted or missing.** Pool is either not on the
  table or is on the table twice (once as reserved and again as
  granted). Fix: a single "options" section with two rows —
  granted, reserved.
- **SAFE ignored until the round.** Founder treats a SAFE as
  "off-cap-table" not just formally but in their own head, and
  is surprised when the pre-new-money FD suddenly includes 10%
  of SAFE holders. Fix: keep an explicit "SAFE stack" section
  with each SAFE's amount, cap, form, and fixed ownership at
  conversion (see chapter 04).
- **Pre-money and post-money confused.** Founder computes
  ownership using a pre-money share count but a post-money
  valuation, or vice versa. Fix: label every column
  "pre-new-money" or "post-close" and check that the two never
  mix on the same row.
- **Rounding errors compound.** Each row is rounded to one
  decimal place; totals no longer sum to 100.0%. Fix: keep
  raw share counts as the source of truth; compute percentages
  from them at every step, never percentages of percentages.

## What "reading a cap table" actually looks like in practice

A working founder, handed a cap-table export, can answer these
questions in under five minutes:

- What is the **total FD share count** — the denominator for
  everything else?
- What percentage does **each founder** own on an FD basis, right
  now?
- How many shares are in the **option pool**, and what percentage
  of FD does that represent — granted vs reserved?
- What is the **SAFE stack** — how many SAFEs, what caps, what
  forms (pre-money or post-money), what fixed ownership at
  conversion?
- What is **already promised** on an FD basis at the *next*
  priced round, before the new-money investor writes a dollar?

If you can answer all five of those from your own cap table today,
the rest of this module is scaffolding. If any answer is a
guess or requires opening a spreadsheet you can't read, this is
the founder-level skill the module exists to build.

## Summary

- A cap table is the ledger of **every equity claim** on the
  company — issued shares plus every promise that becomes shares
  under some future condition.
- The load-bearing view for founder decisions is **fully diluted**:
  `owner FD shares / total FD shares`. Every percentage in this
  module uses that formula.
- **Dilution is arithmetic**, not punishment. Every share issued
  to someone new dilutes everyone else; the founder question is
  whether the trade the new shares bought is worth what they
  cost.
- Sum FD % across the table after every row change. If it doesn't
  sum to 100.0%, fix it before moving on. That discipline is
  what separates a founder who can read a cap table from one
  who thinks they can.

**Next:** the four share classes on an early-stage cap table —
common, preferred (with its default rights), options, and
convertibles on the stack — in
[chapter 02](./02-four-share-classes.md).
