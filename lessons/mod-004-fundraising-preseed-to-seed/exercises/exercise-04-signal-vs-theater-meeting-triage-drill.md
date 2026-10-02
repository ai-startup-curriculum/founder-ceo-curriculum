# Exercise 04 — Signal vs Theater Meeting Triage Drill

**Module:** 004 Fundraising: Pre-seed → Seed · **Stage:** PRE-SEED
→SEED · **Time:** ~90 focused minutes · **Reads with:** chapter
[07](../07-signal-vs-theater.md), with cross-references to
chapters [03](../03-investor-funnel-and-conversion.md) and
[04](../04-parallel-time-boxed-process.md).

## Problem statement

An investor pipeline that lies to the founder is worse than no
pipeline at all. A row marked "in progress" that is really a
polite pass gets follow-up time, inflates the implied term-sheet
count, and crowds out the one or two conversations that could
produce a real yes. The failure mode is boring: compliments get
dispositioned as commitment, radio silence gets dispositioned as
"they're busy," and the honest funnel underneath the tracker
quietly dies.

This exercise is the **weekly triage ritual** that keeps the
pipeline honest. You take a set of in-flight investor meeting
outcomes, apply the signal-vs-theater rules from chapter 07 to
each one, re-disposition every row, and recompute whether the
*honest* funnel still implies the round closes. Run it as a
standalone diagnostic any time you suspect your pipeline is
flattering you.

## Deliverables (three founder artifacts)

1. **A re-dispositioned pipeline table** — every in-flight row
   re-labeled as **ACTIVE / SOFT-NO / DEAD / AMBIGUOUS**, with
   the signal(s) or anti-signal(s) that justified the label.
2. **A next-action list** — exactly one next action per row
   (nudge, kill, log a quarterly update, press for next step),
   with the owner, the specific wording, and the date.
3. **An honest-funnel recount** — the implied term-sheet count
   computed from the *active* rows only, with the delta against
   the generous funnel named and the go / no-go call on the
   round stated.

## Scenario

Pick one:

- **Your real round** (recommended if you're mid-raise): open
  your current pipeline tracker and run the drill on your
  real in-flight rows. The exercise is designed to produce
  a decision — adjust process, pull more intros, or acknowledge
  the round is softer than you've been treating it.
- **Simulated:** use the fixture below. You are three weeks into
  a $3M seed raise. Your tracker has 24 "in progress" rows. The
  following 12 are the ones a weekly ritual would surface for
  triage. Each has a last-meeting type, the most recent
  investor-side communication, and the days since you last
  heard from them.

### Fixture: 12 in-flight pipeline rows

```
Row 01 — Fund A (A-tier, lead-capable)
  Last meeting: partner meeting, 11 days ago.
  Last comms: "Really impressive meeting; want to stay in touch."
  Days since any touch: 11. You've nudged once (day 7). No reply.

Row 02 — Fund B (A-tier, lead-capable)
  Last meeting: partner meeting, 4 days ago.
  Last comms (day 1): "Loved the depth on the cohort data. Can you
    get on a call Thursday with [second partner]? And send the
    customer contracts and raw retention CSVs."
  Days since any touch: 1.

Row 03 — Fund C (B-tier, follow)
  Last meeting: first meeting, 6 days ago.
  Last comms: "This is one of the most interesting decks I've seen
    this year. Really excited about the space."
  Days since any touch: 6. No concrete next step mentioned.

Row 04 — Fund D (A-tier, lead-capable)
  Last meeting: partner meeting, 9 days ago.
  Last comms (day 2): "We'd want to see $1M ARR before we lead."
    You're at $140k ARR; raising a seed.
  Days since any touch: 7.

Row 05 — Fund E (A-tier, lead-capable)
  Last meeting: partner meeting, 3 days ago.
  Last comms (day 0): "I'll come back to you Friday with next
    steps." Today is Friday mid-afternoon. Nothing yet.
  Days since any touch: 3.

Row 06 — Fund F (B-tier, follow)
  Last meeting: first meeting, 14 days ago.
  Last comms: "Keep us posted as you make progress."
  Days since any touch: 14. You nudged on day 7. No reply.

Row 07 — Fund G (A-tier, follow)
  Last meeting: partner meeting, 8 days ago.
  Last comms (day 3): "Reference call with [portfolio founder]
    scheduled next Tuesday. Also — if we were to come in behind a
    lead, what size allocation would you want for us?"
  Days since any touch: 5.

Row 08 — Fund H (B-tier, non-lead)
  Last meeting: first meeting, 10 days ago.
  Last comms: "We'd need to see a lead first." (This fund does not
    lead rounds and has never led a round at your stage.)
  Days since any touch: 10. No reply to your nudge on day 6.

Row 09 — Fund I (A-tier, lead-capable)
  Last meeting: first meeting, 2 days ago.
  Last comms (day 1, in writing): detailed questions on hiring plan
    assumptions, cohort retention methodology, and the fully-loaded
    cost on Engineer #2. Requested a 45-minute follow-up with the
    partner next week.
  Days since any touch: 1.

Row 10 — Fund J (C-tier, follow)
  Last meeting: first meeting, 5 days ago.
  Last comms: "We're not ready to move but come back in three
    months." No specific milestone named for the three-month ask.
  Days since any touch: 5.

Row 11 — Fund K (A-tier, lead-capable)
  Last meeting: first meeting, 20 days ago.
  Last comms: at the meeting, partner said "we'll come back to you
    next week." No reply since. You've nudged twice (day 8, day 14).
  Days since any touch: 20.

Row 12 — Fund L (B-tier, follow)
  Last meeting: first meeting, 5 days ago.
  Last comms (day 2): "We're not ready to move but come back in
    three months once you have signed design partners #4 and #5 —
    that would unlock a conversation on the next round."
  Days since any touch: 3.
```

The round math you're triaging against:

- Round size: **$3M seed** (from exercise 02 in this module).
- Honest-funnel threshold: **≥ 2 term sheets implied, including
  ≥ 1 from a credible lead**, from the active rows plus the
  rest of your in-progress pipeline (assume the untriaged 12
  active rows carry roughly 1.0 implied term sheet between them
  using the chapter 03 heuristics).
- Target close date: **4 weeks from today**.

## The disposition rules (apply row-by-row)

Use the rules from [chapter 07](../07-signal-vs-theater.md). For
each row, pick exactly one label and justify it in one line.

- **ACTIVE** — the fund has committed to a concrete next step
  (second meeting invited, reference call scheduled, data-room
  / specific-diligence request made, term-shaped conversation
  opened, intra-firm introduction to another partner, written
  follow-up questions in 24–48 hours, or an in-meeting cadence
  commitment met). ACTIVE rows stay in the funnel math.
- **SOFT-NO** — "keep us posted," "come back in three months"
  with no specific milestone named, "excited but need to see
  \[large, later-stage metric\]," effusive praise with no next
  action, or a "we'd need a lead first" from a fund that
  doesn't lead. SOFT-NO rows drop out of this round's funnel
  math; they can enter the quarterly-update list.
- **DEAD** — radio silence for more than one week after a
  partner meeting with the fund owing the next step, or a
  second-nudge-with-no-reply pattern. DEAD rows drop out of
  this round's funnel math and are not sent a nudge. (A
  closing-day "we closed, thanks" email per chapter 08 is the
  only remaining comms.)
- **AMBIGUOUS** — neither a concrete next step nor a time-boxed
  anti-signal has triggered yet, and the "when should I expect
  to hear back?" window has not yet elapsed. AMBIGUOUS rows
  stay out of the funnel math until the next weekly ritual
  resolves them.

The forcing rule from chapter 07: **words are theater; actions
are signal.** If the only evidence for ACTIVE is a compliment,
the row is not ACTIVE.

## Requirements

- **Every row has exactly one label.** No "ACTIVE but soft."
  No "could be either." If you cannot pick cleanly, label
  AMBIGUOUS and name the specific action that will resolve it
  within 7 days.
- **The justification is the signal, not the vibe.** For an
  ACTIVE row, name the concrete action the fund took. For a
  SOFT-NO or DEAD row, name the specific anti-signal (phrase +
  days since touch). "Felt engaged" is not a justification.
