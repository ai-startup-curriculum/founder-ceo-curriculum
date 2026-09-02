# Chapter 06 — The Walked Example: Founding → SAFE → Priced Seed

> **Reads with:** module objective 5 — *walk a company's cap
> table from founding through a priced seed — two founders + 10%
> option pool + $500k post-money SAFE at a $5M cap + $2M priced
> seed at an $8M pre-money — showing the dilution each instrument
> caused.*

## Why walk it once, share by share

Chapters 01–05 gave you the parts: what a cap table is, the four
share classes, the SAFE's cap-and-form anatomy, the post-money
invariant, and the pre-money pool refresh. This chapter is the
part where you put those parts together and produce a cap table
that sums to 100.0% at every snapshot.

The reason to walk this once share by share, instead of taking
the summary percentages on faith, is that it makes the
dilution attributable — you can point to each row and say *this
is where the founders lost X percentage points, and this is
why.* When the same shape appears at your Series A pool refresh
or your Series B down-round anti-dilution adjustment, you'll
recognise which cells moved and why. That recognition is the
skill; the arithmetic is just the drill that builds it.

## The scenario

Two co-founders start a company. Twelve months in, they raise a
small SAFE round. Six months after that, they close a priced
seed with an institutional lead.

- **Founding.** Two co-founders each hold **5,000,000 shares of
  common** (10,000,000 total FD, no pool reserved).
- **SAFE round.** A single **$500k post-money SAFE at a $5M
  post-money cap** is signed.
- **Priced seed.** **$2M raise at an $8M pre-money valuation**
  (⇒ $10M post-money). The lead requires a **10% post-close
  option pool**, refreshed pre-money (i.e., inside the $8M
  pre-money).

The walk has four snapshots: founding, after-SAFE-signed,
after-pool-refresh-and-SAFE-conversion (pre-new-money), and
post-close.

## Snapshot 0 — Founding

The simplest possible FD cap table:

```
| Stakeholder | Shares (issued) | Shares (FD) | FD %   |
| Founder A   | 5,000,000       | 5,000,000   | 50.0%  |
| Founder B   | 5,000,000       | 5,000,000   | 50.0%  |
| Option pool | 0               | 0           |  0.0%  |
| Total FD                                     100.0%   |
```

The pool row is on the table at zero — because it will appear at
the round and you want the row to already exist. Founder
ownership: **50% each**.

## Snapshot 1 — SAFE signed

The founders sign a **$500k post-money SAFE at a $5M cap**. On
the cap table itself, nothing changes — the SAFE is not a share.
Underneath the FD table, add a SAFE-stack section:

```
SAFE stack (off cap table until conversion)
  | Investor | Amount | Cap  | Form        | Fixed % at conversion |
  | SAFE #1  | $500k  | $5M  | post-money  | 10.0%                 |
```

The FD table is unchanged:

```
| Stakeholder | Shares (FD) | FD %   |
| Founder A   | 5,000,000   | 50.0%  |
| Founder B   | 5,000,000   | 50.0%  |
| Option pool | 0           |  0.0%  |
| Total FD                  100.0%   |
```

Founder ownership: **still 50% each on the FD table**. Off the
table, the company has now promised 10% at conversion — which
matters when a founder sits down to compute "what have we
already sold?" *before* the priced round starts.

## Snapshot 2 — Priced round: pool refresh + SAFE conversion (pre-new-money)

At the priced round, three things happen before the new-money
row is added:

- The **pool is refreshed to 10% of post-close FD**, sitting
  **inside the pre-money** (per the pre-money refresh
  convention — chapter 05).
- The **SAFE converts** at its fixed 10% of the pre-new-money FD
  (per the post-money invariant — chapter 04).
- The founders' 10,000,000 shares don't change.

This is a small system of equations. Let `T` be the post-close FD
share count. The constraints:

```
new-money shares / T                = 20.0%   (round is $2M/$10M post)
pool shares / T                     = 10.0%   (10% post-close pool)
SAFE shares / (T × 0.80)            = 10.0%   (SAFE invariant on pre-new-money FD)
founder shares                      = 10,000,000
founder shares + pool shares + SAFE shares = pre-new-money FD = T × 0.80
```

