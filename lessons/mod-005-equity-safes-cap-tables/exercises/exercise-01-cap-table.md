# Exercise 01 — Cap Table: Founders + Pool + SAFE + Priced Seed

**Module:** 005 Equity, SAFEs & Cap Tables · **Stage:**
PRE-SEED→SEED · **Time:** ~1 week (≈6–8 focused hours) ·
**Reads with:** chapters
[01](../01-cap-table-fundamentals.md),
[02](../02-four-share-classes.md),
[04](../04-post-money-safe-conversion-math.md),
[05](../05-option-pool-sizing-and-who-pays.md), and
[06](../06-cap-table-walk-founding-to-priced-seed.md).

## Problem statement

You have (or will have) a company with two co-founders, a small
SAFE round on the stack, and a plausible priced seed on the
horizon. You do **not** yet have a defensible answer to the
questions a lead investor's counsel — or your own counsel —
asks in the first ten minutes of the round: *"can I see the
FD cap table walked through the round?"* and *"how much of the
company does each founder end up with at close?"*

This exercise produces both answers. You walk the cap table
share-by-share from founding through a priced seed, produce a
snapshot table that sums to 100.0% at each step, attribute the
dilution at each transition, and name the single structural
decision most responsible for the founder-ownership number.

## Deliverables (three founder artifacts)

1. **A four-step cap table** (spreadsheet or table) showing FD
   share counts and ownership % at each of: founding, after the
   SAFE is signed, after the pool refresh + SAFE conversion at
   the priced round (pre-new-money), and after the new-money
   preferred is issued (post-close). FD % sums to 100.0% at
   every step.
2. **A one-paragraph "where the dilution went" narrative** —
   one sentence per transition naming who was diluted, by how
   many percentage points, and why (pool refresh, SAFE
   conversion, new-money issuance). Include the founder-
   ownership curve (combined founders' % across the four
   snapshots).
3. **A one-paragraph "riskiest structural call" note** — the
   single structural decision in this round (pool size, SAFE
   cap, round size vs pre-money) that most changed founder
   ownership, plus the change you would push for in a real
   negotiation and the counter you expect from the lead.

## Scenario

Pick one:

- **Your real startup** (recommended if you're an operating
  founder): use your **actual** founders' split, every SAFE
  you've already signed (cap, amount, pre- or post-money form,
  any side letters), and the priced round you're planning to
  raise next (from your mod-004 funnel).
- **Simulated:** Two co-founders each hold **5,000,000 shares
  of common** at founding (10,000,000 total FD, no pool yet).
  A single **$500k post-money SAFE at a $5M post-money cap**
  is signed at pre-seed. The priced seed is a **$2M raise at
  an $8M pre-money valuation** ($10M post-money), and the lead
  requires a **10% post-close option pool** (refreshed
  pre-money — meaning the pool sits inside the $8M pre-money
  and dilutes existing holders).

Chapter [06](../06-cap-table-walk-founding-to-priced-seed.md)
walks the simulated scenario step-by-step; the exercise
requires you to *reproduce* that walk yourself, not to copy
the answer.

## Requirements

Each requirement is checkable by inspecting your submission:

- **Founding snapshot.** Table with columns: stakeholder,
  shares (issued), shares (FD), FD %. Sum FD % to 100.0%. Pool
  row present at 0 shares.
- **SAFE-signed snapshot.** FD table unchanged (SAFE off FD).
  SAFE-stack section beneath the FD table with each SAFE's
  amount, cap, form (post-money), any MFN or pro-rata side
  letters, and the fixed ownership it will convert to
  (`amount / post-money cap`).
- **Pre-new-money snapshot (pool refresh + SAFE conversion).**
  Show the solved system: pre-new-money FD share count, pool
  shares, SAFE shares, founders' shares. FD % sums to
  100.0%. Pool is 10.0% of post-close FD (not pre-new-money);
  SAFE is 10.0% of pre-new-money FD (invariant).
- **Post-close snapshot.** Add the new-money row. Show
  `price per share = pre-money / pre-new-money FD share count`
  and `new-money shares = round amount / price per share`. FD
  % sums to 100.0%. Founder ownership at close falls out of
  the arithmetic.
- **Dilution attribution.** For each transition, name who was
  diluted, by how many pp, and why. Combined-founder-
  ownership curve across the four snapshots.
- **Riskiest structural call.** One of pool size, SAFE cap,
  round size vs pre-money — named, with the pp math showing
  the swing, and a specific ask for the negotiation.

## Cap-table template (fill inline)

