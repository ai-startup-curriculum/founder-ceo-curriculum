# Chapter 02 — How Much To Raise: From the Operating Model, Tied to a Milestone, Priced in Dilution

> **Reads with:** module objective 2 — *compute how much to raise
> from the mod-003 operating model, tied to a specific 12–24 month
> milestone, with the resulting seed dilution range (~15–25%)
> stated.*

## A raise is a purchase, not a trophy

The most expensive early fundraising mistake is treating the round
size as a marketing number — "we want to raise a $3M seed" as if the
number itself signals ambition. It doesn't. The round size is the
**purchase price of time**, and the correct number falls out of two
inputs and nothing else:

- **The mod-003 operating model** — the 18-month, cash-forward plan
  that names every hire, every dollar of non-payroll spend, and the
  zero-cash date that results.
- **The milestone the round has to buy** — the specific,
  investor-recognisable evidence you need to raise the *next* round
  at a step up.

If the round size doesn't fall out of those two things, it is a
vibe. And a vibe-priced round is either too small (you're raising
again the moment it closes) or too big (the dilution is unjustified
and the next round has to grow into it). Both are worse than the
right number.

## The three-part arithmetic

The mechanical version of "how much to raise" has three parts.

### Part 1 — cost of the milestone

Reopen the mod-003 model. Ask: **what does it cost to run the
company from close-of-round to the milestone I'm going to sell as
the reason for the next round?**

That number is the sum of:

- **Payroll to the milestone.** Every current person plus every
  planned hire, at fully-loaded cost (see mod-003 chapter 03), from
  the round-close month through the milestone month.
- **Non-payroll spend to the milestone.** Hosting, tools, legal,
  contractors, marketing — the whole non-payroll section of the
  operating model, summed over the same window.
- **Minus expected cash in.** Whatever customer revenue the model
  says will land in the window, at the assumption you're willing to
  defend to a partner. Be conservative — a raise that depends on
  hitting a revenue forecast is a raise that gets in trouble when
  the forecast slips.

Call that number **`M`** — the cost of the milestone.

### Part 2 — post-milestone runway buffer

You don't want cash to hit zero the month you hit the milestone. You
want **6–9 months of runway** *after* the milestone, so that you can
open the next round from strength rather than from panic. Chapter 06
of mod-003 explains why the raise-by month is 6–9 months before
zero cash; the same math applies to the *next* raise, backwards from
the next zero-cash date.

So add a buffer of roughly **6–9 months of post-milestone burn** on
top of `M`. Call that buffer **`B`**. The right burn number for the
buffer is post-hire, post-milestone burn — usually noticeably higher
than today's burn, because the team is bigger by then.

### Part 3 — the raise itself

The raise number is roughly:

```
raise ≈ M + B
```

That is the amount that (a) pays for the milestone and (b) leaves
6–9 months of post-milestone runway to raise the next round. It is
the number to name in the pitch and defend in the model.

Two sanity checks:

- **Runway post-close.** Divide the raise by the average monthly
  gross burn between close and milestone. That number should land in
  the **18–24 month** range. Less than 12 and you're raising again
  immediately; more than 30 and you're either raising more than the
  milestone justifies or the milestone is set too far out.
  <!-- needs-research: primary-source citation for the 18–24 month post-raise runway norm; commonly repeated in the Y Combinator *A Guide to Seed Fundraising* (Geoff Ralston) and Sequoia writings, exact origin varies. -->
- **Milestone fit.** Would a plausible Series A partner, reading the
  milestone in isolation, agree that reaching it justifies opening a
  Series A conversation? If not, either the milestone is too small
  (raise less, aim for a bigger one next) or the wrong shape (raise
  the same, aim for a different one).

## What a "milestone" actually means

The milestone is not "grow the team" or "ship the product." A
fundable milestone is a **specific, investor-recognisable piece of
evidence** — the kind of sentence a partner would put in the
first paragraph of an investment memo.

Examples (US SaaS, illustrative — calibrate to your sector and
stage):

- *"Reach $1.5M ARR at ≥ 100% net revenue retention with a working
  outbound channel that pays back CAC in < 12 months."*