Solve. Substituting `SAFE shares = 0.10 × T × 0.80 = 0.08 × T`
and `pool shares = 0.10 × T`:

```
10,000,000 + 0.10 × T + 0.08 × T = 0.80 × T
10,000,000 = 0.62 × T
T ≈ 16,129,032 shares
```

Round `T` up to the nearest integer share; the resulting FD % may
round to a tenth of a percent from a fraction that isn't exactly
whole. That's fine — this is a walked example, not a real cap-
table software run.

From there:

- `pool shares    = 0.10 × T ≈ 1,612,903`
- `SAFE shares    = 0.08 × T ≈ 1,290,323`
- `pre-new-money FD = 0.80 × T ≈ 12,903,226`

Fill in Snapshot 2 (pre-new-money FD, **before** the new money is
added):

```
| Stakeholder | Shares (FD) | FD % (of pre-new-money) |
| Founder A   | 5,000,000   | 38.75%                  |
| Founder B   | 5,000,000   | 38.75%                  |
| SAFE holder | 1,290,323   | 10.00%                  |
| Option pool | 1,612,903   | 12.50%                  |
| Total FD    | 12,903,226  | 100.00%                 |
```

Sanity check: the founders now own 77.5% of the pre-new-money
FD (down from 100.0% of the previous FD count). The SAFE
holder appears for the first time at 10.0% (its fixed invariant
share). The pool appears at 12.5% of pre-new-money — a bigger
percentage than the 10% post-close target because it sits inside
the smaller pre-money slice.

## Snapshot 3 — New-money preferred issued

Now the new money. Price per share falls out of the pre-money
valuation and the pre-new-money FD share count:

```
price per share = pre-money valuation / pre-new-money FD share count
                = $8,000,000 / 12,903,226
                ≈ $0.6200 / share

new-money shares = round amount / price per share
                 = $2,000,000 / $0.6200
                 ≈ 3,225,806
```

Total post-close FD:

```
post-close FD = pre-new-money FD + new-money shares
              = 12,903,226 + 3,225,806
              = 16,129,032
```

That matches the `T` we solved for. Recompute every FD %
using `owner FD shares / post-close FD`:

```
| Stakeholder    | Shares (FD)  | FD %    |
| Founder A      | 5,000,000    | 31.00%  |
| Founder B      | 5,000,000    | 31.00%  |
| SAFE holder    | 1,290,323    |  8.00%  |
| Option pool    | 1,612,903    | 10.00%  |
| Series Seed    | 3,225,806    | 20.00%  |
| Total FD       | 16,129,032   | 100.00% |
```

The founders end up at **31% each** — a combined **62%** of the
post-close cap table.

## Founder ownership curve

Pulling the founders' combined ownership across the four
snapshots:

| Snapshot                                         | Combined founders |
|--------------------------------------------------|-------------------|
| 0 — Founding                                     | 100.0%            |
| 1 — SAFE signed (SAFE off FD)                    | 100.0%            |
| 2 — Pool refresh + SAFE conversion (pre-new-money) |  77.5%          |
| 3 — Post-close                                   |  62.0%            |

That curve is the round. **The pool refresh + SAFE conversion took
22.5 percentage points; the new-money issuance took another
15.5 percentage points** (`77.5% × 20.0%`). Founders lost more
combined ownership *before* the new-money row was issued than
they lost to the new money itself — which is the whole point of
this chapter and the reason chapters 05 and 07 exist.

## Where the dilution went — per-step attribution

For each transition, name **who was diluted**, **by how many
percentage points**, and **why**:

- **0 → 1 (SAFE signed).** No FD dilution yet — the SAFE is a
  claim on the next round, not an issued share. Founder ownership
  unchanged at 50%/50%. Off-cap-table: the company has now
  promised 10% at conversion.
- **1 → 2 (pool refresh + SAFE conversion).** Founder A dropped
  from 50.00% to **38.75%** (−11.25 pp). Founder B dropped from
  50.00% to **38.75%** (−11.25 pp). The pool appears at
  **12.50%** of pre-new-money FD; the SAFE appears for the first
  time at **10.00%**. Because the pool was refreshed pre-money,
  the pool shares came out of the pre-money holders' stake —
  the incoming Series Seed investor is not diluted by their own
  required pool.
