# Chapter 03 — SAFE Anatomy: Cap, Discount, MFN, and the Pre-Money vs Post-Money Form

> **Reads with:** module objective 3 — *understand a SAFE (Y
> Combinator, 2013; post-money form, 2018) — valuation cap,
> discount, MFN, pre-money vs post-money form.*

## Why the SAFE exists

A priced equity round is expensive to close. It requires a
signed term sheet, a certificate of incorporation amendment, a
stock purchase agreement, an investor rights agreement, a right of
first refusal / co-sale agreement, and — for institutional rounds
— a voting agreement. Each of those documents is negotiated by
counsel on both sides, and the total legal cost at a real seed
round is measured in tens of thousands of dollars and weeks of
elapsed time.

Y Combinator introduced the **SAFE** (Simple Agreement for Future
Equity) in **2013** as a way to close early checks in days rather
than months, on paperwork short enough that a founder can read it
in one sitting. The SAFE is one document, a handful of pages,
with a handful of variables. That was the whole design goal.

In **2018**, YC published a substantial revision: the **post-money
SAFE**, which changed the meaning of the valuation cap in ways
this chapter will make precise. Both forms are still in
circulation on the stack of any company that has been raising
since 2015; you have to be able to read both.
<!-- needs-research: primary-source citation for SAFE history (2013 launch, 2018 post-money revision); Y Combinator's SAFE Financing Documents page (ycombinator.com/documents) and *SAFE User Guide* are the primary sources. -->

## What a SAFE is (and is not)

A SAFE is a **contract**. It gives an investor the right to
receive shares in the company at the *next* priced equity round,
at a price determined by the SAFE's terms. It is:

- **Not debt.** No maturity date, no interest rate, no repayment
  obligation. If the priced round never happens, the SAFE
  never converts, and the investor is not entitled to their money
  back.
- **Not equity yet.** No shares are issued at signing. The SAFE
  holder is not a shareholder of record, does not vote, does not
  hold a certificate. They hold a contractual right to future
  shares.
- **Automatic on conversion.** When the qualifying priced round
  closes, the SAFE converts on its own terms — no additional
  negotiation, no separate signature. That's the whole reason it
  moves fast.

Four terms carry almost all the weight for founder dilution:
**valuation cap**, **discount**, **pre-money vs post-money form**,
and (much less often) **MFN**. Two more mechanics — pro-rata
rights and side letters — are worth naming so the founder counts
them at the round.

## Valuation cap — the ceiling on the SAFE holder's price

The **valuation cap** is the maximum valuation at which the SAFE
converts. It sets a *floor* on the SAFE holder's ownership: the
lower the priced-round valuation, the closer the SAFE holder
converts to the cap; the higher the priced-round valuation, the
more the cap binds and the more shares per dollar the SAFE
holder gets relative to a Series Seed dollar.

A worked example:

- A $500k SAFE at a **$5M cap**. Priced round comes in at a **$5M
  valuation**. Cap and round agree; SAFE holder converts at
  $5M, gets 10% of the pre-new-money FD table
  (`$500k / $5M`), same as a Series Seed investor at that price.
- Same SAFE. Priced round comes in at a **$20M valuation**. Cap
  binds; SAFE holder converts at the $5M cap (not the $20M
  round), so their $500k buys the ownership that $500k at $5M
  would buy — **4× more shares per dollar** than a Series
  Seed investor entering at $20M.
- Same SAFE. Priced round comes in at a **$2M valuation** (a
  down-round scenario). Cap is higher than round; cap doesn't
  bind; SAFE holder converts at $2M, same price as the new
  investor. The **discount** clause (if any) may still apply.

The cap is the single largest driver of founder dilution from a
SAFE. Chapter 04 makes the arithmetic mechanical.

## Discount — a percentage off the round's share price

The **discount** is a percentage off the priced-round share price
— commonly **10–20%**. A 20% discount at a $10M priced round
converts the SAFE at an effective $8M price.

Discount and cap coexist. The SAFE terms say: **whichever gives
the SAFE holder more shares wins.** If the cap binds harder than
the discount, the cap wins. If the discount produces a lower
effective price than the cap, the discount wins. In practice, at
seed, the cap almost always binds harder; discounts matter more
on cap-less SAFEs (which are rare in the US since ~2015).
<!-- needs-research: primary-source citation for the shift away from cap-less SAFEs in the US market; Carta's private-market data and Y Combinator's SAFE User Guide are the anchors. -->

## Pre-money vs post-money form — the load-bearing distinction

The single biggest change in the SAFE's ten-year history is the
2018 revision from the **pre-money form** to the **post-money
form**. The two forms use the same word — "valuation cap" — to
mean different things, and a founder who conflates them will
misread their own dilution by a wide margin.

- **Pre-money SAFE (2013 original).** The cap refers to a
  valuation *before* other SAFEs converted at the round. When
  multiple pre-money SAFEs sit on the stack, each SAFE's
  ownership depends on how *all* of them convert together — an
  interlocking calculation that is hard to do in your head, hard
  to explain to an investor, and prone to producing more
  dilution than the founder expected. YC's own retrospective is
  that the pre-money SAFE created ambiguous math in exactly the
  scenario it was designed for (a stack of small pre-seed
  checks). The pre-money SAFE is still legal, but it is the
  wrong choice for new checks.
  <!-- needs-research: primary-source citation for YC's 2018 statement on why the pre-money SAFE produced ambiguous math; Y Combinator's *SAFE User Guide* (post-2018) is the primary source. -->
