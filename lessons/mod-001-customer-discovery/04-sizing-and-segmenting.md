# Chapter 04 — Sizing and Segmenting: ~15–20 Interviews in a Recognisable Segment

> **Reads with:** module objective 4 — *size and segment the discovery target
> narrowly enough to produce signal — ~15-20 interviews in a recognisable
> segment rather than 'founders' or 'SMBs'.*

## The two knobs that decide whether discovery produces signal

A discovery sprint has, in practice, exactly two design decisions before
the interviews start:

1. **How narrow the segment is.**
2. **How many people from that segment you talk to.**

Get either wrong and the sprint returns noise. Get both right and even a
poorly worded interview guide (see chapter 02) will surface real patterns.

## Segment: narrow enough that you can name three real people

The single most consequential move in a discovery sprint is defining the
segment narrowly. "Founders" is not a segment. "SMBs" is not a segment.
"Marketers" is not a segment. Each of those names a *population*, and the
population is so heterogeneous that any pattern you observe averages across
irreconcilably different buyers, in different situations, with different
budgets, hearing about the same problem in different words.

A **recognisable segment** has three properties:

- **Externally observable.** You can tell from someone's LinkedIn, from a
  public signal (a recent raise, a hiring post, a conference talk), or
  from a short screening question whether they are in the segment.
- **Actionable.** You can list the channels — communities, warm intros,
  filters — through which you'd reliably reach members of it.
- **Homogeneous on the axis that matters.** The buyers inside the segment
  share the *specific situation* that produces the pain you're testing.

The pragmatic test: **can you name three real, specific people who fit the
segment definition, and would you be able to find twenty more?** If the
answer is no, the segment is either too vague ("founders") or so narrow it
doesn't exist as a population ("first-time solo technical founders in
Austin who raised in Q2 2026 from a specific fund").

The right shape is between those extremes:

- Bad: *"founders."*
- Bad: *"early-stage founders."*
- Getting there: *"first-time technical founders raising a pre-seed."*
- Right: *"first-time technical founders who incorporated and started
  raising a pre-seed in the last 12 months."*

The right version is a filter you could apply to LinkedIn and to a warm
intro request and get a manageable, coherent set of names back.

## Why narrow beats broad: the noise problem

Broad segments produce mush for a specific reason. Suppose "founders" is a
population of a million people, and 5% of some sub-segment has the acute
problem you care about; the other 95% either don't, or feel a different
version of it, or feel it at a different scale. An interview set of 15
people drawn from "founders" is expected to contain 0–2 members of the
segment that would show signal, and 13–15 people whose experience will
average against them. The pattern you'd have seen inside the narrow segment
disappears in the average.

Narrow the segment and the arithmetic reverses. Fifteen interviews inside
a segment where 60–80% of the population has the acute problem produces a
pattern strong enough to see with the naked eye — nine or ten people with
the same story, told with the same emotional colour, spending on the same
kinds of workarounds. That is the shape of usable signal.

The consequence for framing: **the goal of the segment definition is not
to capture your whole eventual market**. It is to isolate the tightest
group in which the pain is loud enough to be observable. You can widen the
segment later, once the shape of the problem is clear; you cannot recover
signal you lost by starting wide.

## Sample size: ~15–20, and why

The rule of thumb the sprint targets — **15–20 interviews in a single
narrow segment** — sits between two well-known findings:

- Below ~8–10 interviews, you're reacting to individual quirks: two loud
  people can look like a pattern.
- Around ~12 interviews in a homogeneous group, most dominant patterns have
  usually appeared at least once; new interviews after that mostly repeat
  what you've already heard. This is the "saturation" finding from
  qualitative research methods.
  <!-- needs-research: primary-source citation for the ~12-interview saturation heuristic — commonly cited from Guest, Bunce & Johnson, "How Many Interviews Are Enough? An Experiment with Data Saturation and Variability," *Field Methods* 18(1), 2006. -->

The 15–20 range gives you a small safety margin over 12 — enough that if
two interviews come back off-segment or unusable, you still have a
defensible pattern. Beyond 20 in the same segment, marginal returns fall
sharply; if you have appetite for more discovery, spend it on **a second,
adjacent segment** to test how the pattern generalises, not on the
twenty-first person in the first one.

