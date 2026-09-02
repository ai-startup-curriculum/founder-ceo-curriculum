---
stage: SEED
stages: [PRE-SEED, SEED]
pillar: equity
requires: [mod-004-fundraising-preseed-to-seed]
role_pathways: [founder-ceo, startup-finance-fundraising]
---

# Module 005 — Equity, SAFEs & Cap Tables

> **Stage:** PRE-SEED→SEED · **Pillar:** Equity · **Prereq:**
> mod-004

Equity is the currency you spend to buy time, talent, and
capital. Every hire, every SAFE, every priced round trades a
slice of the company for something the company needs *right now*.
Founders who don't understand the math of that trade end up
ambushed by their own cap table two rounds later — surprised by
how little they own, how much the pool cost them, or how a
"clean" SAFE stack converted into a mess.

The cap table is not paperwork; it's the ledger of every promise
the company has ever made about future ownership. Reading it is a
founder-level skill, on the same shelf as reading the operating
model (mod-003) or the investor funnel (mod-004). If you can't
state, in percentage points, what a $500k SAFE at a $5M cap will
cost you when it converts, you're outsourcing a decision only the
founder can make.

The most expensive mistake at this stage is optimising the
*headline* of a term sheet (valuation, round size) while
ignoring the *structure* (pool refresh, SAFE stack, preference).
A $10M cap that looks better than a $7M cap can, after a large
pool refresh and a stack of SAFEs, deliver *less* founder
ownership at close. Structure decides who owns what; the
headline is the story you tell about it.

Deeper post-Series-A cap-table craft, employee-stock-plan
administration, 409A valuations, and secondary transactions are
deferred to the `startup-finance-fundraising-curriculum` peer
track. The handoff is made explicit in
[chapter 10](./10-boundaries-finance-and-cap-table-craft.md).

## Learning objectives

After this module you can:

1. **Read a cap table** — common, preferred, options (issued
   and reserved), SAFEs and convertibles on the stack — and
   compute ownership through a round on a fully-diluted basis.
2. Distinguish the **four early-stage share classes**: common
   (founders + employees), preferred (priced-round investors,
   with 1× non-participating liquidation preference and
   broad-based weighted-average anti-dilution as defaults),
   options (issued + reserved in the option pool), and
   convertibles (SAFEs + notes) on the stack.
3. Understand a **SAFE** (Y Combinator, 2013; post-money form,
   2018) — valuation cap, discount, MFN, pre-money vs post-
   money form — and compute how a post-money SAFE converts
   using the `SAFE amount / post-money cap = ownership %`
   invariant.
4. Size an **option pool** (~10–15% at seed, refreshed
   pre-money) tied to the mod-003 hiring plan rather than the
   round-number the lead's counsel typed first, and understand
   that the pool comes out of *existing shareholders'* stake,
   not the new investor's.
5. Walk a company's cap table from founding through a priced
   seed — two founders + 10% option pool + $500k post-money
   SAFE at a $5M cap + $2M priced seed at an $8M pre-money —
   showing the dilution each instrument caused.
6. Name the **three structural decisions** in the current
   round that most affect founder ownership at the *next*
   round: pool size (not convention), SAFE cap and stack size,
   round size and pre-money together (not the headline).
