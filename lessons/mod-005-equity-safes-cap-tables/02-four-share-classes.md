# Chapter 02 — The Four Share Classes on an Early-Stage Cap Table

> **Reads with:** module objective 2 — *distinguish the four
> early-stage share classes: common (founders + employees),
> preferred (priced-round investors, with 1× non-participating
> liquidation preference and broad-based weighted-average
> anti-dilution as defaults), options (issued + reserved in the
> option pool), and convertibles (SAFEs + notes) on the stack.*

## Different rows, different rights

The cap table has one column for "shares." Founders new to the
mechanics often assume that column is homogeneous — a share is a
share. It isn't. **The share class determines what a shareholder
is entitled to** at exit, in a down round, when a major decision
comes up for a vote, and — for convertibles — whether they hold
"shares" at all.

Four classes cover almost every seed-stage cap table:

1. **Common stock** — what founders and employees hold.
2. **Preferred stock** — what priced-round investors get.
3. **Options** — grants to employees and advisors, issued or
   reserved.
4. **Convertibles on the stack** — SAFEs and notes, not shares
   yet.

Two later-stage classes (**warrants** and various stock-plan
mechanics) appear as exceptions. Everything in this chapter is
about what makes each of the four load-bearing classes different
from the others and why the difference matters for founder
decisions.

## Common stock — founders and employees

**Common stock** is the residual equity in the company. Common
holders are last in line at exit — they get what's left after
every debt is paid, every preference is satisfied, and every
senior class of shares has taken its share. In exchange, they
have the largest **upside**: every dollar above the sum of
preferences is distributed pro rata across the fully-converted
share count, and common is the largest share of it.

Common is:

- **What founders receive** at incorporation, usually subject to
  a **vesting schedule** (four years, one-year cliff is the modal
  default) so that a co-founder who leaves in year 1 doesn't walk
  away with the whole equity stake.
- **What options grant the right to purchase.** Options are not
  shares themselves — they are a right to buy common at a fixed
  **strike price**, exercisable when the option vests. When
  exercised, the option becomes a common share.
- **Junior in liquidation preference** to every class of
  preferred. If the company sells for less than the sum of
  preferences, common holders receive **nothing** in most cases.
  This is the single most consequential fact about common stock
  and the whole reason preferred exists as a category.

Vesting mechanics — cliff, acceleration on change of control,
"good leaver" vs "bad leaver" clauses — belong to a founder
agreement and to the employee stock plan, and they are important
enough that they warrant their own reading. This module treats
vesting as a fact of common stock rather than teaching the
mechanics.
<!-- needs-research: primary-source citation for the 4-year vest / 1-year cliff modal default; Y Combinator's founder-agreement templates and Cooley GO's model documents are common anchors. -->

## Preferred stock — priced-round investors, with defaults that matter

**Preferred stock** is what priced-round investors receive. At
seed, this is usually a lightweight **Series Seed** or
**Series A Preferred** class; at Series A and later, each round
typically gets its own series (Series A, Series B, ...), each
with its own price per share and its own preference stack.

Preferred is called "preferred" because it has **rights common
doesn't**. Two of those rights land directly in the cap-table
math and are worth naming here so chapter 08 can treat them at
depth:

- **Liquidation preference.** The default is **1× non-participating
  preferred**: at exit, preferred gets its money back first (`1×
  the amount invested`), then it *converts to common* and shares
  the remaining upside pro rata. "Non-participating" means the
  preferred does not double-dip — it takes *either* the
  preference *or* the pro-rata common share, whichever is larger,
  not both. Anything more aggressive — a `2×` preference, or
  **participating preferred** where the investor takes their
  money back *and* participates in the upside — is money coming
  out of the founders' and common holders' pocket at exit.
  <!-- needs-research: primary-source citation for the 1× non-participating default; Brad Feld & Jason Mendelson's *Venture Deals* and the NVCA model documents (nvca.org/model-legal-documents) are the canonical references. -->