If you can only run five interviews this week (a common real constraint),
the honest framing is: *you have a directional read, not a pattern.* Five
interviews can kill an idea (five uniform "we don't feel this pain") but
usually can't confirm one. Say so in the memo (chapter 05).

Two failure shapes worth naming:

- **Too broad, adequate sample.** Twenty "founders" — most patterns wash
  out. Add-a-second-tab, not a real filter.
- **Narrow enough, tiny sample.** Four "recently-raising technical
  founders" — the segment is right, the count doesn't get you saturation.
  Directional only.

Only *narrow segment + ~15–20 interviews* gives you a result you can bring
to a skeptical co-founder or investor and defend.

## Segmenting on the axis that matters

Two founders can pick the same nominal segment ("SaaS marketers at Series A
companies") and get different discovery results because they're implicitly
segmenting on different axes. The axis that matters is the one *most
correlated with whether the pain occurs*, not the one that's easiest to
describe.

Some axes that reliably matter more than the ones founders reach for first:

- **Recency of the triggering situation.** "Marketers at Series A companies
  who launched a new pricing page in the last three months" segments on the
  event that produces the pain, not the demographic.
- **Experience.** First-time vs. second-time in a role often predicts pain
  intensity more than industry does — the second-time person has already
  built the workaround.
- **Team shape.** Solo vs. two-person vs. small-team often predicts *how*
  the problem is felt; a solo founder eats a problem an eight-person
  company assigns to a specialist.
- **Buying authority.** A user who is not the buyer will describe the same
  problem differently — they'll skip the ROI framing that the actual
  purchaser needs. Segment on *who signs* when the sale eventually happens.

The exemplar segment in this module — *first-time technical founders who
incorporated and began raising in the last 12 months* — is built from three
of these axes at once (recency, experience, team-shape) precisely because
that combination is what predicts the "overwhelm" pain the exemplar is
testing.

## Recruit funnel arithmetic

The segment definition drives the recruit funnel. A workable rule of thumb:

- Assume 30–50% of segment-fit people you ask will schedule.
- Assume 60–80% of scheduled calls will actually happen.
- Assume 70–90% of completed calls will be usable interviews (some are
  off-segment on the actual call; some are unproductive).

At the pessimistic end that's roughly 30% × 60% × 70% ≈ **13% conversion
from ask to usable interview**. For 15 usable interviews, plan on 115
segment-fit asks in the funnel. That number sets your recruit channel plan
(see the exemplar's discovery plan in `exemplars/mod-001-customer-discovery/`).

Two channel notes:

- **Warm intros** convert best but scale worst; use them for the first
  four or five.
- **Cold outreach anchored to a public signal** ("saw you closed your
  pre-seed last month") outperforms cold outreach without one by a wide
  margin.

## The failure mode: quietly widening the segment mid-sprint

The most common way a well-defined segment turns into mush is quiet
widening. The founder can't fill the recruit list at the narrow definition,
so they take an interview with someone one step outside — "close enough."
Twelve interviews in, half the set no longer fits the original filter, and
the memo synthesises across a heterogeneous group. The signal is diluted
and the founder doesn't notice because each individual "close enough"
decision felt small.

The disciplined response is to **write down the segment as a filter you
apply per interview**, and to record segment-fit as a field in each
interview note (see chapter 02's capture template). At synthesis time,
you'll count patterns *inside* the segment and separately note what the
off-segment interviews suggested — usually as adjacent-segment hypotheses
to test in a future sprint.

## Summary

- Segment narrowly enough that you can name three real people and know how
  to reach twenty more. Broad names ("founders," "SMBs") are populations,
  not segments.
- Target **~15–20 interviews in a single narrow segment**; below ~10 you
  hear noise, and beyond ~20 in the same segment returns fall sharply.
- Segment on the axis most correlated with the pain — often recency,
  experience, or team shape — not the axis easiest to describe.
- The recruit funnel is roughly 7–10× the interview target end-to-end;
  plan channels accordingly.
- Widening the segment mid-sprint is the fastest way to lose the signal
  you designed the sprint to produce.

**Next:** how to synthesise a stack of interview notes into a memo a
skeptical co-founder or investor would accept —
[chapter 05](./05-insight-memo-synthesis.md).
