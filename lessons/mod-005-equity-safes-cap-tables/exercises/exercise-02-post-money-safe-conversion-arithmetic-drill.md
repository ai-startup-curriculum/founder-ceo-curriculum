# Exercise 02 — Post-Money SAFE Conversion Arithmetic Drill

**Module:** 005 Equity, SAFEs & Cap Tables · **Stage:**
PRE-SEED→SEED · **Time:** ~2 focused hours · **Reads with:**
chapters
[03](../03-safe-anatomy.md) and
[04](../04-post-money-safe-conversion-math.md).

## Problem statement

The post-money SAFE invariant — `SAFE amount / post-money cap =
ownership %` — is one of the shortest and most consequential
formulas in early-stage cap-table math. The problem is that
"knowing the formula" and "being able to compute the right
answer in ten seconds when a lead partner asks how much your
SAFE stack is worth" are different skills.

This exercise is a **drill**: eight small scenarios that walk
you through the invariant on single SAFEs, then stacks, then
stacks with a priced-round dilution on top, then discount /
cap interaction, then MFN swaps at conversion, then a mixed
pre-money / post-money stack (the case where the invariant
does *not* apply). No narrative, no artifacts beyond the
arithmetic — just the reps until the answers come out fast.

## Deliverables (one filled-in drill sheet)

A single **drill sheet** (spreadsheet or Markdown table) with
the correct answer to each of the eight scenarios, plus a
one-sentence note under each scenario stating which formula
or invariant you applied.

## Requirements

Answer each of the following. Show the arithmetic
(intermediate share counts or percentages), not just the
final answer.

### Scenario 1 — Single SAFE, invariant

A $500k SAFE at a $5M post-money cap. Priced round comes in
at a $20M pre-money / $22M post-money. What percentage of the
pre-new-money FD does the SAFE holder own at conversion?

### Scenario 2 — Cap doesn't bind

A $500k SAFE at a **$10M** post-money cap (no discount). Priced
round comes in at a **$4M** pre-money / **$6M** post-money.
Cap-vs-round comparison: which price does the SAFE convert at
— the cap, or the round?

### Scenario 3 — Cap binds; effective price

A $250k SAFE at a **$2.5M** post-money cap. Priced round comes
in at a **$12M** pre-money. What effective price per share does
the SAFE convert at, expressed as a fraction of the round's
own price per share? (I.e., how many times more shares per
dollar does the SAFE holder get compared to a Series Seed
investor at $12M pre?)

### Scenario 4 — Stack sums

Four post-money SAFEs are on the stack:

| Investor | Amount | Cap    |
|----------|--------|--------|
| SAFE #1  | $250k  | $5M    |
| SAFE #2  | $250k  | $5M    |
| SAFE #3  | $500k  | $5M    |
| SAFE #4  | $200k  | $4M    |

What is the total percentage of the pre-new-money FD that the
SAFE stack claims at conversion?

### Scenario 5 — Stack plus priced round

Take the stack from Scenario 4. Priced round comes in at
**$3M raise at $12M pre-money** ($15M post-money). What is
each SAFE holder's percentage of the **post-close** FD? Show
the stackable form (`s × (1 − r)`) for each SAFE.

### Scenario 6 — Discount interaction

A $500k SAFE at a **$10M** post-money cap **with a 20%
discount**. Priced round at **$6M pre-money / $7M post-money**.
Which term wins — cap or discount — and what percentage of the
pre-new-money FD does the SAFE holder own at conversion?

### Scenario 7 — MFN swap at conversion

At month 0, the company issues a **$100k SAFE at a $8M
post-money cap with an MFN clause** to an angel. Six months
later, the company issues a **$500k SAFE at a $4M post-money
cap** to a pre-seed fund. At the priced round eighteen months
after that, the angel elects MFN. What is the angel's
percentage of the pre-new-money FD at conversion after the
MFN swap? (Compare to what the angel's percentage would have
been *without* electing MFN.)

### Scenario 8 — Mixed pre-money / post-money stack

The company has a **$300k pre-money SAFE at a $4M pre-money
cap** (signed in 2016, before the post-money form existed)
and a **$500k post-money SAFE at a $5M post-money cap**
(signed in 2021). At conversion at a priced round, the
post-money SAFE's ownership is deterministic. **Why is the
pre-money SAFE's ownership not?** Answer in one sentence.
(You do not need to compute the pre-money SAFE's exact
ownership — the point is to recognise that the invariant
does not apply.)

## Starter guidance

**Session 1 (~30 min) — the pure invariant.** Do scenarios
1–4. Every answer is either a single `amount / cap` fraction
or a sum of them. If you find yourself opening a spreadsheet,
back off; these are envelope answers.

**Session 2 (~45 min) — priced-round dilution.** Do scenarios
5 and 6. Scenario 5 uses the stackable form
`final = pre × (1 − r)` for every holder; scenario 6 requires
computing effective prices from both cap and discount and
picking the one that gives the SAFE holder more shares.

**Session 3 (~45 min) — the special cases.** Scenarios 7 and 8
are the ones founders regularly miss. Scenario 7 is arithmetic
(the MFN swap changes the cap, which changes the invariant
answer). Scenario 8 is a recognition exercise — the pre-money
SAFE mixes with post-money SAFEs in a non-linear way, which is
the whole reason the 2018 revision was written.