- **Post-money SAFE (2018 revision).** The cap refers to the
  **post-money valuation** *including all SAFEs converted* but
  *before* the new-money priced round. The consequence is
  arithmetic that is deterministic the moment the SAFE is
  signed:

  ```
  SAFE holder's ownership at conversion = SAFE amount / post-money cap
  ```

  That relationship is fixed at signing and does not depend on
  what other SAFEs the company issues later or on whether the
  pool is refreshed at the priced round. Chapter 04 walks the
  arithmetic.

Nearly every SAFE written since 2019 is the post-money form.
Pre-money SAFEs still on the stack of an older company are worth
reading carefully; the two forms sit alongside each other with
identical-looking front pages and materially different math.

## MFN — most favored nation

The **MFN clause** ("most favored nation") says: if the company
issues a **later SAFE** with more favourable terms — lower cap,
higher discount, or better rights — this earlier SAFE holder can
**elect** to swap into those terms instead of keeping their
original ones.

MFN is common in early angel and pre-seed checks. It solves the
first-check problem: an angel who writes an early $50k check at a
$5M cap doesn't want to be worse off than a $50k check written a
month later at a $3M cap. MFN lets the earlier holder catch up
without renegotiating.

Two founder-important details:

- **MFN elections happen at future SAFE issuances**, not
  automatically. The SAFE holder has to actually notice and
  elect (or the company has to notify them, depending on the
  clause's wording).
- **MFN is scoped by the clause language**. Some MFN clauses
  apply to any future SAFE, some to only larger SAFEs, some
  only to caps and not to discount. Read the clause; do not
  assume the standard.

## Pro-rata rights — the option to defend ownership at the priced round

Some SAFEs — typically those from **institutional pre-seed funds**
— carry a **pro-rata right**: the SAFE holder can invest their
pro-rata share of the *next* priced round to maintain the
ownership percentage they held immediately after conversion.

Pro-rata is not universal on angel SAFEs. When a pre-seed fund
writes a $500k SAFE and asks for pro-rata, that fund is
signalling that they intend to keep buying — and that the founder
needs to leave room for them at the Series Seed and Series A
tables.

Pro-rata is often broken out into a **side letter** — a document
attached to the SAFE that contains investor-specific terms not
appearing on the SAFE form itself. Which brings us to:

## Side letters — where investor-specific terms hide

A **side letter** is a document attached to a SAFE (or a priced
round) that adds investor-specific terms without altering the
underlying form. Common contents:

- **Pro-rata rights** — as above.
- **Information rights** — regular financial and operational
  reporting, sometimes an inspection right.
- **MFN scope** — expanding or narrowing which future SAFEs
  trigger MFN.
- **Board observer seats** at pre-seed (rare, but they appear).

When counting the cap table, **read the side letters too**. The
SAFE form tells you what fraction converts; the side letter tells
you what obligations the company has to that holder between now
and conversion.

## Reading a SAFE — the mental checklist

When a SAFE lands on your desk, extract these fields into your
SAFE-stack row:

- **Investor** and **amount** invested.
- **Valuation cap** (numeric) or **uncapped** (rare, but worth
  flagging).
- **Discount** (percentage, or none).
- **Form** — pre-money or post-money.
- **MFN** — yes / no, and (if yes) the scope of the clause.
- **Pro-rata** — yes / no, in the SAFE or in a side letter.
- **Any other side-letter terms** — information rights,
  observer seats, notification rights.
- **Fixed ownership at conversion**, computed from the
  post-money-SAFE invariant (`amount / cap`) if the SAFE is
  post-money form.

That row belongs beneath your FD cap table, permanently, until
the SAFE converts.

## The four common wrong versions

- **Pre-money and post-money confused.** Founder computes
  `amount / cap` on a pre-money SAFE as if the invariant applied.
  It doesn't; pre-money SAFEs interact with each other in
  non-obvious ways at conversion.
- **Cap and discount interaction ignored.** Founder computes
  ownership from the cap and misses that the discount produces
  a lower price and more shares.
- **MFN counted as automatic.** Founder issues a later SAFE at
  a lower cap without checking whether the earlier holders'
  MFN clauses trigger. Earlier holders elect; ownership shifts
  more than expected.
- **Side letters missed.** Founder counts the SAFE and misses
  the pro-rata right; at the priced round, the pre-seed fund
  exercises pro-rata and takes more of the round than the
  founder budgeted for.

## Summary

- The **SAFE** (YC, 2013; post-money form, 2018) is a
  short-form contract that gives an investor the right to
  receive shares at the next priced round on the SAFE's terms.
  It is not debt and it is not equity yet.
- Four terms drive founder dilution: **valuation cap** (the
  ceiling on the SAFE holder's price), **discount** (a
  percentage off the round's price), **form** (pre-money or
  post-money — the load-bearing distinction), and (much less
  often) **MFN**.
- **Post-money form** makes ownership deterministic at signing:
  `SAFE amount / post-money cap = SAFE holder's ownership at
  conversion`. Nearly all SAFEs written since 2019 are
  post-money.
- **Pro-rata rights and side letters** carry investor-specific
  terms that don't appear on the SAFE form. Read them; count
  them in your SAFE stack row.

**Next:** the arithmetic of a post-money SAFE conversion — the
`amount / cap` invariant, how a stack of SAFEs sums, and the
stackable form that shows what happens after the priced round's
new money is added — in
[chapter 04](./04-post-money-safe-conversion-math.md).