- *"Sign 10 enterprise design partners at ≥ $50k ACV, each with a
  measurable outcome, and convert 6 into paid contracts by
  month 12."*
- *"Ship v1, reach 5,000 weekly active users, and demonstrate ≥ 30%
  week-4 retention on a defined onboarding cohort."*
- *"Close 3 lighthouse enterprise customers in the target ICP at ≥
  $100k ACV and demonstrate a repeatable sales cycle < 6 months."*

Each one is testable — a partner can read it and know whether the
evidence exists. And each one is **the story for the next round**:
if the milestone lands, the Series A raise pitches *the working
version of the story that the seed round raised on the promise of*.

Common failure modes:

- **Milestone is a lagging indicator you can't influence.** "Get
  featured in the Wall Street Journal" is not a milestone.
- **Milestone is an activity, not an outcome.** "Ship v1" alone is
  not a milestone; "ship v1 and demonstrate the retention curve" is.
- **Milestone is priced to the wrong next round.** A seed milestone
  should be sized to open a Series A conversation, not to open a
  Series B or a Series A-2 bridge.

## Dilution — the price you pay for the raise

Cash is not free. Every raise is a **sale of ownership in the
company**, and the total ownership you sell across all rounds is
finite — a founder who has sold 60% of the company by Series A is
in a materially different governance position than one who has sold
30%.

At seed, the expected dilution for a priced round is roughly
**15–25%** of post-money ownership. Mod-005 walks through the
arithmetic of SAFE cap → priced conversion → new-money dilution →
option-pool refresh; here it is enough to know the range and the
implications.
<!-- needs-research: primary-source citation for the 15–25% seed dilution norm; the range is repeated by Y Combinator's *A Guide to Seed Fundraising*, Fred Wilson (AVC), and Brad Feld / Jason Mendelson's *Venture Deals*, but exact origin varies. Verify against recent Carta *State of Private Markets*. -->

The relationship between raise size, valuation, and dilution is:

```
new-money dilution ≈ raise / post-money valuation
post-money valuation = pre-money + raise
```

For a $3M raise at a $12M post-money valuation, the new money owns
**25%** and the pre-existing cap table has been diluted by that
same 25%. For a $3M raise at a $20M post-money valuation, the new
money owns **15%**. Same cash, different price — and it is the
price the market will bear on your evidence and story, not the
number you decide you want.

Two heuristics for interpreting your own arithmetic:

- **If your calculation says you need to sell more than 25% at
  seed, either the valuation is too low or the round is too big
  for the story.** Selling 40% at seed leaves the cap table
  under-water for the Series A investor — they will need to take
  another 20–25%, and now the founders and early team are below
  50%. That is a structurally worse company to run.
- **If your calculation says you need to sell less than 15% at
  seed, you likely didn't raise enough, or the price was too high
  to be defensible at the Series A mark.** The Series A investor
  underwrites against a valuation that has to grow into itself; if
  the seed price was aggressive, the Series A becomes a
  flat-or-down round even when the milestone lands.

The comfortable range at seed — enough capital, honest valuation —
is **15–25% dilution**. Outside that range, look at the raise size
and the milestone before you look at the valuation.

## Worked example (illustrative, not prescriptive)

To make the arithmetic concrete, run through it once with round
numbers. **These numbers are illustrative** — plug in your own
mod-003 model.

Assume:

- Round closes month 0.
- Milestone is reached month 15.
- Cost of the milestone (`M`): payroll + non-payroll − expected
  cash in, summed months 1–15 → **$2.1M**.
- Average post-hire monthly gross burn between month 15 and month
  21: **$120k/mo**.
- Post-milestone buffer of **8 months** at $120k/mo → **`B` =
  $0.96M**.
- Raise ≈ `M + B` = **$3.06M** → round up to a clean **$3.0M–$3.1M**.

Sanity checks:

- Average monthly gross burn between close (month 0) and milestone
  (month 15) is roughly $2.1M / 15 ≈ **$140k/mo**; raise divided by
  that burn is $3.1M / $140k ≈ **22 months of runway**. Within the
  18–24 month band.