- **2 → 3 (new money issued).** Every pre-new-money holder is
  diluted by exactly **20%** of their pre-round position (the
  round is 20% post-money). Founder A drops from 38.75% to
  **31.00%** (−7.75 pp). Founder B similarly. The SAFE holder
  drops from 10.00% to **8.00%** (−2.00 pp). The pool drops from
  12.50% to **10.00%** (−2.50 pp).

Combined founder loss across the round: **50.0% × 2 = 100.0%**
combined at founding → **62.0%** combined at close. **38 pp of
combined founder dilution**, distributed:

- ~20 pp to the new-money investor (the round itself).
- ~10 pp to the option pool (the refresh, funded pre-money by
  the founders).
- ~8 pp to the SAFE holder (the SAFE conversion, funded
  pre-money by the founders).

That attribution is the founder-important number, and it will
reappear every time you walk a real round.

## Sanity checks

At every snapshot, run the invariants:

- **Sum of FD % = 100.0%.** If it doesn't, someone is
  miscounted; go back and find them.
- **Founder shares × two = 10,000,000, unchanged throughout.**
  Founders' *share count* doesn't move; only the denominator
  changes.
- **SAFE holder's percentage of pre-new-money FD = amount / cap
  = 10.0%.** If it isn't, the SAFE conversion is wrong.
- **New-money percentage of post-close FD = round /
  post-money = 20.0%.** If it isn't, the price per share is
  wrong.
- **`Founder A + Founder B = 62.0% of post-close`** if the pool
  refresh and the SAFE conversion followed the standard scenario.

## What changes if you push one lever

To sharpen intuition, hold everything else constant and change
one input:

- **Pool at 15% instead of 10%.** Founders end up at roughly
  **29% each** instead of 31% — a **~2 pp per-founder swing**
  from the same round.
- **SAFE cap at $2.5M instead of $5M.** SAFE fixed ownership is
  now 20% (not 10%) of pre-new-money FD. Founders end up at
  roughly **23% each** — a **~8 pp per-founder swing** for the
  same $500k in.
- **$3M round at $7M pre-money instead of $2M at $8M pre.**
  New money is 30% (not 20%). Founders end up at roughly
  **26% each** — a **~5 pp per-founder swing**, in exchange for
  $1M more cash.

Which of those swings you can control depends on the round;
chapter 07 gets specific about which structural decisions are
the ones actually still moving in this round.

## Common wrong versions

- **Founders shown on the table but pool ignored.** The founders
  look like they own more than they do because the pool row is
  missing. Common at incorporation-era cap tables that were
  never updated.
- **SAFE double-counted as both a stack row and an FD row
  pre-round.** The SAFE is either on the stack (pre-round) or
  in the FD table (post-conversion), never both.
- **Pool refresh applied post-money by mistake.** The founder
  computes a 10% post-money pool as if it dilutes the new
  investor too. It doesn't — the convention is pre-money, and
  the pool comes out of existing holders only.
- **Percentages of percentages.** Founder rounds each row to
  one decimal, then computes the total from the rounded
  percentages, and gets 99.9% or 100.1%. Always compute
  percentages from raw share counts.

## Summary

- The walked scenario — two founders, $500k SAFE at $5M cap,
  10% pool, $2M at $8M pre — produces a **62%** combined
  founder ownership at close (**31% each**).
- **~20 pp of dilution went to the new-money investor**, **~10
  pp to the option pool**, and **~8 pp to the SAFE holder** —
  the pool refresh and the SAFE conversion together diluted
  the founders **more than the round itself did.**
- Run the invariants at every snapshot: FD % sums to 100.0%,
  founder share count unchanged, SAFE at `amount / cap` of
  pre-new-money FD, new money at `round / post-money` of
  post-close FD.
- Attribution matters. "We got diluted by the round" hides
  three separate dilution events that each responded to a
  different founder decision.

**Next:** the three structural decisions in this round that
most affect founder ownership at the *next* round — pool size
(not convention), SAFE cap and stack size, round size and
pre-money together — in
[chapter 07](./07-three-structural-decisions.md).
