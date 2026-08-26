---
stage: SEED
stages: [PRE-SEED, SEED]
pillar: equity
requires: [mod-004-fundraising-preseed-to-seed]
role_pathways: [founder-ceo, startup-finance-fundraising]
---

# Module 005 — Equity, SAFEs & Cap Tables

> **Stage:** PRE-SEED→SEED · **Pillar:** Equity · **Prereq:** mod-004

## Why this module

Equity is the currency you spend to buy time, talent, and capital. Every hire,
every SAFE, every priced round trades a slice of the company for something the
company needs *right now*. Founders who don't understand the math of that trade
end up ambushed by their own cap table two rounds later — surprised by how
little they own, how much the pool cost them, or how a "clean" SAFE stack
converted into a mess.

The cap table is not paperwork; it's the ledger of every promise the company
has ever made about future ownership. Reading it is a founder-level skill, on
the same shelf as reading the operating model (mod-003) or the investor funnel
(mod-004). If you can't state, in percentage points, what a $500k SAFE at a
$5M cap will cost you when it converts, you're outsourcing a decision only the
founder can make.

The most expensive mistake at this stage is optimizing the *headline* of a
term sheet (valuation, round size) while ignoring the *structure* (pool
refresh, SAFE stack, preference). A $10M cap that looks better than a $7M cap
can, after a large pool refresh and a stack of SAFEs, deliver *less* founder
ownership at close. Structure decides who owns what; the headline is the story
you tell about it.

## Learning objectives

After this module you can:

1. Read a **cap table** — common, preferred, options (issued and reserved),
   SAFEs and convertibles on the stack — and compute ownership through a
   round.
2. Understand a **SAFE** (post-money vs pre-money form, valuation cap,
   discount, MFN) and compute how it converts into equity at a priced round.
3. Size an **option pool**, understand the "pre-money pool" convention, and
   know **who** the pool dilutes and when.
4. Walk a company's cap table from founding through a priced seed, showing
   the dilution each instrument caused and where founder ownership ends up.
5. Name the two or three structural decisions in the current round that most
   affect founder ownership at the *next* round.

## Core concepts

### 1. What a cap table actually is

A capitalization table (or "cap table") is the ledger of every equity claim on
the company: shares issued, shares reserved for grant, and every promise (SAFE,
convertible note, warrant) that will become shares under some future condition.
Two views matter:

- **Issued.** Shares actually held by a person or entity today — the founders'
  common, options actually granted and vested, preferred stock from priced
  rounds.
- **Fully diluted (FD).** Everything that *would* exist if every reserved
  option was granted, every SAFE and note converted, every warrant exercised.
  FD is the number investors care about, because it's the denominator that
  determines ownership after the next round.

Percentage ownership is always `owner's FD share count / total FD share count`.
When the FD share count changes — a pool refresh, a SAFE conversion, a new
priced round — every non-purchaser's percentage moves. That movement is
**dilution**, and it is not optional; every share issued to someone new
dilutes everyone else.

### 2. The share classes on an early-stage cap table

Four classes cover almost every seed-stage cap table:

- **Common stock.** What founders and employees hold. Options grant the right
  to buy common at a fixed strike price; when exercised, they become common
  shares.
- **Preferred stock** (usually **Series Seed** or **Series A Preferred**).
  What investors get in a priced round. Preferred has rights common doesn't —
  a **liquidation preference** (default: 1× non-participating — preferred gets
  its money back first at exit, then converts to common and shares the upside
  pro rata), an **anti-dilution** provision (default: broad-based
  weighted-average — a formula that reprices in a down round), and consent
  rights on major decisions.
- **Options** (issued and reserved). Grants to employees, contractors, and
  advisors. Reserved options sit in the **option pool** until granted; issued
  options are already promised to someone, subject to vesting.
- **Convertibles on the stack** (SAFEs and notes). Not shares yet. Rights to
  buy shares at the *next* priced round, at a price determined by the SAFE
  or note terms. They convert automatically at the round; until then they are
  a promise, not an issued share.