- **Anti-dilution.** The default is **broad-based
  weighted-average**: if the company later issues shares at a
  lower price per share (a "down round"), the preferred holder's
  conversion price is adjusted downward *by a formula that
  weights the size of the down round against the whole
  post-conversion FD share count*. This slightly increases the
  preferred holder's share of the company but does not devastate
  the common. **Full-ratchet** anti-dilution — the punitive
  alternative — resets the preferred's conversion price to the
  new low price *regardless of round size*, which can transfer
  most of the company from common to preferred in a single down
  round. Chapter 08 works through the math.
  <!-- needs-research: primary-source citation for the broad-based weighted-average default; *Venture Deals* and NVCA model documents are the canonical references. -->

Preferred stock also carries **consent rights** on major decisions
— sale of the company, issuance of new senior stock,
capital-structure changes — encoded as **protective provisions**
in the certificate of incorporation. These are not cap-table
rows, but they shape which decisions the founder can make
unilaterally and which require investor approval.

## Options — issued and reserved

**Options** grant the right to purchase common at a fixed strike
price, usually equal to the fair market value of the common on the
grant date (in the US, established by a **409A valuation** —
covered in [chapter 10](./10-boundaries-finance-and-cap-table-craft.md)
as a deferred boundary).
<!-- needs-research: primary-source citation for 409A valuation mechanics; IRS regulations under Internal Revenue Code §409A and standard valuation methodology (income / market / asset approaches) are the anchors. -->

On the cap table, options appear as **two rows** in the FD table:

- **Issued (or "granted") options.** Options actually promised to
  a named person — employee, advisor, or contractor. Subject to
  a **vesting schedule** (four years with a one-year cliff is
  the modal default at seed), so a grantee who leaves in year 1
  vests zero shares. Vested-but-unexercised options are shares
  the grantee has earned the right to buy but has not yet paid
  for; they still count in the FD share count.
- **Reserved options** (the "option pool" or "unallocated pool").
  Options set aside for future grants but not yet promised to
  anyone. Reserved options count in the FD share count *even
  though no one holds them yet* — that is why the pool
  dilutes.

The pool is sized at ~10–15% of the post-money FD cap table at
seed and refreshed at each priced round. Chapter 05 covers
sizing, refresh, and who pays for it in depth.

Two option-mechanic details worth flagging:

- **ISOs vs NSOs.** In the US, options come in two tax flavours —
  **Incentive Stock Options** (ISOs, employee-only, favorable
  tax treatment on qualifying dispositions) and **Non-Qualified
  Stock Options** (NSOs, granted to employees, advisors, and
  contractors, with less favourable tax treatment). The
  distinction matters to the grantee's tax planning and to the
  company's stock-plan administration; it does not change the
  cap-table math. Deferred to the finance track.
  <!-- needs-research: primary-source citation for ISO / NSO tax treatment; IRS Publication 525 and Internal Revenue Code §422 (ISOs) / §83 (NSOs) are the statutory anchors. -->
- **Early exercise and 83(b) elections.** Some employee stock
  plans allow exercise before vest, which combined with an
  **83(b) election** starts the capital-gains holding period at
  grant rather than at vest. Important to individual grantees
  and to the employee-stock-plan administration; not a
  cap-table-math item for this module.
  <!-- needs-research: primary-source citation for 83(b) elections; IRC §83(b) and IRS regulations are the anchors. -->

## Convertibles on the stack — SAFEs and notes

**Convertibles** are contracts, not shares. They give an investor
the right to receive shares at the *next* priced round, at a price
determined by the convertible's terms. Two forms dominate at
early stage:

- **SAFE** (Simple Agreement for Future Equity — Y Combinator,
  2013; post-money revision, 2018). Not debt (no maturity date,
  no interest); not equity yet (no shares issued until
  conversion). Converts automatically at the next priced round.
  Chapter 03 covers the anatomy.
  <!-- needs-research: primary-source citation for the SAFE origin and 2018 post-money revision; Y Combinator's SAFE Financing Documents page (ycombinator.com/documents) and *SAFE User Guide* are the primary sources. -->
