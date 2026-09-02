# Chapter 04 — Post-Money SAFE Conversion Math: The Amount / Cap Invariant

> **Reads with:** module objective 3 (arithmetic half) — *compute
> how a post-money SAFE converts using the `SAFE amount / post-money
> cap = ownership %` invariant.*

## The invariant

For a **post-money SAFE**, the SAFE holder's ownership at
conversion is deterministic the moment the SAFE is signed:

```
SAFE holder's ownership % = SAFE amount / post-money cap
```

That percentage is fixed — regardless of how many other SAFEs
are on the stack, regardless of whether the option pool is
refreshed at the priced round, regardless of what price the new
money enters at. It is the whole reason post-money SAFEs
displaced pre-money SAFEs after 2018: they let the founder,
the SAFE holder, and everyone else at the table know, in advance,
exactly what fraction of the company has already been sold.

That invariant is stated in Y Combinator's *SAFE User Guide* and
is what the 2018 revision was designed to make true.
<!-- needs-research: primary-source citation for the amount/cap invariant; Y Combinator's *SAFE User Guide* (post-2018) is the primary source. -->

Concretely:

- **$500k SAFE at a $5M post-money cap** → 10% at conversion.
- **$250k SAFE at a $2.5M post-money cap** → 10% at conversion.
- **$1M SAFE at a $10M post-money cap** → 10% at conversion.

All three convert to the same 10%. Cap dominates check size; a
low cap is a large percentage sold at a small dollar amount.

## What "at conversion" actually means — three snapshots

The invariant fixes the SAFE holder's ownership *at conversion*.
It is worth being precise about which snapshot of the cap table
that refers to, because there are three snapshots at the priced
round and confusing them is where founders lose track of their
own dilution:

- **Pre-round FD.** The cap table the day before the priced round
  closes — founders' common, option pool as of today, no SAFEs
  yet converted. The SAFE sits **off** this snapshot; it is a
  contractual claim waiting for the trigger.