```
Snapshot 0 — Founding
  | Stakeholder      | Shares (issued) | Shares (FD) | FD %  |
  | Founder A        | 5,000,000       | 5,000,000   | 50.0% |
  | Founder B        | 5,000,000       | 5,000,000   | 50.0% |
  | Option pool      | 0               | 0           |  0.0% |
  | Total FD                                          100.0% |

SAFE stack (off cap table until conversion):
  | Investor | Amount | Cap   | Form        | Fixed % at conversion |
  | SAFE #1  | $500k  | $5M   | post-money  | 10.0%                 |

Snapshot 1 — SAFE signed (SAFE still off FD)
  | Stakeholder | Shares (FD) | FD %  |
  | Founder A   | 5,000,000   | 50.0% |
  | Founder B   | 5,000,000   | 50.0% |
  | Option pool | 0           |  0.0% |
  | Total FD                    100.0% |
  Note: SAFE is a 10% claim at conversion; not on the FD until the priced round.

Snapshot 2 — Priced round: pool refresh + SAFE conversion (pre-new-money)
  Solve for post-close FD (T), pool shares, SAFE shares, pre-new-money FD:
    new-money shares / T                = 20.0%   (round is $2M/$10M post)
    pool shares / T                     = 10.0%
    SAFE shares / (T × 0.80)            = 10.0%   (SAFE invariant)
    founder shares                      = 10,000,000
    founder + pool + SAFE               = T × 0.80

  Fill in:
    pre-new-money FD share count:   ___
    pool shares (reserved):         ___
    SAFE shares (converted):        ___
    post-close FD share count (T):  ___

  | Stakeholder | Shares (FD) | FD % (of pre-new-money) |
  | Founder A   | 5,000,000   | ___                     |
  | Founder B   | 5,000,000   | ___                     |
  | SAFE holder | ___         | 10.0%                   |
  | Option pool | ___         | ___                     |
  | Total FD                    100.0%                  |

Snapshot 3 — New-money preferred issued ($2M @ $8M pre)
  price per share = $8,000,000 / pre-new-money FD share count = $___
  new-money shares = $2,000,000 / price per share             = ___

  | Stakeholder | Shares (FD) | FD %  |
  | Founder A   | 5,000,000   | ___   |
  | Founder B   | 5,000,000   | ___   |
  | SAFE holder | ___         | ___   |
  | Option pool | ___         | 10.0% |
  | Series Seed | ___         | 20.0% |
  | Total FD                    100.0%|

Founder ownership curve (both combined):
  Snapshot 0: 100.0%   Snapshot 1: 100.0%   Snapshot 2: ___%   Snapshot 3: ___%
```

## Dilution narrative template (fill inline)

```
Snapshot 0 → 1 (SAFE signed): No FD dilution yet — the SAFE is a
claim on the next round, not an issued share. Founder ownership
unchanged at 50% / 50%. Off-cap-table: the company has now
promised 10% at conversion.

Snapshot 1 → 2 (pool refresh + SAFE conversion): Founder A dropped
from 50.0% to ___% (___ pp). Founder B dropped from 50.0% to
___% (___ pp). The pool appears at ___% of the pre-new-money FD;
the SAFE holder appears for the first time at 10.0% (fixed by the
post-money cap). Because the pool was refreshed pre-money, the
pool shares came out of the pre-money holders' stake — the
incoming Series Seed investor is not diluted by their own
required pool.

Snapshot 2 → 3 (new money issued): Every pre-new-money holder is
diluted by exactly 20.0% of their pre-round position (the round
is 20% post-money). Final ownership: Founder A ___%, Founder B
___%, SAFE holder ___%, pool 10.0%, Series Seed 20.0%.
```

## Riskiest-structural-call template (fill inline)

```
The single structural decision that most changed founder
ownership in this round:
  ___  (pool size / SAFE cap / round size vs. pre-money — pick one)

Reasoning, with the pp math:
  If ___ had been ___ instead of ___, founder ownership at close
  would have been ___% instead of ___% — a swing of ___ pp per
  founder.

The change I would push for in a real negotiation:
  ___

The pushback I expect from a lead investor:
  ___

The counter I would offer:
  ___
```

## Acceptance criteria

You are done when *all* of the following are true:

- [ ] FD % sums to **100.0%** at every snapshot.
- [ ] Pool row is present at Snapshot 0 (even at zero shares).
- [ ] SAFE-stack section shows amount, cap, form, and fixed % at
      conversion for every SAFE.
- [ ] Snapshot 2 (pre-new-money) shows the solved share counts
      for pool, SAFE, and founders, with the pre-new-money FD
      total.
- [ ] Snapshot 3 shows price per share, new-money share count,
      and every row recomputed against post-close FD.
- [ ] Founder-ownership curve across the four snapshots is
      recorded.
- [ ] Dilution narrative names who lost how many pp at each
      transition.
- [ ] Riskiest-structural-call note picks one of pool size,
      SAFE cap, round size vs pre-money, and shows the pp swing
      that decision produced.

## Self-assessment rubric

<!-- needs-research: exemplar for mod-005 not yet authored; the rubric-vs-exemplar comparison assumes future exemplars/mod-005-equity-safes-cap-tables/. -->

| Dimension | Weak | Strong |
|---|---|---|
| FD accounting | Issued shares only; pool ignored | FD share count includes the reserved pool and the converted SAFE; sums to 100.0% at every step |
| Pool convention | Pool assumed to dilute the incoming investor | Pool is refreshed pre-money and dilutes existing holders; the pp math is shown |
| SAFE handling | SAFE ignored until priced round or double-counted | Post-money SAFE = amount/cap fixed ownership pre-new-money; converted at the correct share count |
| Priced-round math | "20% dilution" hand-waved | Price per share computed from pre-money and pre-new-money FD count; new-money shares issued explicitly |
| Dilution attribution | "We got diluted by the round" | Every transition names who was diluted, by how many percentage points, and why |
| Structural call | "The valuation was too low" | One named structural lever (pool size / cap / round vs. pre-money) with the pp impact quantified |
| Live-lab realism | Simulated numbers only | Real cap table walked; own SAFEs listed with actual caps and forms |

## Definition of done

A skeptical co-founder or an early-stage venture lawyer would
read your cap table and narrative and agree that (a) the FD
share counts and percentages are correct at every step, (b)
the SAFE conversion and pool refresh followed market
convention, and (c) the structural call you named would move
founder ownership in the direction — and by roughly the
magnitude — you claim.

> Solutions are not provided in this repository; they live in
> the paired solutions repo.