## Templates (fill inline)

```
Scenario 1
  SAFE: $500k @ $5M post-money cap
  Priced round: $20M pre / $22M post
  Invariant: ownership at conversion = ______________
  SAFE % of pre-new-money FD: __________%

Scenario 2
  SAFE: $500k @ $10M post-money cap (no discount)
  Priced round: $4M pre / $6M post
  Cap-vs-round comparison:
    Cap price: __________
    Round price: __________
    SAFE converts at: __________ (cap / round)
  SAFE % of pre-new-money FD: __________%

Scenario 3
  SAFE: $250k @ $2.5M post-money cap
  Priced round: $12M pre
  Cap effective price per share: __________
  Round price per share (assuming 12M pre and a nominal FD count):
    (round price is relative; use ratio)
  Shares-per-dollar multiplier vs Series Seed: __________×

Scenario 4
  SAFE #1: $250k @ $5M → ______%
  SAFE #2: $250k @ $5M → ______%
  SAFE #3: $500k @ $5M → ______%
  SAFE #4: $200k @ $4M → ______%
  Total stack %: __________%

Scenario 5
  Take Scenario 4 stack. Round: $3M @ $12M pre.
  New-money % of post-close FD (r): __________%
  For each SAFE, final % = pre × (1 − r):
    SAFE #1: ______% → ______%
    SAFE #2: ______% → ______%
    SAFE #3: ______% → ______%
    SAFE #4: ______% → ______%
  Sum of SAFE stack at close: __________%
  (Cross-check: total pre-new-money × (1 − r) = stack close %)

Scenario 6
  SAFE: $500k @ $10M post-money cap + 20% discount
  Priced round: $6M pre / $7M post
  Cap effective price: __________
  Discounted round price: __________ (round price × 0.80)
  Winner: __________ (cap / discount)
  SAFE % of pre-new-money FD: __________%

Scenario 7
  Angel SAFE (original terms): $100k @ $8M post-money cap
  Angel SAFE without MFN election: __________%
  Later SAFE (post-money): $500k @ $4M
  If angel elects MFN, angel SAFE is now: $100k @ $4M cap
  Angel SAFE with MFN election: __________%
  Change: __________ pp
  Who funds the change? __________ (founders / other SAFE holders / new money)

Scenario 8
  Pre-money SAFE: $300k @ $4M pre-money cap (2016 form)
  Post-money SAFE: $500k @ $5M post-money cap (2018+ form)
  Post-money SAFE % at conversion (invariant): __________%
  Why the pre-money SAFE % is NOT determined by amount/cap:
    __________________________________________________________________
    __________________________________________________________________
```

## Acceptance criteria

You are done when *all* of the following are true:

- [ ] Every scenario has a numerical answer with the arithmetic
      shown.
- [ ] Scenario 1 answer is `amount / cap` computed correctly.
- [ ] Scenario 2 correctly identifies that the cap doesn't bind
      and the SAFE converts at the round price.
- [ ] Scenario 3 correctly identifies the shares-per-dollar
      multiplier (should be > 1× — SAFE gets more shares per
      dollar than a $12M-pre Series Seed investor).
- [ ] Scenario 4 stack sum is correct and shown as a linear
      addition.
- [ ] Scenario 5 uses the `pre × (1 − r)` stackable form for
      every SAFE and confirms the cross-check.
- [ ] Scenario 6 correctly identifies whether cap or discount
      wins by comparing effective prices.
- [ ] Scenario 7 shows the MFN swap changing the invariant
      answer and identifies who funds the change.
- [ ] Scenario 8 correctly recognises that the pre-money SAFE's
      ownership is not determined by the invariant, and names
      why in one sentence.

## Self-assessment rubric

<!-- needs-research: exemplar for mod-005 not yet authored; the rubric-vs-exemplar comparison assumes future exemplars/mod-005-equity-safes-cap-tables/. -->

| Dimension | Weak | Strong |
|---|---|---|
| Invariant application | Formula memorised but applied inconsistently | Every post-money SAFE answered as `amount / cap` without reference to other SAFEs |
| Cap-vs-round comparison | Founder assumes cap always binds | Compares cap and round explicitly; identifies which binds |
| Stack sums | SAFE-by-SAFE without a running total | Stack sum computed as `Σ (amount_i / cap_i)`; sanity-checked against pre-new-money FD |
| Priced-round dilution | New money treated as separate from SAFE dilution | Every pre-new-money holder recomputed as `pre × (1 − r)` post-close |
| Cap-vs-discount | Discount ignored or double-counted with cap | Both computed; the one giving the SAFE more shares wins |
| MFN mechanics | Assumes MFN is automatic | Recognises that MFN is *elected* and produces a specific pp change at conversion |
| Pre-money recognition | Applies post-money invariant to pre-money SAFE | Recognises the pre-money form does not obey the invariant and names the interaction reason |

## Definition of done

A skeptical seed-stage lead investor, handed your drill sheet,
would agree that (a) every answer is correct, (b) the
arithmetic is legible, and (c) you can apply the same
patterns to their own SAFE portfolio without opening a
spreadsheet.

> Solutions are not provided in this repository; they live in
> the paired solutions repo.
