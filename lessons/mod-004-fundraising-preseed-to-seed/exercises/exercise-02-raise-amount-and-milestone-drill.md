# Exercise 02 — Raise Amount & Milestone Drill

**Module:** 004 Fundraising: Pre-seed → Seed · **Stage:** PRE-SEED
→SEED · **Time:** ~2–3 focused hours · **Reads with:** chapters
[01](../01-fundraising-ladder.md) and
[02](../02-raise-amount-milestone-dilution.md).

## Problem statement

You have (or will have) an 18-month operating model from mod-003.
You do **not** yet have a defensible answer to the question a
partner asks in the first ten minutes of the pitch: *"why are you
raising $X, and what does $X buy?"*

This exercise produces that answer. You compute the raise size
from the mod-003 model, tie it to a specific
investor-recognisable milestone, sanity-check it against the
post-close runway and seed-dilution norms, and write a one-line
"raise thesis" you can defend in a meeting without opening a
spreadsheet.

## Deliverables (two founder artifacts, plus one call)

1. **The raise arithmetic** — cost of the milestone (`M`) +
   post-milestone runway buffer (`B`) → raise amount, sanity-
   checked against post-close runway (target 18–24 months) and
   seed dilution (target 15–25% for a priced round).
2. **The milestone statement** — a specific, testable,
   investor-recognisable sentence naming what the round will
   have bought by month 12–24.
3. **A one-line raise thesis** — the sentence you use when a
   partner asks *"why $X?"* — round size, milestone, and
   post-close runway in one breath, defensible without opening a
   sheet.

## Scenario

Pick one:

- **Your real startup** (recommended if you're an operating
  founder): pull the actual numbers from your mod-003 model.
- **Simulated:** Your mod-003 model has these characteristics:
  - Current cash: $310k. Current gross burn: $42k/mo (revenue
    ~$0 for the purposes of the model).
  - Two engineers planned: one starts month 3, one starts month
    6, both at $180k base × 1.30 fully-loaded → ~$19.5k/mo each.
  - Non-payroll spend: ~$8k/mo (hosting, tools, contractors,
    legal, other).
  - No revenue in the plan window.
  - You want to raise a **seed** to reach a milestone 15 months
    from close: *"10 paying design partners at ≥ $3k ARPA."*

## Requirements

- **Compute `M`** — the total spend needed from month 0 (close)
  through the milestone month, minus any expected cash in during
  that window. Show the components (payroll, non-payroll, minus
  revenue).
- **Compute `B`** — the 6–9 month post-milestone runway buffer at
  the post-hire, post-milestone monthly burn rate.
- **Compute the raise** ≈ `M + B`. Round to a clean number.
- **Sanity-check post-close runway.** Raise / average monthly
  gross burn between close and milestone. Report the months. Must
  land in the 18–24 month band; if not, name which knob you'd
  turn (milestone timing, team plan, or shrink the round).
- **Sanity-check dilution.** State the raise. State three possible
  post-money valuations (a defensible low, mid, and high for your
  stage and evidence). Compute new-money dilution at each. Must
  land in 15–25%; if not, name why.
- **Write the milestone statement.** Testable outcome; not an
  activity; sized to open a Series A conversation (or, for a
  pre-seed, sized to open a seed conversation).
- **Write the one-line raise thesis** — a single sentence a
  partner would nod at.

## Starter guidance

**Session 1 (~30 min) — inputs.** Open the mod-003 model. Pull
these numbers into a scratch sheet:
- Current cash on hand.
- Current gross burn.
- Planned hires with start months and fully-loaded costs.
- Non-payroll spend by month (or a monthly average).
- Any revenue you're willing to defend to a partner.
- The milestone month you're targeting.

**Session 2 (~1 hr) — the arithmetic.** Compute `M`:

```
M = Σ(monthly gross burn, month 1 through milestone month)
   − Σ(monthly cash in, month 1 through milestone month)
```

Compute `B`:

```
B = post-milestone monthly gross burn × 6..9 months
```

Then:

```
raise ≈ M + B
```

Round to a clean number (typically to the nearest $250k or $500k
at seed).

**Session 3 (~30 min) — the sanity checks.** Post-close runway:

```
post-close runway = raise / average monthly gross burn (month 1 → milestone)
```

Must be 18–24 months. If less, either the buffer `B` is too small
or the milestone is too far out. If more, either the milestone is
too near-term or the raise is bigger than the story justifies.

