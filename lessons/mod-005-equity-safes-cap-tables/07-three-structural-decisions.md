# Chapter 07 — The Three Structural Decisions That Most Move Founder Ownership

> **Reads with:** module objective 6 — *name the three structural
> decisions in the current round that most affect founder
> ownership at the next round: pool size (not convention), SAFE
> cap and stack size, round size and pre-money together (not the
> headline).*

## Structure beats headline

Founders talk about **valuation** because it's the number in the
term sheet's first line. Investors also talk about valuation
because it's the number the round is priced at. The problem is
that "valuation" — meaning the pre-money or post-money valuation
of the priced round — is only one of three levers that determine
how much of the company the founders own at close, and it is not
usually the largest.

A **$10M pre-money at a $3M round with a 15% pool** produces less
founder ownership than a **$7M pre-money at a $2M round with a
10% pool** — even though the first "headline" is $10M and the
second is $7M. Structure decides who owns what; the headline is
the story you tell about it.

Three structural decisions carry almost all the ownership weight:

1. **Pool size** (not pool convention).
2. **SAFE cap and stack size** (the total already promised
   before the round starts).
3. **Round size and pre-money together** (the shape of the
   raise, not the headline).

Two more decisions — **liquidation preference** and
**anti-dilution** — live on the term sheet rather than in the
cap-table math itself, but they reach into the cap table at
exit and in down rounds. Chapter 08 covers them. Everything
here is the pure cap-table structural work.

## Decision 1 — Pool size (not pool convention)

The **pre-money pool refresh convention** is standard at every
institutional fund. Fighting the convention is not a winning
move; it marks the founder as un-oriented to the market and
burns political capital that would be better spent on the
number that's actually negotiable.

What *is* negotiable is the **size** of the pool. And the size
of the pool is a direct, one-for-one transfer of ownership from
founders to the pool.

The math (chapters 05 and 06):

- Pool size is expressed as a **percentage of post-close FD**.
- Every extra percentage point of pool sits inside the
  pre-money.
- Every extra percentage point inside the pre-money comes out
  of the pre-money holders — founders (and any converted SAFE
  holders), not the new investor.

Numerical illustration, holding everything else in the standard
scenario constant (2 founders, $500k SAFE at $5M cap, $2M at
$8M pre):

| Pool at post-close | Combined founders at close | Per-founder swing vs 10% |
|--------------------|----------------------------|--------------------------|
| 5%                 | ~67%                       | +2.5 pp per founder      |
| 10%                | ~62%                       | baseline                 |
| 15%                | ~58%                       | −2 pp per founder        |
| 20%                | ~54%                       | −4 pp per founder        |

<!-- needs-research: verify the swings above against a full cap-table walk with each pool percentage; the numbers are illustrative and calibrated against the walk in chapter 06. -->

Five percentage points of pool — the difference between a
counsel-typed 15% default and a hiring-plan-defended 10% —
is roughly **two percentage points per founder** at close. That
is not a rounding error; it is a real amount of the company that
the founder has the choice to fund or not to fund.

**The lever:** bring a **hiring plan with grants attached** to
the pool-size discussion. Ten percent is defensible when it
supports the eighteen-month hiring plan (mod-003) plus a modest
buffer. Fifteen percent is a gift to the next round's
investors when the hiring plan needs ten.

## Decision 2 — SAFE cap and stack size

Every SAFE the founder signs at a low cap sells a large
percentage of the company for a small dollar amount. The
post-money invariant makes the arithmetic legible:

```
each SAFE's ownership at conversion = SAFE amount / post-money cap
total SAFE stack ownership          = Σ (amount_i / cap_i)
```

Two SAFE-stack decisions dominate:

- **The cap on the current SAFE.** A $500k SAFE at a $2.5M cap is
  20% of the pre-new-money FD; the same $500k at a $10M cap is
  5%. **Cap dominates check size for founder dilution.**
- **The size of the total stack.** A single 10% SAFE is one
  problem; four SAFEs summing to 25% is a very different
  problem — and one that many founders don't compute because
  they think in terms of individual checks rather than the
  running total.

Illustration, holding the priced round constant at $2M/$8M pre
and pool constant at 10%:

| SAFE stack (pre-new-money) | Combined founders at close | Per-founder swing vs 10% |
|----------------------------|----------------------------|--------------------------|
| 0% (no SAFE)               | ~70%                       | +4 pp per founder        |
| 10% ($500k @ $5M)          | ~62%                       | baseline                 |
| 20% ($1M @ $5M)            | ~54%                       | −4 pp per founder        |
| 30% ($1.5M @ $5M)          | ~46%                       | −8 pp per founder        |

<!-- needs-research: verify the swings above against a full cap-table walk with each SAFE-stack size; the numbers are illustrative and calibrated against the walk in chapter 06. -->

The founder-important observation: **the SAFE cap is a decision
you're making today for a round you haven't priced yet.** The
priced-round investor will look at the SAFE stack when they
compute their own price. If the stack is 30%, the priced-round
lead will demand a lower pre-money to compensate — which
dilutes founders *more*, on top of the SAFEs.

**The lever:** every SAFE cap decision is a founder ownership
decision. Set caps that are defensible against a plausible
priced-round valuation 12–18 months out. Keep a running total
of the stack. Don't sign the fourth SAFE without checking
what the stack has become.

## Decision 3 — Round size and pre-money together

The single most common headline mistake is comparing rounds by
**pre-money valuation** in isolation. Pre-money by itself doesn't
determine dilution; the pair (round size, pre-money) does.