7. Recognise the **two term-sheet clauses** that reach into
   the cap table: **liquidation preference** (1× non-
   participating default; anything more aggressive is money
   out of the founders' pocket at exit) and **anti-dilution**
   (broad-based weighted-average default; full-ratchet is a
   punitive term worth pushing hard to remove).
8. **Brief legal counsel** with a defensible cap-table walk
   and term-sheet redline, and route the legal opinion to
   counsel — this module reads and authors the paper, counsel
   delivers opinion.
9. Locate the **boundary to
   `startup-finance-fundraising-curriculum`** (level 30) for
   deep priced-round mechanics beyond the seed, employee-
   stock-plan administration, 409A valuations, secondary
   transactions, and post-Series-A cap-table craft.

## Chapters

| # | Chapter | Reads with objective |
|---|---|---|
| 01 | [What a Cap Table Actually Is: Issued, Fully Diluted, and Ownership Arithmetic](./01-cap-table-fundamentals.md) | 1 |
| 02 | [The Four Share Classes on an Early-Stage Cap Table](./02-four-share-classes.md) | 2 |
| 03 | [SAFE Anatomy: Cap, Discount, MFN, and the Pre-Money vs Post-Money Form](./03-safe-anatomy.md) | 3 |
| 04 | [Post-Money SAFE Conversion Math: The Amount / Cap Invariant](./04-post-money-safe-conversion-math.md) | 3 |
| 05 | [Option Pool Sizing: Tie It to the Hiring Plan; Know Who Pays](./05-option-pool-sizing-and-who-pays.md) | 4 |
| 06 | [The Walked Example: Founding → SAFE → Priced Seed](./06-cap-table-walk-founding-to-priced-seed.md) | 5 |
| 07 | [The Three Structural Decisions That Most Move Founder Ownership](./07-three-structural-decisions.md) | 6 |
| 08 | [Term-Sheet Clauses That Reach Into the Cap Table: Liquidation Preference and Anti-Dilution](./08-term-sheet-clauses-liq-pref-anti-dilution.md) | 7 |
| 09 | [Briefing Counsel: The Founder Authors the Cap-Table Walk and the Redline; Counsel Delivers the Legal Opinion](./09-briefing-counsel-and-the-redline.md) | 8 |
| 10 | [Boundaries: This Module Owns the Seed-Stage Cap Table; Peer Tracks Own Post-Series-A Depth and Stock-Plan Administration](./10-boundaries-finance-and-cap-table-craft.md) | 9 |

Read in order. Chapters 01–02 establish the language; 03–04 dive
into SAFEs; 05 handles the option pool; 06 puts it all together
in the walked example; 07 names the levers; 08 covers the two
term-sheet clauses that reach into cap-table math; 09 covers the
counsel handoff; 10 marks the boundary to the finance track.

## Exercises

The exercises progress from arithmetic drills to a full walked
cap table to a term-sheet redline. Do them in order for the
first pass; on live-lab reruns, order to match whichever round
you're actually working.

| # | Exercise | Time | Reads with chapter |
|---|---|---|---|
| 01 | [Cap Table: Founders + Pool + SAFE + Priced Seed](./exercises/exercise-01-cap-table.md) | ~6–8 hr | 01, 02, 04, 05, 06 |
| 02 | [Post-Money SAFE Conversion Arithmetic Drill](./exercises/exercise-02-post-money-safe-conversion-arithmetic-drill.md) | ~2 hr | 03, 04 |
| 03 | [Option Pool Sizing Tied to Hiring Plan](./exercises/exercise-03-option-pool-sizing-tied-to-hiring-plan.md) | ~2–3 hr | 05 |
| 04 | [Term-Sheet Redline Drill](./exercises/exercise-04-term-sheet-redline-drill.md) | ~2 hr | 08, 09 |

Exercise 02 is a good warm-up if you've never applied the
post-money SAFE invariant to a real stack; exercise 01 is the
load-bearing walk-through that most references the rest of the
module; exercise 03 depends on your mod-003 hiring plan
(exercise 01 in that module); exercise 04 is best done after
chapters 08 and 09.

Solutions are not provided in this repository; they live in the
paired solutions repo. Reference deliverables — if and when
authored — will live under
`exemplars/mod-005-equity-safes-cap-tables/`.
<!-- needs-research: exemplar for mod-005 not yet authored; the exercise rubrics reference a future exemplars/mod-005-equity-safes-cap-tables/. -->

## Resources

Real, citable references — YC's SAFE documents (2013 form and
2018 post-money revision), *Venture Deals* (Feld & Mendelson),
NVCA model legal documents, Carta cap-table data, Cooley GO's
startup-form library, and adjacent-track pointers — are
collected in [`resources.md`](./resources.md).

## Live-lab note

If you're an operating founder using this as a live lab: run
the walk on **your** cap table. Start with your actual founders'
split, list every SAFE you've signed (cap, amount, pre- or post-
money form, any side letters), sketch the priced round you're
likely to raise next (from your mod-004 funnel), and compute
where your ownership lands. The scenario numbers in the exercises
are a scaffold; the point of the exercises is to know your own
numbers before a lead investor's counsel does.

The two term-sheet clauses in chapter 08 are worth reading against
whatever term sheet you *last saw* (yours, a peer founder's,
someone else's leaked one). Every deviation from the defaults is
either founder cost or a signal about the lead's operating style.

---

> ⚠️ AI-assisted content under ongoing human review.
> Cross-reference primary sources; this is a learning resource,
> not advice for a specific situation.
