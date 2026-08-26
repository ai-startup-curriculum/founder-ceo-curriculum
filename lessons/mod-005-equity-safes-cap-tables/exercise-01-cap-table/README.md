# Exercise 01 — Cap Table: Founders + Pool + SAFE + Priced Seed

**Module:** 005 Equity, SAFEs & Cap Tables · **Stage:** PRE-SEED→SEED ·
**Time:** ~1 week (≈6–8 focused hours)

## Deliverables (two founder artifacts, plus one call)

1. **A four-step cap table** (spreadsheet or table) showing FD share counts
   and ownership % at each of: founding, after the SAFE is signed, after the
   pool refresh + SAFE conversion at the priced round, and after the new
   priced-round money is issued. FD % sums to 100.0% at every step.
2. **A one-paragraph "where the dilution went" narrative** — one sentence per
   step naming who was diluted, by how many percentage points, and why (pool
   refresh, SAFE conversion, new-money issuance).
3. **A one-paragraph "riskiest structural call" note** — the single
   structural decision in this round (pool size, SAFE cap, round size vs.
   pre-money) that most changes founder ownership, plus the change you would
   push for in a real negotiation and the counter you expect from the lead.

## Scenario

Pick one:

- **Your real startup** (recommended if you're an operating founder): use
  your **actual** founders' split, every SAFE you've already signed (cap,
  amount, pre- or post-money form), and the priced round you're planning to
  raise next (from your mod-004 funnel).
- **Simulated:** Two co-founders each hold **5,000,000 shares of common** at
  founding (10,000,000 total FD, no pool yet). A single **$500k post-money
  SAFE at a $5M post-money cap** is signed at pre-seed. The priced seed is a
  **$2M raise at an $8M pre-money valuation** ($10M post-money), and the
  lead requires a **10% post-close option pool** (refreshed pre-money —
  meaning the pool sits inside the $8M pre-money and dilutes existing
  holders).

## Steps

1. **State the founding cap table.** Table with columns: stakeholder, shares
   (issued), shares (FD), FD %. Sum FD % to 100.0%. If it doesn't sum, fix
   the sheet before you go further. This is the invariant you'll re-check
   after every step.
2. **Add the option pool row at 0%.** Even if you didn't reserve a pool at
   incorporation, add the row now with 0 shares reserved so it's on the
   table when the refresh lands. Every seed-stage cap table has a pool row;
   better to see it as a zero than to add it under time pressure at the
   round.
3. **Sign the SAFE.** A post-money SAFE at a $5M cap for $500k is
   contractually 10% of the company at conversion (`$500k / $5M`). Do **not**
   add the SAFE to the FD share count yet — SAFEs are on the stack until the
   priced round. Add a "SAFE stack" section beneath the FD table with the
   SAFE's amount, cap, form (post-money), any MFN or pro-rata side letters,
   and the fixed ownership it will convert to.
4. **Set up the pool refresh at the priced round.** The lead's ask is a 10%
   post-close pool. Because the pool is refreshed pre-money, the pool takes
   its shares out of the *pre-money* holders (founders + converting SAFE).
   Compute the pool share count so that `pool shares / post-close FD =
   10.0%`. Write down which cells changed and by how many percentage points.
5. **Convert the SAFE.** At conversion, the SAFE holder gets shares equal to
   10% of the pre-new-money, post-pool-refresh FD (the post-money SAFE
   invariant). Add those shares to the FD table. Sum FD % across the
   pre-new-money holders — it should equal 100.0% at this snapshot (the
   new-money shares are added in the next step).
6. **Issue the new-money preferred.** The $2M / $8M-pre round is 20% of the
   $10M post-money. Compute:
   - `price per share = pre-money / pre-money FD share count`
   - `new-money shares = $2M / price per share`
   Add the new-money row to the FD table. Recompute every FD %. The
   pre-money holders (founders, SAFE, pool) should each be at
   `pre-round % × (1 − 20%)`.
7. **Read off the final ownership.** Founder A, Founder B, SAFE holder,
   option pool (reserved), Series Seed. Sum to 100.0%. Compare founder
   ownership at each of the four steps — that curve is the story of the
   round.
8. **Write the dilution narrative and the riskiest-structural-call note.**
   For each step, one sentence: who was diluted, by how many percentage
   points, why. Then: which one structural decision (pool size, SAFE cap,
   round size vs. pre-money) is most responsible for the founder ownership
   number? What change would you push for in a real negotiation, and what
   pushback do you expect?

## Cap-table template (fill inline)

```
Step 0 — Founding
  | Stakeholder      | Shares (issued) | Shares (FD) | FD %  |
  | Founder A        | 5,000,000       | 5,000,000   | 50.0% |
  | Founder B        | 5,000,000       | 5,000,000   | 50.0% |
  | Option pool      | 0               | 0           |  0.0% |
  | Total FD                                          100.0% |

SAFE stack (off cap table until conversion):
  | Investor | Amount | Cap    | Form        | Fixed ownership at conversion |
  | SAFE #1  | $500k  | $5M    | post-money  | 10.0%                          |

Step 1 — SAFE signed (SAFE still off FD)
  | Stakeholder | Shares (FD) | FD %  |
  | Founder A   | 5,000,000   | 50.0% |
  | Founder B   | 5,000,000   | 50.0% |
  | Option pool | 0           |  0.0% |
  | Total FD                    100.0% |
  Note: SAFE is a 10% claim at conversion; not on the FD until the priced round.

Step 2 — Priced round: pool refresh + SAFE conversion (pre-new-money)
  Target: pool = 10.0% of post-close FD (post-close includes the $2M new money).
  Solve for pool_shares, SAFE_shares, and total pre-new-money FD such that:
    pool_shares       / post-close FD = 10.0%
    SAFE_shares       / (post-close FD × 0.8) = 10.0%   (post-money SAFE invariant)
    founder_shares    unchanged at 10,000,000
    post-close FD     = pre-new-money FD / 0.8          (new money = 20%)

  Fill in:
    pre-new-money FD share count:   ___
    pool shares (reserved):         ___
    SAFE shares (converted):        ___
    post-close FD share count:      ___

  | Stakeholder | Shares (FD) | FD % (of pre-new-money) |
  | Founder A   | 5,000,000   | ___                     |
  | Founder B   | 5,000,000   | ___                     |
  | SAFE holder | ___         | 10.0%                   |
  | Option pool | ___         | ___                     |
  | Total FD                    100.0%                  |

Step 3 — New-money issued ($2M @ $8M pre)
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
  Step 0: 100.0%   Step 1: 100.0%   Step 2: ___%   Step 3: ___%
```

## Dilution narrative template (fill inline)

```
Step 0 → 1 (SAFE signed): No FD dilution yet — the SAFE is a claim on the
next round, not an issued share. Founder ownership unchanged at 50% / 50%.
Off-cap-table: the company has now promised 10% at conversion.

Step 1 → 2 (pool refresh + SAFE conversion): Founder A dropped from 50.0%
to ___% (___ pp). Founder B dropped from 50.0% to ___% (___ pp). The pool
appears at ___% of the pre-new-money FD; the SAFE holder appears for the
first time at 10.0% (fixed by the post-money cap). Because the pool was
refreshed pre-money, the pool shares came out of the pre-money holders'
stake — the incoming Series Seed investor is not diluted by their own
required pool.

Step 2 → 3 (new money issued): Every existing holder is diluted by exactly
20.0% of their pre-round position (the round is 20% post-money). Final
ownership: Founder A ___%, Founder B ___%, SAFE holder ___%, pool 10.0%,
Series Seed 20.0%.
```

## Riskiest-structural-call template (fill inline)

```
The single structural decision that most changed founder ownership in this
round:
  ___  (pool size / SAFE cap / round size vs. pre-money — pick one)

Reasoning, with the pp math:
  If ___ had been ___ instead of ___, founder ownership at close would have
  been ___% instead of ___% — a swing of ___ pp.

The change I would push for in a real negotiation:
  ___

The pushback I expect from a lead investor:
  ___

The counter I would offer:
  ___
```

## Rubric (self-assess, then compare to the exemplar)

<!-- needs-research: exemplar for mod-005 not yet authored; rubric-vs-exemplar comparison assumes future exemplars/mod-005-equity-safes-cap-tables/. -->

| Dimension | Weak | Strong |
|---|---|---|
| FD accounting | Issued shares only; pool ignored | FD share count includes the reserved pool and the converted SAFE; sums to 100.0% at every step |
| Pool convention | Pool assumed to dilute the incoming investor | Pool is refreshed pre-money and dilutes existing holders; the pp math is shown |
| SAFE handling | SAFE ignored until priced round or double-counted | Post-money SAFE = amount/cap fixed ownership pre-new-money; converted at the correct share count |
| Priced-round math | "20% dilution" hand-waved | Price per share computed from pre-money and pre-new-money FD count; new-money shares issued explicitly |
| Dilution attribution | "We got diluted by the round" | Every step names who was diluted, by how many percentage points, and why |
| Structural call | "The valuation was too low" | One named structural lever (pool size / cap / round vs. pre-money) with the pp impact quantified |
| Live-lab realism | Simulated numbers only | Real cap table walked; own SAFEs listed with actual caps and forms |

## Definition of done

A skeptical co-founder or an early-stage venture lawyer would read your cap
table and narrative and agree that (a) the FD share counts and percentages
are correct at every step, (b) the SAFE conversion and pool refresh followed
market convention, and (c) the structural call you named would move founder
ownership in the direction — and by roughly the magnitude — you claim.