- **Each row has exactly one next action.** A nudge, a kill, a
  quarterly-update log, a scheduled follow-up, or an
  in-meeting question to ask next time. One owner, one date,
  one specific thing to send or say. No "follow up as needed."
- **At most one nudge per row.** A second nudge to a row that
  has already failed a nudge is not permitted. If you want to
  nudge again, you must either upgrade the warm path or move
  the row to DEAD.
- **Recompute the funnel on active rows only.** Apply the
  partner-meeting → term-sheet heuristic from
  [chapter 03](../03-investor-funnel-and-conversion.md)
  (~15–25%) to active partner-meeting rows and the full
  heuristic chain to active first-meeting rows. Add in the ~1.0
  implied term sheet from the untriaged pipeline (fixture
  only). Compare to the pre-triage count.
- **State the call on the round.** Does the honest funnel
  implied term-sheet count still meet the threshold (≥ 2
  including ≥ 1 lead)? If not, name the cheapest fix — pull
  more A-tier warm intros, extend the close window, or
  consciously size the round down.

## Starter guidance

**Session 1 (~30 min) — the disposition pass.** Walk the 12
rows in order. For each, look only at the facts given (last
meeting type, exact wording, days since touch). Resist
reinterpreting the exact wording charitably. Write the label
and the one-line justification in the template below.

Watch for the trap patterns from the chapter:

- "Really impressive / really excited" with no next action = SOFT-NO.
- "Keep us posted" with no specific milestone = SOFT-NO.
- "Come back in three months" with no named deliverable = SOFT-NO;
  "come back in three months once you have X" with X named = ACTIVE
  for the *next* round (log quarterly-update list), SOFT-NO for
  *this* round.
- Partner-meeting + >7 days + fund owes next step + nudged = DEAD.
- "Need to see \[Series A metric\]" at seed = SOFT-NO at this
  round (do not run your process around them).
- A promise met on the committed date (even if the content is
  "need more time") = ACTIVE if a new next step is set, otherwise
  AMBIGUOUS until the fund commits.
- A promise *missed* without a new concrete commitment = move
  toward SOFT-NO.

**Session 2 (~20 min) — the next-action list.** For each row,
write exactly one next action. For ACTIVE rows, the next action
is already named by the fund (confirm it on the calendar); your
job is to log the owner and the date. For SOFT-NO rows, the
action is either (a) add to quarterly-update list and close the
loop at round-close per chapter 08, or (b) if a specific
deliverable was named, note it as a *next-round* warm intro.
For DEAD rows, the action is "no action; include in closing-day
email." For AMBIGUOUS rows, the action is the specific question
or nudge that will resolve the row within 7 days.

**Session 3 (~25 min) — the funnel recount.** Count the ACTIVE
rows by meeting stage reached (first meeting vs partner
meeting). Apply the chapter-03 downstream heuristics:

```
first-meeting → partner-meeting   ~20–35%
partner-meeting → term sheet      ~15–25%
```

