# Chapter 08 — Term-Sheet Clauses That Reach Into the Cap Table: Liquidation Preference and Anti-Dilution

> **Reads with:** module objective 7 — *recognise the two term-
> sheet clauses that reach into the cap table: liquidation
> preference (1× non-participating default; anything more
> aggressive is money out of the founders' pocket at exit) and
> anti-dilution (broad-based weighted-average default;
> full-ratchet is a punitive term worth pushing hard to remove).*

## Why these two clauses matter more than the rest

A seed or Series A term sheet has a dozen clauses that matter,
and *Venture Deals* (Feld & Mendelson) is the canonical
reference for reading all of them. This module singles out two
because they are the ones that **reach directly into the cap
table math** — one at exit, one in a down round — and both
have well-established defaults that a well-informed founder
should recognise on sight.

- **Liquidation preference.** How proceeds are distributed at
  exit before common shareholders see anything. The
  **default is 1× non-participating**. Anything more aggressive
  is money coming out of the founders' pocket at exit.
- **Anti-dilution.** How preferred is repriced if the company
  later issues shares at a lower price. The **default is
  broad-based weighted-average**. **Full-ratchet** is a
  punitive alternative worth pushing hard to remove.

Every other clause on a seed or Series A term sheet is
important — board composition, protective provisions,
information rights, drag-along, pro-rata — but this module
teaches the two that show up as arithmetic in the cap table
under stress.
<!-- needs-research: primary-source citation for the seed / Series A term-sheet defaults; the NVCA model documents (nvca.org/model-legal-documents) and Brad Feld & Jason Mendelson's *Venture Deals* are the canonical references. -->

## Liquidation preference — what it is and what the defaults mean

**Liquidation preference** is the amount preferred shareholders
are entitled to receive at a liquidation event (sale of the
company, IPO in some cases, dissolution) **before** common
shareholders receive anything.

Three parameters:

- **Multiple.** The dollar amount, as a multiple of the amount
  originally invested. `1×` means the preferred gets its money
  back before common; `2×` means it gets twice its money back;
  `3×` (rare, and a red flag) means three times.
- **Participation.** After the preference is paid, does the
  preferred **also** share in the remaining upside as if it
  were common? **Non-participating** = no (the default, and
  the founder-friendly answer). **Participating** = yes (worse
  for common; the preferred double-dips).
- **Seniority within the stack.** In multi-round companies,
  each series has its own preference. Most commonly, the
  **most recent** series is senior to earlier ones; older
  preferred is paid only after newer preferred's preference
  is satisfied. This is the **stacked** default. **Pari-passu**
  means all preferred is paid pro rata; sometimes appears in
  down-round scenarios.

The seed and Series A **default** — and what the NVCA model
documents put in the standard template — is **1× non-participating
preferred, stacked**. Anything more aggressive is a deviation
from market that a founder should recognise, question, and
push to remove.
<!-- needs-research: primary-source citation for the "1× non-participating, stacked" default at seed and Series A; NVCA model documents and *Venture Deals* are the canonical references. -->

## Worked example: 1× non-participating vs 1× participating

Assume the standard scenario cap table at close, with the
Series Seed lead having invested $2M for **20%** of a $10M
post-money company. Now the company exits at three prices:
$50M, $10M, and $8M.

### Case A: 1× non-participating (the default)

The Series Seed holder is entitled to `1× $2M = $2M` in
preference, **or** to convert to common and take 20% of the
exit, **whichever is larger**.

- **Exit at $50M.**
  - Preference route: $2M.
  - Conversion route: 20% × $50M = $10M.
  - Series Seed takes conversion → **$10M** to Series Seed;
    **$40M** to common (founders + pool + SAFE-converted
    preferred, distributed pro rata).
- **Exit at $10M.**
  - Preference route: $2M.
  - Conversion route: 20% × $10M = $2M.
  - Series Seed indifferent; typical model shows conversion
    at the crossover point → **$2M** each way; **$8M** to
    common.
- **Exit at $8M.**
  - Preference route: $2M.
  - Conversion route: 20% × $8M = $1.6M.
  - Series Seed takes preference → **$2M** to Series Seed;
    **$6M** to common (which is `$6M / 62% ≈ $9.68M
    pre-preference` distributed across the non-preferred
    cap table, so the founders get roughly `31%/62% × $6M
    = $3M` each).

In each case, common shareholders receive **everything above
the preference amount**, distributed pro rata across the
converted-common cap table. That is the founder-friendly
behaviour.

### Case B: 1× participating

Same $2M investment for 20% of a $10M post-money. Now the
Series Seed **participates**: it gets its $2M preference
**and** its 20% share of the remaining upside.

- **Exit at $50M.**
  - Series Seed: $2M preference + 20% × ($50M − $2M) =
    $2M + $9.6M = **$11.6M**.
  - Common: $50M − $11.6M = **$38.4M**.
  - Difference vs non-participating case: **$1.6M more to
    Series Seed, $1.6M less to common** at this exit
    price.
- **Exit at $10M.**
  - Series Seed: $2M + 20% × ($10M − $2M) = $2M + $1.6M
    = **$3.6M**.
  - Common: **$6.4M**.
  - Difference: **$1.6M more to Series Seed, $1.6M less to
    common** than non-participating.
- **Exit at $8M.**
  - Series Seed: $2M + 20% × ($8M − $2M) = $2M + $1.2M
    = **$3.2M**.
  - Common: **$4.8M**.
  - Difference: **$1.2M more to Series Seed, $1.2M less to
    common** than non-participating.

Participating preferred takes real money out of the founders'
pocket at every exit price. And it compounds when there are
multiple series of participating preferred — each series
takes its participation before common sees anything.

### Case C: 2× non-participating

Same $2M investment for 20%. Now the preference is `2× $2M =
$4M`.

- **Exit at $50M.**
  - Preference route: $4M.
  - Conversion route: 20% × $50M = $10M.
  - Series Seed takes conversion → **$10M** to Series Seed
    (no change from 1× non-participating at this size).
- **Exit at $10M.**
  - Preference route: $4M.
  - Conversion route: 20% × $10M = $2M.
  - Series Seed takes preference → **$4M** to Series Seed;
    **$6M** to common (vs $8M under 1× non-participating —
    the founders lost $2M).
- **Exit at $8M.**
  - Preference route: $4M.
  - Conversion route: 20% × $8M = $1.6M.
  - Series Seed takes preference → **$4M** to Series Seed;
    **$4M** to common (vs $6M under 1× non-participating).

At every exit price *below the crossover*, the higher multiple
takes real money from common. At exits *above the crossover*,
the multiple doesn't bind — but "the crossover" moves further
out with every preference multiple above 1×.

## What to redline on liquidation preference

Founders should recognise, and push back on, any deviation
from the default:

- **Participating preferred.** Push to remove. If the lead is
  firm, negotiate a **cap on participation** ("2× cap" — the
  preferred stops participating after receiving 2× its
  investment total, at which point it converts to common).
- **Multiples above 1×.** Push to remove. `2×` in the current
  seed market is a red flag; `3×` or higher is a term
  founders should refuse.
- **Broken seniority** (a later round demanding pari-passu
  when the earlier round is stacked). Read the whole
  preference stack; know who is paid first.

The number to remember when reading a term sheet: **1×
non-participating, stacked**. That is the founder-friendly
default; anything more aggressive is money coming out of the
founders' pocket at exit.

## Anti-dilution — how preferred is repriced in a down round

**Anti-dilution** is the clause that adjusts the preferred's
**conversion price** (the effective price at which preferred
converts to common) if the company later issues shares at a
**lower** price per share (a "down round"). Without an
anti-dilution clause, a down round dilutes preferred just as
much as it dilutes common; with the clause, preferred is
partially protected.

Two forms dominate:

- **Broad-based weighted-average.** The default. The preferred's
  conversion price is adjusted by a formula that weights the
  size of the down round against the whole post-conversion FD
  share count. Mild adjustment; a small down round produces a
  small adjustment.
- **Full-ratchet.** The preferred's conversion price resets to
  the new low price *regardless of round size*. Even a tiny
  down round produces a full reset. Historically punitive;
  worth pushing hard to remove.

A third form, **narrow-based weighted-average**, uses a
different denominator (only preferred, not full FD) and
produces a somewhat larger adjustment than broad-based. Less
common but worth recognising.

## Weighted-average anti-dilution — the formula

The broad-based weighted-average formula, in words:

```
new conversion price = old conversion price × (A + B) / (A + C)

where:
  A = FD shares outstanding immediately before the down round
  B = shares that would have been issued in the down round at
      the old conversion price
  C = shares actually issued in the down round at the new
      (lower) price
```

Concretely: a Series Seed that invested at a $0.62 conversion
price into the standard scenario (chapter 06), followed by a
Series A down round that issued shares at $0.40 per share.
Assume Series A raised $4M at the new price.

- `A` = post-close FD from chapter 06 ≈ **16,129,032 shares**.
- `B` = $4M / $0.62 = **~6,451,613 shares** (what the round
  would have been at the old price).
- `C` = $4M / $0.40 = **10,000,000 shares** (what the round
  actually is at the new price).

```
new conversion price = $0.62 × (16,129,032 + 6,451,613) / (16,129,032 + 10,000,000)
                     = $0.62 × (22,580,645 / 26,129,032)
                     = $0.62 × 0.8642
                     ≈ $0.5358
```

The Series Seed's conversion price drops from $0.62 to
~$0.54 — a mild adjustment. The preferred's effective
ownership grows slightly at the expense of common; the
adjustment does not devastate the common holders.

## Full-ratchet anti-dilution — the punitive version

Under **full-ratchet**, the same scenario resets the Series
Seed conversion price to the **new** price, $0.40, regardless
of round size:

```
new conversion price = $0.40 (full ratchet)
```

That is a **35% price reset** on the Series Seed's original
conversion — which translates into the Series Seed getting
`0.62 / 0.40 = 1.55×` more shares on conversion than it
originally would have. That extra 55% of Series Seed shares
comes directly out of common.

Full-ratchet applied to a small down round (say, a $500k
bridge at a slightly lower price) produces the *same* full
reset — a tiny amount of new dilution to preferred causes an
enormous adjustment across the whole prior preferred stack.
That asymmetry is why full-ratchet is called punitive.

## What to redline on anti-dilution

- **Full-ratchet.** Push hard to remove. Full-ratchet at seed
  is a market outlier; at Series A it appears occasionally
  and is worth resisting.
- **Narrow-based weighted-average.** Prefer broad-based if
  possible; narrow-based produces a bigger adjustment.
- **No "pay-to-play" carve-out.** A **pay-to-play** provision
  says that a preferred holder who **doesn't** participate
  pro rata in the down round *loses* their anti-dilution
  protection. This aligns incentives — anti-dilution
  protects investors who keep supporting the company, not
  those who bail — and is worth requesting if the standard
  isn't already pay-to-play.
  <!-- needs-research: primary-source citation for pay-to-play mechanics; *Venture Deals* is the canonical reference. -->
- **Broad exclusions from anti-dilution triggers.** Standard
  exclusions include option-pool grants, warrants issued to
  strategic partners, and shares issued in acquisitions.
  Anti-dilution should trigger on genuine down rounds of
  common financing, not on ordinary business shares.

The number to remember: **broad-based weighted-average**.
That is the founder-friendly default; **full-ratchet** is the
punitive alternative worth pushing hard to remove.

## The two clauses on the term sheet — what to look for

When you receive a term sheet, find these two clauses first
and read them against the defaults:

- **"Liquidation Preference"** section: look for the
  **multiple** (should be 1×), **participation** (should be
  non-participating), and **seniority** (should be stacked
  with newest-senior in a multi-round company).
- **"Anti-dilution"** section: look for the **type**
  (should be broad-based weighted-average), any **exclusions**
  from the trigger, and any **pay-to-play** provision.

Any deviation from the defaults is a redline. Chapter 09
covers how to bring the redlined term sheet to counsel and
how the founder / counsel handoff works — counsel delivers
the legal opinion; the founder authors the redline.

## What is *not* in this chapter (and why)

Term sheets have many other clauses that matter. This chapter
skips them because they do not reach into the cap-table math
in the same way:

- **Board composition** — governance, not cap table. Owned by
  the operations-and-governance track.
- **Protective provisions** — consent rights on major
  decisions; matter enormously but don't produce a cap-table
  number.
- **Drag-along and tag-along** — mechanics of exit and
  secondary sales.
- **Pro-rata rights** — right to invest in future rounds;
  covered in chapter 03 as a SAFE-side term.
- **Information rights** — quarterly reporting cadence.

*Venture Deals* covers all of them; this module scopes to the
two that show up in the cap table under stress.

## Common wrong versions

- **Focusing on valuation, ignoring preference.** Founder
  accepts a slightly higher pre-money in exchange for 2×
  participating preferred. At a middling exit, this trade
  produces less founder cash-in-hand than the original
  offer.
- **Signing full-ratchet without noticing.** Because
  full-ratchet is rare, it's easy to miss when it appears
  in a term-sheet template. Every anti-dilution clause
  should be read explicitly.
- **Assuming the "market" clause is founder-friendly.**
  Some fund templates default to more aggressive terms
  than the NVCA model. "Standard for our fund" is not the
  same as "standard for the market."
- **Redlining without counsel review.** Founders should
  identify the redlines; counsel drafts them and confirms
  the exact language. Chapter 09 covers the handoff.

## Summary

- Two term-sheet clauses reach into the cap-table math:
  **liquidation preference** (at exit) and **anti-dilution**
  (in down rounds).
- The **defaults** at seed and Series A are **1×
  non-participating preferred, stacked** and **broad-based
  weighted-average anti-dilution**. Recognise them on sight;
  anything more aggressive is money coming out of the
  founders' pocket at exit or in a down round.
- **Participating preferred, multiples above 1×, and
  full-ratchet anti-dilution** are the three deviations
  worth pushing hardest to remove. **Pay-to-play** is a
  provision worth requesting.
- Other term-sheet clauses matter (board, protective
  provisions, drag-along, information rights) but don't
  produce a cap-table number under stress. See *Venture
  Deals* for the full read.

**Next:** how to brief legal counsel with a cap-table walk
and a term-sheet redline the founder authored themselves —
and where the founder-authored artifact stops and the legal
opinion begins — in
[chapter 09](./09-briefing-counsel-and-the-redline.md).