```
new-money dilution = round amount / post-money valuation
post-money         = pre-money + round amount
```

Illustration, holding pool at 10% and no SAFE:

| Round     | Pre-money | Post-money | New-money %  | Combined founders at close |
|-----------|-----------|------------|--------------|----------------------------|
| $2M       | $8M       | $10M       | 20.0%        | ~72%                       |
| $3M       | $8M       | $11M       | 27.3%        | ~65%                       |
| $2M       | $10M      | $12M       | 16.7%        | ~75%                       |
| $3M       | $10M      | $13M       | 23.1%        | ~69%                       |
| $3M       | $12M      | $15M       | 20.0%        | ~72%                       |

<!-- needs-research: verify the swings above against a full cap-table walk (no SAFE, 10% post-close pool); the numbers are illustrative. -->

Read the table across rows, not down columns:

- A **$3M at $12M pre** and a **$2M at $8M pre** produce **the
  same founder ownership at close** — the pre-money went up
  and so did the round.
- A **$3M at $8M pre** and a **$2M at $10M pre** — different
  headlines, materially different dilution. The **$8M pre**
  headline is $2M lower, but the $3M round takes 27% (vs 17%
  for the $10M pre / $2M round). Founders end up **10 pp
  lower** on the $3M/$8M version.

**The founder-important rule:** compare rounds by **post-money
founder ownership**, not by pre-money headline. The pre-money
number optimises for the marketing announcement; the founder
ownership number optimises for the founder's actual position.

There is a separate discipline about **round size** on the
mod-004 side — the round should be the amount that buys the
milestone plus a 6–9-month post-milestone buffer, no more and
no less. Any round size chosen for cap-table optics ("we should
raise more so we can announce a bigger round") is a round size
that will produce avoidable dilution. Mod-004 chapter 02 is the
reference.

## The three decisions, side by side

Combining the three levers in the standard scenario, here is
the combined founder ownership at close under a few
combinations. Each cell holds two founders combined; halve for
per-founder:

| Pool | Stack | Round      | Combined founders at close |
|------|-------|------------|----------------------------|
| 10%  | 10%   | $2M @ $8M  | 62%                        |
| 10%  | 20%   | $2M @ $8M  | 54%                        |
| 15%  | 10%   | $2M @ $8M  | 58%                        |
| 10%  | 10%   | $3M @ $12M | 62%                        |
| 15%  | 20%   | $3M @ $8M  | 44%                        |

<!-- needs-research: verify the swings above against full cap-table walks; the numbers are illustrative and calibrated against the walk in chapter 06. -->

The **worst-case row** — 15% pool + 20% SAFE stack + $3M at $8M
pre — puts the founders at **22% each** at close. The **standard
scenario** — 10% pool, 10% SAFE, $2M at $8M pre — puts them at
**31% each**. That is a **9-pp-per-founder swing** driven
entirely by the three structural decisions this chapter is
about. None of it is about the valuation headline.

## What the founder can and cannot negotiate

At the term sheet, the founder can negotiate **all three**:

- Pool size — with a hiring plan.
- Pre-money — with evidence and market comparables.
- Round size — with the mod-003 milestone math.

At the SAFE stage, the founder can negotiate:

- SAFE cap — with the priced-round-valuation story 12–18
  months out.
- SAFE form (post-money, of course) and any side letters.

At neither stage can the founder easily change:

- **The pre-money pool refresh convention.** Universal at
  institutional funds.
- **The 1× non-participating liquidation preference norm.**
  Universal at seed and Series A (chapter 08).
- **The broad-based weighted-average anti-dilution norm.**
  Universal at seed and Series A (chapter 08).

Founders who spend their negotiation credit on the universal
conventions have none left for the actual variables. Spend it
on the three levers in this chapter.

## Common wrong versions

- **Optimising for the pre-money number.** Founder pushes for a
  higher pre-money in isolation, accepts a larger round or a
  larger pool to get it, and ends up more diluted at close.
- **Signing SAFE-by-SAFE without a stack total.** Each SAFE
  looks small; the stack is 25%.
- **Accepting counsel's default 15% pool.** Every institutional
  fund's default template is somewhere in the 10–20% pool
  range; the specific default is arbitrary, and the founder
  has to bring the hiring-plan-based counter-number.
- **Comparing two term sheets on pre-money alone.** The correct
  comparison is founder ownership at close, computed from
  (pre-money, round size, pool) together.

## Summary

- Three structural decisions in the current round move founder
  ownership more than the pre-money headline:
  - **Pool size**, not pool convention. Bring a hiring plan.
  - **SAFE cap and stack size**. Cap dominates check size for
    founder dilution; a running stack total is a founder
    tool.
  - **Round size and pre-money together**. Compare rounds by
    post-money founder ownership, not by pre-money headline.
- Two more decisions (**liquidation preference** and
  **anti-dilution**) live on the term sheet but reach into the
  cap table at exit and in down rounds. Chapter 08.
- Universal conventions — pre-money pool refresh, 1×
  non-participating preference, broad-based weighted-average
  anti-dilution — are not the place to spend negotiation
  credit. Spend it on the three levers above.

**Next:** the two term-sheet clauses that reach into the cap
table — liquidation preference (1× non-participating default;
anything more aggressive is money out of the founders' pocket
at exit) and anti-dilution (broad-based weighted-average
default; full-ratchet is a punitive term worth pushing hard
to remove) — in
[chapter 08](./08-term-sheet-clauses-liq-pref-anti-dilution.md).