- **Convertible note.** Debt that converts to equity at a
  qualifying financing (or matures and is repaid, in theory).
  Carries **interest** (typically 4–8% simple) and a **maturity
  date** (typically 18–24 months). Substantively similar to a
  SAFE for the founder except that a note has a real
  maturity — if the priced round doesn't happen by then, the
  note is repayable in cash (which a seed-stage company almost
  never has), and the noteholder can extend, convert at the
  cap, or (in theory) call the default. Notes are still in use
  where SAFEs are not the local convention or where an investor
  specifically wants debt treatment; SAFEs have become the
  dominant early-stage instrument in the US since roughly 2015.
  <!-- needs-research: primary-source citation for the SAFE-vs-note dominance shift; Cooley GO's convertible-note materials and Carta's private-market data are common anchors. -->

Convertibles sit **off the FD share count** until conversion —
they don't have a strike price to convert against yet, since the
price is determined by the priced round they convert *into*. Well-
run cap-table hygiene keeps a **SAFE stack section** underneath
the FD table with each convertible's amount, cap, form (pre-money
or post-money for SAFEs, plus any discount, MFN, or pro-rata side
letter), and the fixed ownership it will claim at conversion.

At the priced round, the stack **converts to preferred** (or, in
some structures, to a shadow class of preferred with slightly
adjusted rights) at the price the SAFE's terms dictate. From that
moment forward, converted-SAFE shares are just preferred shares
on the cap table.

## Warrants (rare at seed, worth naming)

**Warrants** are rights to buy shares at a stated price for a
stated period. They look like options but are typically issued to
**non-employees** — most commonly to a **venture-debt lender** as
"warrant coverage" (a small percentage of the loan amount,
exercisable at a stated price) or to an early strategic partner.

Warrants sit in the FD share count at their **expected exercise**
just like options. They are not common at pure seed stage, but
they appear at Series A and beyond, and a working founder should
recognise the row when it shows up.

## Reading the stack — the mental order

When you sit down with a cap table, read the classes in this
order:

1. **Common** — founders' and employees' issued shares.
2. **Options: granted** — issued but unexercised.
3. **Options: reserved** — the unallocated pool.
4. **Preferred, senior-most last** — Series Seed first, then A,
   then B, etc. (Most-recent series is usually senior in
   liquidation preference.)
5. **Convertibles on the stack** — every SAFE and note, with
   its cap, form, and fixed ownership at conversion.
6. **Warrants** — if any.

The **FD share count** is the sum of rows 1–4 plus 6. The
**convertibles** are additional claims that will grow that
denominator at the next priced round, when they convert.

## Summary

- Four share classes cover almost every seed-stage cap table:
  **common** (founders + employees), **preferred** (priced-round
  investors), **options** (granted + reserved pool), and
  **convertibles** (SAFEs + notes on the stack).
- Preferred stock carries **rights** that common doesn't — the
  defaults are **1× non-participating liquidation preference**
  and **broad-based weighted-average anti-dilution**. Chapter 08
  covers both in depth.
- **Options** appear as two rows in the FD table — granted and
  reserved. Reserved options dilute even though no one holds
  them yet.
- **Convertibles sit off the FD share count** until conversion,
  but a working cap table keeps them in a "SAFE stack" section
  with each convertible's terms and the fixed ownership it
  will claim at the next round.
- Reading order: common → granted options → reserved pool →
  preferred (by series, senior-most last) → convertibles →
  warrants. Sum rows 1–4 (and 6) for the FD share count;
  convertibles will grow that count at the next round.

**Next:** the anatomy of a SAFE — valuation cap, discount, MFN,
pre-money vs post-money form, and the two forms' very different
implications for founder dilution — in
[chapter 03](./03-safe-anatomy.md).