- The milestone ("10 paying design partners at ≥ $3k ARPA / $360k
  ARR trajectory") is a story a Series A partner could underwrite
  as an opening question — plausible, testable, sized to the
  round.

Now the dilution frame. At a **$12M post-money** ($9M pre-money +
$3M raise), the new money owns **25%** — the top of the healthy
band. At a **$15M post-money**, new money owns **20%** — the
middle. At a **$20M post-money**, new money owns **15%** — the
bottom.

Which of those the market will support depends on the evidence you
walk in with and the sector; the model doesn't pick the price, but
the model tells you which raise size / dilution combinations are
even worth pitching.

## What if the number I get is too big?

A common outcome of the first pass through this arithmetic is a
raise size that is honest but implausible for the evidence you have
— e.g., "$5M seed" when the story is really a pre-seed story. Three
levers, in order of preference:

- **Shrink the milestone.** Aim for a smaller, still-fundable next
  step that costs less to reach. Not every seed round has to buy a
  Series-A-shaped milestone; a smaller round to a stronger seed
  extension is a legitimate path.
- **Shrink the team plan.** If the milestone can be reached by 6
  people instead of 10, the cost of the milestone drops. Mod-003's
  fully-loaded-hire discipline (chapter 03) is where this lever
  lives.
- **Split into two rounds.** A pre-seed on SAFEs now, a priced seed
  after the wedge is proven, is often the honest answer when the
  gap between current evidence and the "$5M seed" story is too
  wide.

Do **not** solve the problem by raising the milestone to justify
the round size. That is how founders end up raising against a story
they cannot deliver — the round closes, and the next 18 months are
spent trying to make the pitch true instead of building the
business.

## What if the number I get is too small?

The mirror problem: the model says $1M is enough, but the honest
next-round story requires a bigger team than $1M pays for. Usually
this means one of:

- The model under-counts fully-loaded cost (mod-003 chapter 03).
- The milestone is easier to reach than the story implies, so the
  next round is smaller than the current founder is anticipating —
  raise the smaller amount and plan to raise again from strength.
- The buffer `B` is too thin. A 3-month post-milestone buffer will
  not survive a raise process; extend it to 6–9 months and re-run.

In practice a raise smaller than about $1.5M is usually a
pre-seed, not a seed, and the round structure and target investors
should shift accordingly (see
[chapter 01](./01-fundraising-ladder.md)).

## The four common wrong versions

- **Round size picked from vibes.** "We're raising $3M" with no
  operating model behind it. When a partner asks "why $3M?", the
  founder cannot answer without opening a spreadsheet in the
  meeting.
- **Round size without a milestone.** A raise that is not tied to
  a specific piece of investor-recognisable evidence never ends —
  the founder spends the money and then has to explain to the
  next partner what the round was for.
- **Milestone set to justify the round.** The founder wants to
  raise $5M, so the milestone gets promoted to a Series-A-worthy
  outcome the current team cannot plausibly deliver. Now the round
  closes on a lie and the 18 months after it are unhappy.
- **Dilution ignored.** The founder optimises for "as much cash as
  possible" and sells 35% at seed. The Series A investor then
  discovers a broken cap table and either passes or takes so much
  to fix it that the founders are minority owners by Series B.

## Summary

- The right round size falls out of two inputs: **cost of the
  milestone** (from the mod-003 model) plus a **6–9 month
  post-milestone runway buffer**. Everything else is a vibe.
- The **milestone** is a specific, investor-recognisable piece of
  evidence that opens the next round — testable, outcome-based,
  sized to the appropriate next-round conversation.
- Sanity-check the raise on **post-close runway** (18–24 months is
  the healthy band) and on **seed dilution** (15–25% is the
  healthy band; mod-005 covers the arithmetic).
- If the number is too big for the evidence, shrink the milestone
  or split into two rounds. Do **not** inflate the milestone to
  justify a bigger raise.

**Next:** how to turn the raise size into a **funnel** of segmented
investor targets with named conversion assumptions — in
[chapter 03](./03-investor-funnel-and-conversion.md).
