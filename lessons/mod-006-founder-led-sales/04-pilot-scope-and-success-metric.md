# Chapter 04 — Pilot Design: Scope, Success Metric, Duration, Contract

> **Reads with:** module objective 4 — *design a pilot with a
> scoped success metric, a fixed duration (typically 4–8 weeks),
> and a written contract — knowing that a pilot without a
> success metric is a free consulting engagement.*

## What the pilot is for

A pilot exists to answer **one question**: *does this
customer's world change measurably when they use our product?*

That question has a yes-or-no answer. If yes, the pilot ends
with a commercial conversation on a named calendar. If no,
the pilot ends with clean debrief data — what didn't move,
why, and what we learned about the product or the segment —
and both sides walk away without a hangover.

Everything about the design of the pilot flows from that
single-question framing. Scope is narrow because the question
is narrow. The success metric is pre-agreed because "did the
world change" is not a matter of opinion. The duration is
short because a pilot that goes on indefinitely has already
answered the question by not answering it. The contract is
written because unwritten pilots slide into free consulting
engagements the founder cannot exit.

## The failure mode: pilot as free consulting

The single most expensive pilot mistake is to run a pilot
with no pre-agreed success metric and no contract. It fails
in a specific, predictable pattern:

1. Founder is excited to land a big-logo pilot.
2. "Pilot" means "we set the product up and their team uses
   it for a while."
3. Six weeks in, their team is using it lightly. Champion
   says nice things.
4. Founder asks about next steps. Champion says "let me
   check with procurement."
5. Silence for four weeks.
6. Champion returns. "We loved it, but priority X came up
   and we're not going to move on this until next fiscal."
7. Founder has spent 10 weeks of engineering time on a
   customer that never had to say yes or no.

The mechanism of the failure: without a pre-agreed metric,
there is no forcing function that requires the buyer to
convert; without a written contract, there is no legal
document with a duration that ends by itself. The pilot
becomes a free consulting engagement that only the buyer's
budget cycle can end.

The fix is not "chase harder." The fix is structural: build
the metric and the end date into the pilot before it starts.

## The four fields every pilot needs

Every pilot the founder signs has four fields, minimum:

```
Scope           — What we will do; what we will not do
Success metric  — Pre-agreed, quantitative, owned by their side
Duration        — 4-8 weeks, calendar-fixed, with an end date
Price           — Paid, free-with-teeth, or (rarely) free
```

Add three fields that make the pilot end cleanly:

```
Exit criteria   — What happens on success, partial, and miss
Signers         — Who signs the pilot agreement on both sides
Attribution     — Whose data, whose measurement, whose report
```

The rest of the chapter walks through each field.

## Scope: one workflow, one team, one metric

The scope for a first pilot is deliberately narrow. Three
constraints:

- **One workflow.** Not "the product." Not "our platform."
  One specific workflow the buyer's team does today that
  will be replaced or augmented.
- **One team.** Not "the department." Not "the company." One
  named team with a named lead and a named set of users
  (~5–20 people for a typical B2B SaaS pilot).
- **One metric.** See the next section; this is the load-
  bearing constraint. Multi-metric pilots become debates about
  which metric mattered; single-metric pilots have an answer.

Anything that would fall outside those constraints is either
out-of-scope (list it explicitly in the pilot document) or a
reason to redesign the pilot around a different workflow.

Scope discipline lets the pilot answer its question in 4–8
weeks. Wide scope makes the pilot answer nothing in 6 months.

**Explicitly list out-of-scope items** in the pilot document:

```
In scope:
  - [workflow] for [team] with [named users]
  - Integration with [system A]
  - Weekly measurement of [success metric]

Out of scope:
  - Adjacent workflow [W2]  (would need separate pilot)
  - Additional teams beyond [team]
  - Custom features not on the current roadmap
  - Migration of historical data older than [date]
  - SSO / SCIM / [enterprise feature] until commercial deal
```

Listing out-of-scope explicitly does two things: it protects
your engineering calendar from scope creep during the pilot,
and it signals to the buyer that "not now, in exchange" — the
enterprise features are on the other side of a signed
contract, not this pilot.

## Success metric: pre-agreed, quantitative, owned by their side

The success metric is the load-bearing element of the pilot
design. A metric that is not pre-agreed, quantitative, and
owned by their side is not a metric — it is a hope.