You will occasionally see warrants, secondary common (from a founder tender),
and various stock plans. The four classes above are the load-bearing ones for
a first cap table.

### 3. Ownership arithmetic — how to compute a percentage

The universal rule is: `owner FD shares / total FD shares = ownership %`.

Two subtleties trip founders:

- The total FD share count includes every reserved-but-not-granted option.
  Founders who forget this over-report their own ownership because they're
  dividing by *issued* shares, not *FD* shares.
- After a SAFE or a priced round, new shares are issued — the denominator
  grows. Founder ownership goes *down* even though the founder's share count
  didn't change. That's dilution; it isn't punishment, it's arithmetic.

A useful sanity check: sum every stakeholder's FD % across the whole table.
It should sum to 100.0%. If it doesn't, someone is miscounted or an instrument
is missing.

### 4. The option pool — sizing, refresh, and who pays

Every institutional round expects the company to carry an **option pool** — a
block of common stock reserved for grants to employees, advisors, and future
hires. Two facts drive most of the founder pain here:

- **Typical size.** At seed, the pool is usually **10–15%** of the post-money
  FD cap table; at Series A, it's typically topped up ("refreshed") back to
  around 10–15% again after the round dilutes the prior pool. Later stages
  refresh smaller — the pool is largest, in percentage terms, when the
  company is smallest.
  <!-- needs-research: primary-source citation for the 10–15% seed pool norm — commonly cited in Carta pool-size data and in Y Combinator / Cooley round-size posts, but exact ranges shift by stage, sector, and geography. -->
- **Who pays for it.** This is the single most consequential structural detail
  a founder can miss. The market convention is that the pool is set up (or
  refreshed) **pre-money** — meaning the pool sits inside the pre-money
  valuation, and the pool comes out of the *existing shareholders'* stake,
  not the new investor's. In practice: if a lead demands a "15% post-close
  pool," the founders (and other existing holders) dilute themselves by
  roughly that whole 15% before the investor's money is even added to the
  denominator.

The lever a founder actually has is **pool size, not pool convention.** The
convention is standard and non-negotiable at most funds. The size is
negotiable — and every extra percentage point of pool is a percentage point
of founder dilution. The right size is the size the company will *actually
grant* between now and the next round, not the round-number the investor
asked for. If your hiring plan needs 6% in new grants over 18 months and 4%
is already granted-but-unvested, a 10% pool is defensible; a 15% pool is a
gift to the next round's investors.

### 5. SAFEs — what they are, what the terms mean

A **SAFE** (Simple Agreement for Future Equity, Y Combinator, 2013; revised
to the post-money form in 2018) is a contract that gives an investor the
right to receive shares at the *next* priced round, at a price determined by
the SAFE's terms. It is not debt (no maturity date, no interest) and not
equity yet (no shares issued until conversion). It exists to let pre-seed and
early-seed rounds close in days rather than months, without the legal cost
of a priced round.

Four terms carry almost all the weight:

- **Valuation cap.** The maximum valuation at which the SAFE converts. If the
  cap is $5M and the next priced round is at $20M, the SAFE converts as if
  the price were $5M — the SAFE holder gets ~4× more shares per dollar than
  a Series Seed dollar bought at $20M. If the cap is *higher* than the next
  round's valuation, the cap doesn't bind and the discount (if any) applies
  instead.
- **Discount.** A percentage discount off the priced-round share price —
  commonly 10–20%. A 20% discount at a $10M priced round converts the SAFE
  at an effective $8M price. Discount and cap coexist; whichever gives the
  SAFE holder more shares wins.
- **Pre-money vs post-money SAFE.** YC's original 2013 SAFE was **pre-money**:
  the cap referred to a valuation *before* other SAFEs converted, so a stack
  of pre-money SAFEs created ambiguous math and unpredictable founder
  dilution. The 2018 revision is **post-money**: the cap refers to the
  post-money valuation *including all SAFEs converted* but *before* the
  new-money priced round. Post-money SAFE ownership is calculable the moment
  the SAFE is signed — `SAFE amount / post-money cap = SAFE holder's
  ownership %`, guaranteed at conversion. Almost every SAFE written in 2019+
  is post-money; a pre-money SAFE still on the stack is worth reading
  carefully.
  <!-- needs-research: primary-source citation for YC's 2018 post-money SAFE revision and the "amount / cap = ownership %" invariant. Preferred source: ycombinator.com/documents (SAFE User Guide). -->