- **Pre-new-money FD** (also called **"post-conversion,
  pre-money"**). The cap table *after* all SAFEs convert *and*
  after any pool refresh required by the round, but *before* the
  new-money investor's shares are issued. This is the snapshot
  the post-money SAFE invariant refers to: the SAFE holder owns
  `amount / post-money cap` of **this** table.
- **Post-close FD.** The cap table after the new-money investor's
  shares are issued. Every pre-new-money holder — founders,
  converted SAFEs, and pool — is diluted by exactly the
  new-money percentage.

The invariant is a claim on the **middle snapshot**. To read what
the SAFE holder ends up owning **at close**, you have to dilute
that snapshot by the new money.

## Stack-adjacent form — what happens after the new money is added

If the SAFE's fixed ownership of the pre-new-money FD is `s` and
the new-money ownership of the post-close FD is `r`, then after
the priced round the SAFE holder owns roughly:

```
final SAFE ownership ≈ s × (1 − r)
```

Worked example: a $500k SAFE at a $5M cap (`s = 10%`) at a priced
round where new money is 20% (`r = 20%`) ends up at
`10% × (1 − 20%) = 8%` of the post-close cap table.

The same shape applies to every pre-new-money holder, not just
SAFEs. Each pre-money percentage becomes `pre × (1 − r)`
post-close. That is why the new money's percentage is exactly
`r` and every other row's percentage adds up to `(1 − r)`.

## A stack of SAFEs sums

Because each post-money SAFE's ownership is fixed at signing, a
stack of them **adds up linearly**:

```
total SAFE stack ownership = Σ (SAFE amount_i / post-money cap_i)
```

Four $250k SAFEs at $5M post-money caps are, together, `4 × ($250k /
$5M) = 20%` of the pre-new-money FD table — the same as a single
$1M SAFE at the same cap.

The linear-sum property is a **founder tool**, not an
investor-side gotcha. It lets you count, at any moment, exactly
how much of the company you've already promised. If you can't do
that sum on the back of an envelope, you're raising SAFE by SAFE
without a running total, and the surprise arrives at the priced
round.

Two caveats to the linear sum:

- **Different caps sum on the same principle**, but each SAFE
  contributes `amount_i / cap_i`. A $500k SAFE at $5M (10%) plus
  a $300k SAFE at $6M (5%) is 15% of the pre-new-money FD.
- **Pre-money SAFEs do not sum linearly.** They interact with
  each other at conversion in ways the post-money form was
  designed to eliminate. If your stack mixes pre-money and
  post-money SAFEs, the math gets substantially harder and
  usually needs a spreadsheet or a cap-table service. If your
  stack is all post-money, the sum is a running total on a
  sticky note.

## What the invariant does not fix

The invariant fixes the SAFE holder's percentage of the
**pre-new-money FD**. It does *not* fix:

- **Ownership at close.** That is `s × (1 − r)` after the new
  money is added.
- **The pool refresh.** If the priced round requires a pool
  refresh, the pool comes out of the pre-new-money holders'
  stake — including the just-converted SAFE holder's stake.
  The SAFE holder still owns `s` of the pre-new-money FD, but
  the founders now own a smaller percentage of that same
  pre-new-money FD than they would have without the refresh.
  Chapter 05 walks the pool-refresh math.
- **Anti-dilution and later-round dilution.** Every future round
  will further dilute the SAFE-converted shares just like any
  other preferred. The invariant is about the SAFE's *entry*
  point, not its lifetime ownership.

## Converting shares — the mechanical steps

At the priced round, the mechanical steps to convert a post-money
SAFE (worked as though your cap-table software isn't doing it for
you) are:

1. **Compute the target ownership.** For each SAFE:
   `s_i = SAFE amount_i / post-money cap_i`.
2. **Compute the pre-new-money FD share count** — the total
   number of FD shares you want to exist *after* SAFEs
   converted and any pool refresh, but *before* new money is
   added. This step often solves a small system of equations
   because the pool refresh target (e.g., "pool = 10% of
   post-close FD") depends on the post-close FD share count.
3. **Compute each SAFE's share count** as `s_i × pre-new-money
   FD share count`. Add those rows to the FD table.
4. **Compute the new-money shares** — `round amount / price per
   share`, where `price per share = pre-money valuation /
   pre-new-money FD share count`. Add the new-money row to the
   FD table.
5. **Compute every FD %** as `owner FD shares / post-close FD
   share count`. Sum to 100.0%.

Cap-table software runs this in the background. When it produces
a number you don't recognise, this is the sequence to walk by
hand — it will always reproduce.

## Discount interacting with cap

The invariant `SAFE amount / post-money cap` assumes the cap
binds. If the SAFE also has a **discount** and the priced round
comes in below the cap:

- Compute the **effective price** the SAFE gets: `min(round price
  per share × (1 − discount), price implied by the cap)`.
- The SAFE's share count is `SAFE amount / effective price`.

At almost every seed round, the cap binds much harder than the
discount, so the discount clause never gets exercised. The
discount matters most on **cap-less SAFEs** (rare in the US)
and in **down-round** scenarios where the priced-round valuation
comes in below the SAFE's cap.

## MFN swaps at the moment of conversion

If a SAFE has an **MFN clause** and the company has issued a
later SAFE with more favourable terms, the earlier SAFE holder
may **elect** those terms before conversion — swapping their
$5M cap for the later SAFE's $3M cap, for example.

Founder-important consequences at the conversion moment:

- **Every MFN election increases the elected holder's
  percentage** at conversion (because the cap is lower, the
  invariant makes their `amount / cap` larger).
- **Every dollar of MFN-elected uplift comes out of the founders'
  and other non-electing holders' pre-new-money percentages.**
  New money is still `r`; MFN moves the pie inside the
  pre-new-money slice.

MFN elections are rare, but when they happen at a priced round,
they can produce several percentage points of surprise dilution.
Read the MFN clauses on every SAFE before you issue a later one
at a lower cap.

## The four common wrong versions

- **Applying the post-money invariant to a pre-money SAFE.**
  Doesn't work. Pre-money SAFEs interact with each other at
  conversion; use a cap-table service or a systematic spreadsheet.
- **Counting SAFEs at their nominal caps without summing.** Four
  $250k SAFEs at $5M is 20%, not "just one 5% SAFE at a time."
  Sum the stack.
- **Confusing pre-new-money with post-close.** The SAFE holder's
  fixed percentage is 10% of the pre-new-money FD; at close,
  after the new-money row is added, they own `10% × (1 − r)`.
  Both numbers are true; use the right one for the question
  you're answering.
- **Forgetting the pool refresh sits inside the pre-new-money
  FD.** The refresh dilutes the founders and (indirectly) the
  SAFE holder's *share of the founders' post-close pool*, even
  though the SAFE's own fixed percentage doesn't move. Chapter
  05 works this through.

## Summary

- **`SAFE holder's ownership % = SAFE amount / post-money cap`**
  is the invariant for post-money SAFEs. Fixed at signing;
  applies to the **pre-new-money FD** at the priced round.
- After the new money is added, the SAFE holder owns
  `s × (1 − r)` of the post-close FD — where `s` is the
  invariant and `r` is the new money's post-close ownership.
- **Stacks of post-money SAFEs sum linearly**: `Σ (amount_i /
  cap_i)`. Cap dominates check size for founder dilution — a
  low cap is a large percentage sold at a small dollar amount.
- Discount clauses matter most on cap-less SAFEs and in
  down-round scenarios. **MFN elections** at conversion can
  produce surprise dilution when a later SAFE has better
  terms.
- **Pre-money SAFEs do not sum linearly** and are the reason
  the 2018 post-money form was invented. If your stack mixes
  forms, use cap-table software.

**Next:** the option pool — how to size it against the mod-003
hiring plan (not the round-number counsel typed first), why the
pre-money refresh convention makes founders pay for it, and how
to defend a smaller pool at the term sheet — in
[chapter 05](./05-option-pool-sizing-and-who-pays.md).