Compute the implied term-sheet contribution from the triaged 12
and add the fixture's ~1.0 implied term sheet from the
untriaged in-progress rows. Compare to the pre-triage count
(assume the pre-triage count would have treated every row as
"in progress" at the partner-meeting → term-sheet heuristic for
rows that reached a partner meeting, and at the first → partner
→ term-sheet heuristic for rows that didn't).

**Session 4 (~15 min) — the call on the round.** State the
honest implied term-sheet count. State whether it meets the
threshold. If yes, name what you'll keep doing. If no, name the
single highest-leverage fix (not three; one).

## Templates (fill inline)

```
DISPOSITION PASS (12 rows)
  | Row | Fund | Last meeting | Days since touch | Signal / anti-signal | Label | Justification |
  |-----|------|---------------|-------------------|-----------------------|-------|---------------|
  | 01  | A    |               |                   |                       |       |               |
  | 02  | B    |               |                   |                       |       |               |
  | ... |      |               |                   |                       |       |               |
  | 12  | L    |               |                   |                       |       |               |

LABEL COUNTS
  ACTIVE   : ___      (list rows: ___)
  SOFT-NO  : ___      (list rows: ___)
  DEAD     : ___      (list rows: ___)
  AMBIGUOUS: ___      (list rows: ___)

NEXT-ACTION LIST (one per row)
  | Row | Action (nudge / kill / log Q-update / confirm / ask Q) | Specific wording or next step | Owner | By (date) |
  |-----|---------------------------------------------------------|-------------------------------|-------|-----------|
  | 01  |                                                         |                               |       |           |
  | ... |                                                         |                               |       |           |

HONEST-FUNNEL RECOUNT
  ACTIVE rows reaching partner meeting      : ___
  ACTIVE rows at first-meeting stage        : ___
  AMBIGUOUS rows (not counted this week)    : ___

  Chapter-03 heuristics applied:
    first → partner × partner → term sheet  : ___% × ___% = ___%
    partner → term sheet                    : ___%

  Implied term sheets from the 12 triaged rows:
    partner-meeting rows: ___ × ___% = ___
    first-meeting rows : ___ × ___% × ___% = ___
    subtotal           : ___

  Untriaged pipeline contribution (fixture)  : ~1.0
  Total honest implied term sheets           : ___
  Pre-triage implied term sheets (generous)  : ___
  Delta                                       : ___

CALL ON THE ROUND
  Honest implied term sheets ≥ 2?               YES / NO
  Includes ≥ 1 credible lead?                   YES / NO
  Round meets honest threshold?                 YES / NO

  If NO, the single highest-leverage fix:
    [ ] pull more A-tier warm intros (name whose intros, by when)
    [ ] extend the close window by ___ weeks and name why that produces a yes
    [ ] consciously size the round down to $___ with milestone impact ___
    [ ] other: ___

CLOSING-DAY EMAIL LIST (per chapter 08)
  Rows receiving the "we closed" email: all SOFT-NO + DEAD rows (list): ___
```

## Acceptance criteria

You are done when *all* of the following are true:

- [ ] Every one of the 12 rows (or your real in-flight rows) has
      **exactly one** label (ACTIVE / SOFT-NO / DEAD / AMBIGUOUS).
- [ ] Every row's justification names the **specific signal or
      anti-signal** (phrase, action, or days-since-touch), not a
      vibe.
- [ ] Every row has **exactly one next action** with an owner
      and a date.
- [ ] No row has more than one nudge logged against it; a row
      that has already received a nudge-with-no-reply is DEAD
      (or has had its warm path upgraded).
- [ ] The honest implied term-sheet count is computed from
      **ACTIVE rows only** plus the untriaged pipeline
      contribution, with the chapter-03 heuristics stated.
- [ ] The pre-triage vs post-triage delta is named.
- [ ] A clear go / no-go call on the round is stated, with the
      single highest-leverage fix named if the honest funnel
      doesn't clear the threshold.

## Self-assessment rubric

<!-- needs-research: exemplar for mod-004 not yet authored; the rubric-vs-exemplar comparison assumes future exemplars/mod-004-fundraising-preseed-to-seed/. -->

| Dimension | Weak | Strong |
|---|---|---|
| Signal honesty | Compliments dispositioned as commitment | Only concrete fund-side actions count as ACTIVE |
| Anti-signal discipline | Radio silence read as "they're busy" | > 1 week + nudged + fund owes next step = DEAD |
| Label cleanliness | "ACTIVE-ish," "SOFT-ACTIVE" | Exactly one label per row |
| Next-action specificity | "Follow up" | One action, one owner, one date, specific wording |
| Nudge discipline | Three or four follow-ups per silent partner | At most one nudge; next step is kill or warm-path upgrade |
| Funnel recount | Pre-triage math reused | Honest math from ACTIVE rows only, delta named |
| Round call | "We'll see how it plays out" | Explicit go / no-go with single highest-leverage fix |
| Closing-loop | SOFT-NO rows forgotten | SOFT-NO + DEAD rows on the closing-day email list |

## Definition of done

A skeptical peer founder — one who has run a seed round recently
and knows what "keep us posted" means — would read your
re-dispositioned pipeline and agree that (a) every ACTIVE label
is backed by a concrete fund-side action, (b) every SOFT-NO /
DEAD label is backed by a specific anti-signal, (c) the
next-action list is executable this week, and (d) the honest
funnel recount is the number you should be running the round
against — not the generous one you had before.

> Solutions are not provided in this repository; they live in the
> paired solutions repo.