**Pre-agreed.** Written into the pilot document, signed by
both sides, before the pilot starts. Not "we'll figure out
what success looks like as we go." Once the pilot has started,
the buyer has no incentive to agree to a metric that might
fail; they will always prefer "let's see how it goes."

**Quantitative.** A number, not an adjective. "Reduce
time-to-resolution from 4.2 hours baseline to under 2 hours"
is quantitative. "Improve support efficiency" is not.
Adjectives are debatable at pilot exit; numbers are not.

**Owned by their side.** Their data, measured on their
systems, reported by a named person on their team. If you
own the measurement, you own the debate at pilot exit. If
they own it, the number is unambiguous.

A working success-metric template:

```
Metric:              [specific number, e.g., P1-ticket TTR]
Baseline:            [measured before pilot start]
Target:              [pilot passes if reached, e.g., <2 hrs]
Measurement method:  [their systems / their instrumentation]
Reporter:            [named person on their team]
Cadence:             [weekly / mid-pilot / end-of-pilot]
```

Baseline before target. If you cannot measure the baseline
before starting, the pilot cannot pass. The first week of
the pilot is often "instrument the baseline, then start the
intervention" — and if the buyer resists instrumenting their
own baseline, the metric is not actually a shared priority.

**Choosing the right metric type.** Most successful B2B
pilots pick a metric in one of four families:

- **Time saved on a task.** Time-to-resolution, cycle time,
  time-to-decision.
- **Error rate reduction.** Defects, misroutes, rework,
  incidents.
- **Volume that shifted.** Tickets deflected, calls avoided,
  meetings replaced.
- **Adoption threshold.** N% of named users active weekly by
  end of pilot (usually as a secondary, not primary, metric).

Revenue-linked metrics (bookings driven, retention lifted)
are usually too slow to move inside 4–8 weeks and are best
kept out of the primary metric. If they matter, name them as
secondary and let the primary carry the pass/fail.

## Duration: 4–8 weeks, calendar-fixed

Enterprise B2B pilots typically run 4–8 weeks. Shorter is
often too short for the metric to move; longer is often
long enough for the buyer's priorities to drift.
<!-- needs-research: 4-8 week B2B pilot duration is a commonly cited industry heuristic (e.g., in enterprise SaaS playbooks from SaaStr, First Round Review, Winning by Design) but has no single canonical primary-source study. -->

The duration must be **calendar-fixed** — a start date and
an end date, both written into the agreement, both known to
the champion and the economic buyer. The end date is what
forces the commercial conversation to happen; without it, the
pilot has no natural end.

Two duration mistakes to avoid:

- **Duration-by-usage** ("the pilot runs until they've done
  X actions"). Buyers can slow-walk usage forever; the pilot
  never ends.
- **Extending automatically** ("we'll just push the end date
  a couple weeks"). Once the end date can move, all end
  dates move. Extension should require a written amendment,
  not a Slack message.

If the champion asks to extend, treat it as a signal. Either
the metric is close (and a 2-week extension with a written
amendment makes sense) or the pilot answered its question by
not answering it (and the extension is a soft-no).

## Price: paid, free-with-teeth, or (rarely) free

Three pricing options for a pilot, in decreasing order of
signal:

- **Paid pilot.** Best. A pilot invoice, even a small one,
  gets procurement and legal touching the deal early, which
  moves the paper process forward before the pilot ends. It
  also filters buyers who are not serious enough to open a
  PO. Typical paid-pilot amount: $5k–$25k for a 4–8 week
  enterprise pilot, sized to be small enough that
  procurement doesn't need multiple sign-offs but large
  enough to be real.
- **Free-with-teeth.** A signed pilot agreement, a named
  economic buyer, and pre-agreed conversion criteria. Free
  in dollars, but with the same commitment shape as a paid
  pilot: end date, metric, named signers on both sides.
  Appropriate when the buyer's procurement cycle would
  swamp a small pilot invoice.
- **Free.** No agreement, no named criteria. **Do not run
  these.** They are the free consulting engagement failure
  mode. If a prospect will not sign even a free-with-teeth
  agreement, they are not qualified.

The signal from asking for money — even a small amount — is
worth more than the money itself. A buyer who agrees to a
$10k pilot invoice has, by that act, put your deal on a
procurement track and named an economic buyer. A buyer who
refuses that same $10k invoice was probably going to stall
at contract anyway; better to know now.

## Exit criteria: three named outcomes

Every pilot has three possible outcomes, and each one needs
a pre-agreed next step:

```
If success metric hit:      → commercial proposal within [N] days
                              (typical N = 5-15)
If success metric partial:  → decision rule: extend, kill, re-scope
                              (name the specific rule)
If success metric missed:   → clean end; both sides walk away;
                              we owe them a debrief document
                              summarizing what we learned
```

Naming all three outcomes in the pilot agreement does two
things: it prevents the "let's just see how it goes"
extension trap, and it signals to the buyer that you are
willing to walk away if the metric doesn't move — which is
counter-intuitively a signal that the metric is real.

## Signers: the champion is not enough

The pilot agreement is signed on both sides by someone with
authority. On your side, it is the founder. On their side,
it should be at least the champion's manager — ideally the
economic buyer.

The reason: a pilot signed by the champion alone can be
killed at contract by the champion's manager or by
procurement, who will ask "who authorized this pilot?" and
find no one senior enough. A pilot signed by the economic
buyer has already crossed that threshold once. The path from
"successful pilot" to "signed contract" is much shorter when
the same person signs both.

Practical rule: if the champion cannot get their manager to
sign the pilot agreement, that is a qualification signal —
the champion may not have the internal weight to close the
eventual contract either. Better to know at pilot signature
than at contract stage.

## The written pilot agreement

The pilot agreement does not need to be a 40-page MSA. A
2-page pilot agreement or "letter of engagement" is enough,
covering:

- **Parties and dates.** Your legal entity, theirs; pilot
  start and end dates.
- **Scope.** The in-scope and out-of-scope lists from above.
- **Success metric and measurement.** The metric template
  from above.
- **Fees.** Paid amount if paid; "no fee" if free-with-teeth.
- **IP and data.** Their data stays theirs; your product IP
  stays yours; pilot-specific outputs (custom reports,
  integrations) named explicitly.
- **Confidentiality.** Standard mutual NDA, if not already
  signed.
- **Exit and conversion.** The three exit outcomes from
  above.
- **Signers.** Names, titles, and dates.

The 2-page pilot agreement is usually pre-drafted by counsel
so the founder can customize the scope and metric fields per
deal without a fresh legal review each time. Chapter 05
covers the counsel handoff for pilot and contract paper.

## What the pilot is not

- **The pilot is not a POC ("proof of concept").** A POC
  proves the product technically works. A pilot proves the
  buyer's world changes. Technical POCs happen inside a
  pilot, but they are not the pilot's success criterion.
- **The pilot is not a discount opportunity.** "Pilot pricing"
  that quietly becomes the permanent contract pricing is a
  common mistake; the pilot fee and the contract ACV are
  separate quantities, and the pilot fee is not a signal
  about the eventual ACV.
- **The pilot is not "the customer trying you out."** That
  framing puts you in the seller-of-something-optional
  position, which is exactly the position that fails to
  close. The framing that closes: *we are running a joint
  experiment on a shared hypothesis*, with a written
  protocol and a pre-agreed pass/fail.

## Summary

- A pilot exists to answer **one question**: does the
  customer's world change measurably? Yes → commercial
  conversation. No → clean debrief. No third answer.
- **Four required fields**: scope (one workflow, one team,
  one metric), success metric (pre-agreed, quantitative,
  owned by their side), duration (4–8 weeks, calendar-fixed),
  price (paid best, free-with-teeth second, free never).
- **Three required additional fields** to make the pilot end
  cleanly: exit criteria (success / partial / miss), signers
  (economic buyer, not just champion), attribution (their
  data, their measurement, their reporter).
- **A written pilot agreement** of ~2 pages, pre-drafted by
  counsel, customized per deal for scope and metric. Free
  pilots without agreements are the free-consulting failure
  mode; do not run them.
- The pilot is a **joint experiment on a shared hypothesis**,
  not a trial run of the product. That framing is what
  closes; "try us out" is what stalls.

**Next:** the path from a successful pilot to a signed
enterprise contract — procurement, security review, DPA/BAA,
MSA, and the first annual contract value — in
[chapter 05](./05-pilot-to-enterprise-contract.md).