Dilution:

```
new-money dilution ≈ raise / post-money valuation
post-money = pre-money + raise
```

Try three post-money valuations you'd defend as plausible for
your evidence: a low, a mid, and a high. Compute dilution at each.
Must land in 15–25% at a defensible price.

**Session 4 (~30 min) — milestone and thesis.** Write the
milestone as a single sentence with a **number** in it (ARR, ACV,
customer count, retention percentage, etc.). Then write the
one-line raise thesis:

```
We're raising $X at $Y post-money to buy Z months of runway to
reach [testable milestone] by [date].
```

Read it out loud. If you can't say it in one breath and defend
each clause without a spreadsheet, tighten it.

## Templates (fill inline)

```
INPUTS (from mod-003 model)
  Current cash                           : $______
  Current monthly gross burn             : $______
  Planned hires:
    Hire 1 — role, start month, fully-loaded $/mo: _____________________
    Hire 2 — role, start month, fully-loaded $/mo: _____________________
    Hire 3 — role, start month, fully-loaded $/mo: _____________________
  Average non-payroll spend $/mo         : $______
  Expected revenue in plan window        : $______
  Target milestone month (from close)    : month ______  (date: ______)

ARITHMETIC
  M = spend (month 1 → milestone) − cash in (month 1 → milestone)
      Payroll total in window            : $______
      Non-payroll total in window        : $______
      Cash in (revenue) in window        : $______
      M                                  : $______

  Post-hire, post-milestone monthly gross burn: $______
  Buffer months (choose 6–9)             : ______
  B = post-milestone burn × buffer months: $______

  Raise ≈ M + B                          : $______
  Rounded raise (clean number)           : $______

SANITY CHECKS
  Average monthly gross burn (close → milestone): $______
  Post-close runway (raise / avg burn)   : ______ months   [target 18–24]
  Pass / fail                            : ______

  Post-money valuation scenarios:
    Low   : pre-money $____ + raise $____ = post-money $____ → dilution __%
    Mid   : pre-money $____ + raise $____ = post-money $____ → dilution __%
    High  : pre-money $____ + raise $____ = post-money $____ → dilution __%
  Which scenarios land in 15–25%?        : ______

MILESTONE STATEMENT
  "____________________________________________________________________
   ____________________________________________________________________
   by [date]."

ONE-LINE RAISE THESIS
  "We're raising $____ at $____ post-money to buy ____ months of runway
   to reach ______________________________________ by [date]."
```

## Acceptance criteria

You are done when *all* of the following are true:

- [ ] `M` is computed with components (payroll, non-payroll,
      minus revenue) shown.
- [ ] `B` is computed at the post-hire, post-milestone burn rate
      with a buffer of 6–9 months named.
- [ ] The raise is `M + B` rounded to a clean number.
- [ ] Post-close runway is computed and lands in **18–24 months**
      (or the knob to turn is named).
- [ ] Three post-money valuation scenarios are named and dilution
      is computed at each; at least one lands in **15–25%**.
- [ ] The milestone statement is a **single sentence with a
      number in it** and is testable in a diligence conversation.
- [ ] The one-line raise thesis can be said in one breath and
      defended without opening the sheet.

## Self-assessment rubric

<!-- needs-research: exemplar for mod-004 not yet authored; the rubric-vs-exemplar comparison assumes future exemplars/mod-004-fundraising-preseed-to-seed/. -->

| Dimension | Weak | Strong |
|---|---|---|
| Raise arithmetic | Number picked from vibes | Raise = M + B, each component shown from the mod-003 model |
| Milestone | Activity ("ship v1") | Testable outcome with a number, sized to the next round |
| Post-close runway | Not computed | Falls out of the arithmetic; lands in 18–24 months or names the fix |
| Dilution | Not considered | Three valuation scenarios; at least one lands in 15–25%; unrealistic scenarios flagged |
| Raise thesis | Multi-paragraph, spreadsheet-required | One sentence, defensible without a sheet |
| Consistency with model | Numbers disagree with mod-003 | Every input traceable to a named cell in the mod-003 model |

## Definition of done

A skeptical seed-stage partner, hearing your one-line raise
thesis and skimming your arithmetic, would agree that (a) the
raise size falls out of the operating model, (b) the milestone is
specific enough to underwrite, and (c) the dilution and
post-close runway are in defensible bands for a seed round.

> Solutions are not provided in this repository; they live in the
> paired solutions repo.