- **MFN** ("most favored nation"). A clause that says: if the company issues
  a later SAFE with more favorable terms (lower cap, higher discount), this
  SAFE holder can elect those terms instead. Common in early angel checks;
  a way for a small early check to keep up with a later lead.

Two more mechanics worth knowing:

- **Pro rata rights.** Some SAFEs (typically institutional pre-seed funds')
  carry a right to invest their pro rata share in the *next* priced round to
  maintain ownership. Not universal; negotiated separately, often via a side
  letter.
- **Side letters.** Investor-specific terms attached to a SAFE (information
  rights, MFN scope, pro rata) that don't appear on the SAFE itself. When
  counting the cap table, read the side letters too.

### 6. How a post-money SAFE converts — the arithmetic

For a post-money SAFE, at the priced round:

1. Compute the SAFE holder's fixed ownership: `SAFE amount / post-money cap`.
   For a $500k SAFE at a $5M post-money cap, that's `$500k / $5M = 10%`.
2. That 10% is 10% of the fully diluted cap table *immediately before the
   priced round's new money is added*, but *after* all SAFEs have converted
   and *after* any pre-money pool refresh required by the round. This is the
   "post-money" invariant: the SAFE's percentage is fixed regardless of what
   other SAFEs or pool refresh exist.
3. The priced round's new money then buys additional preferred at the round's
   price. That further dilutes every existing holder — including the
   just-converted SAFE.

The stackable form: if the SAFE ownership `s = SAFE amount / cap` and the
priced-round new-money ownership `r = round amount / round post-money`, then
after the round the SAFE holder ends up owning roughly `s × (1 − r)` — the
SAFE's fixed pre-new-money percentage, diluted by the new money.

Two implications founders regularly miss:

- **A stack of SAFEs sums.** Four $250k SAFEs at $5M post-money caps are,
  together, 20% of the company at conversion — the same as a single $1M SAFE
  at the same cap. Any founder counting "just one 5% SAFE at a time" without
  summing the stack is under-reporting their dilution.
- **A low cap is a big check, in ownership terms.** A $250k SAFE at a $2.5M
  cap is 10% of the company; the same $250k at a $10M cap is 2.5%. Cap
  dominates check size for founder dilution.

### 7. The priced-round mechanics — pre-money, post-money, price per share

A priced round issues new preferred shares at a defined price:

- **Pre-money valuation.** The company's valuation *before* the new money is
  added: `pre-money = pre-money FD share count × price per share`. The
  pre-money FD share count includes the refreshed pool and the converted
  SAFEs.
- **Post-money valuation.** `pre-money + round amount`.
- **Price per share.** `pre-money / pre-money FD share count`. New investors'
  shares = `round amount / price per share`.
- **New-money ownership.** `round amount / post-money valuation` — same
  number, from a different angle.

A worked example, walked in the exercise. Two co-founders each hold 5,000,000
common shares (10,000,000 total). A single $500k post-money SAFE sits at a
$5M cap. The priced seed is $2M at an $8M pre-money valuation and the lead
requires a 10% post-close option pool, refreshed pre-money.

At the round:

- The SAFE is contractually 10% of the pre-new-money, post-refresh FD.
- The pool refresh is set up pre-money to bring the pool to 10% post-close.
  That means the pool sits inside the $8M pre-money, diluting the founders
  (and, effectively, the just-converted SAFE holder relative to what they'd
  have owned without a pool).
- The $2M / $8M-pre round is 20% of the $10M post-money. New preferred =
  20% of the post-close FD; the remaining 80% is founders + SAFE + pool.

The final walk (rounded to whole percentage points for readability):

| Stakeholder                 | At founding | After SAFE signed | Post-round |
|---|---|---|---|
| Founder A                   | 50%         | 50% (SAFE off FD) | ~31%       |
| Founder B                   | 50%         | 50% (SAFE off FD) | ~31%       |
| SAFE holder                 | 0%          | 0% on FD (10% at conversion) | ~8% |
| Option pool (reserved)      | 0%          | 0%                | 10%        |
| Series Seed investor        | 0%          | 0%                | 20%        |
| **Total**                   | 100%        | 100%              | 100%       |

The exercise walks this arithmetic precisely, share by share.

### 8. The two or three decisions that matter most

Once you can do the arithmetic, the founder-level question is: which decisions
in *this* round are still moving the number that matters — founder ownership
at Series A?

- **Pool size, not pool convention.** The convention (pre-money refresh) is
  standard; the size is where the money is. Every extra percentage of pool is
  a percentage of founder dilution. Size the pool to a defensible 18-month
  hiring plan (from mod-003), not to the number the lead's counsel typed
  first.
- **SAFE cap and stack size.** Every SAFE you sign at a low cap is a large
  percentage sold at a small dollar amount. Post-money SAFEs make the math
  legible; that legibility is a tool *for* the founder, not against them —
  use it to know, before the priced round, exactly how much of the company
  you've already promised.
- **Round size and pre-money together, not separately.** A "higher valuation"
  achieved by taking a larger round at a smaller pre-money can dilute *more*,
  not less. Compare rounds by post-money founder ownership, not by the
  pre-money headline.

Two structural terms belong on this shortlist even though they live on the
term sheet, not the cap table: **liquidation preference** (default is 1×
non-participating; anything more aggressive — participating preferred, higher
multiples — is money coming out of the founders' pocket at exit) and
**anti-dilution** (default is broad-based weighted-average; full-ratchet is a
punitive term worth pushing hard to remove). *Venture Deals* is the reference
for both; call them out in the round docs even when the cap table looks
clean.
<!-- needs-research: primary-source citation for the "1× non-participating" and "broad-based weighted-average" defaults; Feld & Mendelson's *Venture Deals* is the canonical reference, and NVCA model documents (nvca.org) are the primary-source templates. -->

## The exercise

Model the cap table for a company from founding through a priced seed:
**two founders, a 10% option pool, a $500k SAFE at a $5M post-money cap,
and a $2M priced seed at an $8M pre-money valuation.** Compute ownership at
each step and show where the pool dilution lands. See
**[exercise-01-cap-table](./exercise-01-cap-table)**.

## Live-lab note

If you're an operating founder using this as a live lab: run the same walk
on **your** cap table. Start with your actual founders' split, list every
SAFE you've signed (cap, amount, pre- or post-money form), sketch the next
priced round you're likely to raise (from your mod-004 funnel), and compute
where your ownership lands. The scenario numbers are a scaffold; the point
of the exercise is to know your own numbers before a lead investor's counsel
does.

## Further reading

- Y Combinator, *SAFE Financing Documents* (ycombinator.com/documents) — the
  primary source for the SAFE, including the 2018 post-money revision, user
  guide, and side-letter templates.
- Y Combinator, *A Guide to Seed Fundraising* (Geoff Ralston) — where SAFEs,
  priced rounds, and pool sizing fit together at a seed round.
- Brad Feld & Jason Mendelson, *Venture Deals* — the term-sheet reference:
  liquidation preference, anti-dilution, pool math, and every clause worth
  negotiating on the paper.
- Fred Wilson, *AVC* (avc.com) — twenty years of essays on cap tables,
  dilution, and founder/investor economics.
- Carta, *State of Private Markets* and *Cap Table 101* — primary data on
  dilution norms and worked cap-table examples by stage.
- National Venture Capital Association, *Model Legal Documents*
  (nvca.org/model-legal-documents) — the industry-standard priced-round
  templates that most seed and Series A rounds start from.

> ⚠️ AI-assisted content under ongoing human review. Cross-reference primary
> sources; this is a learning resource, not advice for a specific situation.
