# Chapter 05 — From Successful Pilot to Enterprise Contract: Procurement, Security, DPA/BAA, MSA, and First ACV

> **Reads with:** module objective 5 — *path a successful pilot to
> an enterprise contract: procurement, security review, DPA / BAA,
> master service agreement, and the first annual contract value.*

## A successful pilot is the middle of the deal

A metric hit at pilot exit is not a signed contract. It is the
buyer's *permission to proceed* to the paper process — the
sequence of procurement, security review, data processing
agreements, and a master service agreement that turns a
successful pilot into an annual commitment with dollars on it.

That paper process is where seed-stage deals slip most
predictably. The founder who invested six weeks in a pilot
and then treated the contract phase as "just paperwork" is
the founder who watches the deal stall for another two to
four months while procurement, InfoSec, and legal work
through their queues in parallel with the champion losing
attention.

This chapter is the map of the paper process, in the order
the founder needs to walk it. The rule that governs the whole
thing: **the CEO negotiates and signs; counsel drafts and
reviews.** The founder cannot outsource the commercial
decisions (price, term, redlines to non-standard clauses),
and counsel cannot outsource the legal opinion (whether the
DPA meets your contractual obligations, whether the MSA
carve-outs are enforceable, what the auto-renew clause
actually says). Both are necessary.

## The paper process, end to end

For a mid-market or enterprise SaaS deal at seed stage, the
paper process runs through five parallel-but-sequenced tracks:

```
1. Commercial proposal / order form  (you send)
2. Security review                    (their InfoSec)
3. DPA / BAA                          (their + your legal)
4. MSA                                (their + your legal)
5. Procurement + signature            (their procurement + signer)
```

The tracks are not fully sequential — security review can run
in parallel with the commercial proposal, and the DPA can
often be negotiated alongside the MSA. But there is a
dependency: procurement will not release the signature slot
until the MSA, order form, and DPA are all done, and security
sign-off is usually a gating item that must clear before any
of them.

Calendar realism for a first enterprise deal:

- **Small mid-market (< 500 employees), no HIPAA/PHI,
  standard SaaS:** ~30–60 days from pilot end to signature.
- **Mid-market, standard security review, DPA required:**
  ~60–90 days.
- **Enterprise (5,000+ employees), full security review,
  DPA + BAA, MSA redline:** ~90–180 days.
- **Regulated (healthcare, financial services, government):**
  180+ days; may require compliance evidence you don't yet
  have (SOC 2, HITRUST, FedRAMP).
<!-- needs-research: procurement/security/legal cycle length by buyer size; commonly cited ranges in enterprise SaaS playbooks (Gartner, First Round, SaaStr) but vary widely by buyer, product category, and geography. -->

Founders who plan a "signature by end of month" from a pilot
that ended yesterday consistently miss. Planning to the
midpoint of the realistic range — and communicating the
realistic range to the buyer's champion upfront — sets the
right expectation on both sides.

## Track 1 — The commercial proposal and order form

The **commercial proposal** is the founder-authored document
that describes what the buyer gets, at what price, for what
term, sent within days of a successful pilot. The **order
form** is the shorter, legal document that will be attached
to the MSA at signature.

The commercial proposal (2–4 pages) covers:

- **Recap of the pilot outcome.** The success metric,
  baseline, target, and result. In the buyer's own words
  where possible.
- **What's included in the paid tier.** The product surface,
  the user count, the support tier, the SLAs, the
  integrations. Named explicitly, not "everything in our
  Enterprise plan."
- **Price.** The first annual contract value (ACV), stated
  as an annual number. Optional multi-year discount if you
  offer one.
- **Term.** 12 months is standard for a first deal. Multi-
  year is possible for a discount but adds risk if the
  product is still changing rapidly.
- **Onboarding plan.** Who does what in the first 30 days
  after signature. This is what the champion needs to sell
  internally alongside the commercial ask.
- **Success criteria for renewal.** The metric that will be
  measured through the first year to justify the renewal.

The **order form** is a 1-page document that lists: parties,
term start and end, price, payment schedule, user count, and
a reference to the MSA it attaches to. It is the document
that gets signed at the end alongside the MSA. Draft it
early so procurement can start reviewing.

## Track 2 — Security review

Security review is the buyer's information-security team
(InfoSec) reviewing your product's security posture before
allowing their organization to send you their data. It is a
gating item for most enterprise deals; procurement will not
progress a deal that hasn't cleared security.

Two common formats:

- **A vendor security questionnaire** the buyer sends you
  to fill out. Common frameworks include the CAIQ (Consensus
  Assessments Initiative Questionnaire, from the Cloud
  Security Alliance) and the SIG (Standardized Information
  Gathering questionnaire from Shared Assessments).
  <!-- needs-research: CAIQ — Cloud Security Alliance, https://cloudsecurityalliance.org/research/cloud-controls-matrix. SIG — Shared Assessments, https://sharedassessments.org/sig/. -->
- **A review of your existing compliance evidence.** SOC 2
  Type II is the most common ask; ISO 27001, HIPAA, and
  FedRAMP show up for specific verticals or buyer sizes.
  <!-- needs-research: SOC 2 — AICPA Trust Services Criteria, https://www.aicpa-cima.com/topic/audit-assurance/audit-and-assurance-greater-than-soc-2. -->

Practical rules for seed-stage founders:

- **Have a security page or short trust document ready
  before you enter your first pilot.** Even a 5-page
  document covering data handling, encryption, access
  control, subprocessors, and incident response answers
  60–70% of most questionnaires.
- **Do not lie or hedge in security questionnaires.** If
  you don't have SOC 2, say so, name your plan and timeline,
  and offer compensating controls. Getting caught in a
  security review misrepresentation kills the deal and
  poisons future ones.
- **Route non-standard questions to your CTO or security
  advisor.** Security questionnaires reference specific
  controls (NIST CSF categories, CIS benchmarks) that a
  non-technical founder should not answer alone.
- **A SOC 2 Type II audit typically takes ~6 months of
  observation plus ~2–3 months of audit** and costs
  $20k–$50k+ at seed stage. Plan for it before you need
  it — if security reviews are killing pilots, you are
  already late.
  <!-- needs-research: SOC 2 Type II typical cost and duration for seed-stage startups; commonly cited ranges from Vanta, Drata, and A-LIGN publications but vary widely. -->

## Track 3 — DPA and (when relevant) BAA

The **Data Processing Agreement (DPA)** is the contract
between you (the data processor) and the buyer (the data
controller) that governs how you handle personal data. It
became standard practice with the EU GDPR (Article 28) in
2018, and any deal involving EU or UK data subjects will
require one.
<!-- needs-research: GDPR Article 28 — Regulation (EU) 2016/679, official text at https://eur-lex.europa.eu/eli/reg/2016/679/oj. -->

Standard DPA terms cover:

- The subject matter, duration, nature, and purpose of
  the processing.
- The categories of data subjects and personal data.
- Your obligations as processor (security measures, sub-
  processors, breach notification, deletion at end of term).
- The buyer's rights as controller (audit, instruction).
- Cross-border transfer mechanisms (SCCs, adequacy
  decisions, TIA — transfer impact assessment).

The **Business Associate Agreement (BAA)** is the U.S.
healthcare analog, required by HIPAA between covered entities
(healthcare providers, health plans, healthcare
clearinghouses) and their business associates (vendors
handling Protected Health Information, PHI). A BAA is
required *before* PHI is shared; a pilot that touches PHI
without a BAA is a HIPAA violation.
<!-- needs-research: HIPAA BAA requirements — 45 CFR §164.502(e) and §164.504(e); U.S. Department of Health and Human Services, https://www.hhs.gov/hipaa/for-professionals/covered-entities/sample-business-associate-agreement-provisions/. -->

Practical rules:

- **Have a template DPA drafted by counsel** before you
  need it. Buyers will often send their own DPA as a
  redline against your template; having a template gives
  you a defensible starting position.
- **Do not sign a BAA for a product not designed to handle
  PHI.** A HIPAA violation from an unrelated data path is
  a serious problem. If you are not sure your product can
  meet HIPAA obligations, do not sign the BAA and be
  honest with the buyer about the timeline.
- **Cross-border transfer is a real issue post-Schrems II**
  (EU CJEU, 2020). If you serve EU customers from U.S.
  infrastructure, your DPA will need Standard Contractual
  Clauses (SCCs) and a documented transfer impact
  assessment. Counsel drafts; you sign.
  <!-- needs-research: Schrems II — Case C-311/18, EU CJEU decision (July 2020). European Commission SCCs, Implementing Decision (EU) 2021/914. -->

## Track 4 — MSA (Master Service Agreement)

The **MSA** is the umbrella contract that governs the
commercial relationship. Order forms attach to it; renewals
extend it; additional products under the same MSA don't
require a fresh master contract. The MSA is where the
lawyer-time gets spent in an enterprise deal.

Standard MSA sections:

- **Definitions.**
- **Services and license grants.**
- **Fees, payment, and taxes.**
- **Term and termination** (auto-renewal is a common
  founder-side ask; buyer often pushes back).
- **Warranties and disclaimers** (buyers push for uptime and
  performance warranties; you push for standard "as-is"
  language with a service level exception).
- **Limitation of liability** (typically capped at 12 months
  of fees, sometimes with carve-outs for gross negligence,
  IP infringement, or data breach).
- **Indemnification** (mutual is best; one-sided in the
  buyer's favor is a founder-side redline).
- **Confidentiality and IP.**
- **Data protection** (usually references the DPA).
- **General terms** (governing law, venue, notices).

**MSA negotiation is where founders lose or preserve
protection they will need for years.** Two examples of clauses
that matter:

- **Limitation of liability cap.** Buyer often asks for
  unlimited liability or a multiple of fees. Standard is
  1× annual fees. Anything higher is a real risk to a small
  company.
- **Indemnification scope.** Buyer often asks you to
  indemnify against IP infringement claims. Standard is
  yes, with carve-outs for the buyer's own modifications or
  combinations. Blanket indemnification is a founder-side
  redline.

The right pattern: **your counsel drafts the MSA once,
you use it as the starting document for every deal, buyers
redline against it, you negotiate the redlines against a
pre-agreed decision tree from counsel** ("we can accept X,
push back on Y, do not accept Z under any circumstances").
That decision tree is the counsel handoff artifact for the
contract phase — see the boundary chapter (chapter 08) for
how the founder/counsel split works.

Where counsel is unavailable to draft the original MSA:
NVCA does not publish an MSA template; the standard starting
points are Bonterms (a free open-source model MSA published
by a consortium of GC-led companies), Common Paper's cloud
services template, and the SaaS Term Sheet template
maintained by TechGC.
<!-- needs-research: Bonterms — https://bonterms.com/forms/. Common Paper — https://commonpaper.com/. TechGC SaaS Term Sheet — https://www.techgc.co/. -->

## Track 5 — Procurement and signature

Procurement is the buyer's function that owns supplier
onboarding, contract management, and the paper flow between
legal, InfoSec, and finance. Procurement's job is to reduce
supplier risk and standardize commercial terms — which means
they are, structurally, an obstacle to fast deal closure,
not because they are unhelpful but because their metrics
optimize for something different from yours.

Working with procurement effectively:

- **Get introduced early.** Ask the champion, at pilot exit
  or before, "who from procurement will be involved, and
  when should I introduce myself?" Deals introduced to
  procurement in the last week close slower than deals
  introduced in the first week of the paper process.
- **Complete the vendor onboarding forms on their portal
  before they ask.** Most large enterprises have vendor
  portals (SAP Ariba, Coupa, Oracle Procurement Cloud);
  filling in the vendor profile is a gating item that can
  add weeks if you leave it for the end.
- **Pre-negotiate the pricing structure with the champion,
  not procurement.** By the time it reaches procurement, the
  price should be one of two agreed-upon numbers (with and
  without a specific concession); procurement's job is to
  approve it, not renegotiate it.

The **signer** on the buyer's side is often not the champion
and often not the economic buyer — it may be a signatory
authorized for contracts of a specific size, typically a
VP-level or C-level. Confirm the signer, their signing
authority for the deal size, and their calendar availability
early. A signature that requires "the CFO to be back from
vacation" is a two-week slip you can avoid by asking in
advance.

## The first annual contract value

The **first annual contract value (ACV)** is the annualized
revenue the customer commits to in year one. For a first
enterprise deal at seed stage, ACVs typically land in one of
three bands:

- **$10k–$50k ACV.** Small-team pilot converts. Common for
  first-in-vertical mid-market deals. Usually paid annually
  in advance; may include multi-year discount options.
- **$50k–$250k ACV.** Named-department deployment. Typical
  first serious enterprise deal for a seed-stage B2B SaaS
  company. Almost always involves full paper process
  (MSA, DPA, SOC 2 evidence).
- **$250k+ ACV.** Rare at seed stage; usually indicates the
  buyer is running a strategic initiative that happened to
  land your pilot at the right time. High reward but also
  high paper-process cost; often takes 6+ months from
  pilot end to signature.
<!-- needs-research: seed-stage first-ACV bands are commonly cited industry ranges (SaaStr, First Round, Bessemer's State of the Cloud reports) but vary widely by product category and buyer segment. -->

The pricing conversation at first contract is not "what is
this worth"; it is "what have similar buyers agreed to pay,
and what did the pilot demonstrate the value is worth to
them specifically." The pilot's success metric — the
quantified change to the buyer's world — is the load-bearing
input to the ACV negotiation. A $50k ACV against a $500k/year
saved-time metric is easy to defend; a $50k ACV against no
quantified metric is a negotiation you're going to lose.

## What the founder personally owns in the contract phase

The founder personally, without delegation to counsel:

- Owns the **commercial terms**: price, term, discounts,
  concessions.
- Owns the **MSA redline decisions**: which clauses to hold,
  which to concede, which to escalate to counsel for a
  specific opinion.
- Owns the **relationship with the champion and economic
  buyer** through the entire paper process. Silence during
  contract phase is when champions lose interest.
- Owns the **calendar management** — the shortest plausible,
  realistic, and longest-tolerable dates for each step,
  communicated to both the buyer's champion and your own
  team.

Counsel, in parallel:

- Drafts the MSA, DPA, BAA, and order form templates.
- Reviews buyer redlines and delivers a written opinion:
  what is standard, what is aggressive, what is
  non-negotiable.
- Advises on specific clauses that touch legal exposure
  (indemnification, warranties, IP, data breach
  liability).
- Never negotiates directly with the buyer's business
  team; buyer counsel and your counsel talk on legal
  points only.

The founder-counsel split for contract paper mirrors the
counsel handoff from mod-005 chapter 09: **the CEO
authors the commercial artifact and the negotiating
position; counsel authors the legal opinion.** Chapter 08
of this module makes the boundary to counsel explicit.

## When the contract closes

A signed enterprise contract at seed stage is a milestone
worth naming carefully:

- **Bank the ACV in the mod-003 operating model** — this is
  now revenue on the forecast, at collection terms in the
  order form (typically annual-in-advance, sometimes
  quarterly).
- **Update the mod-002 unit economics with the actual
  price paid**, not the price on your website. This is
  the market's actual willingness to pay for what you
  built; it is one of the highest-signal inputs the
  business has ever had.
- **Debrief the deal in a written note** — what worked,
  what didn't, what the champion did that made it move,
  what killed weeks that we can compress next time. This
  note is the input to the repeatable playbook that
  chapter 07 uses as the transition signal.
- **Send a note to the passers** on deals that stalled or
  died during your paper process. The founder-led sales
  discipline includes not burning bridges; some of those
  passers become customers 6–12 months later.

## Summary

- A successful pilot is **permission to proceed** to the
  paper process, not a signed contract. The paper process is
  where most seed-stage deals slip.
- The **five parallel-but-sequenced tracks**: commercial
  proposal / order form, security review, DPA (and BAA when
  relevant), MSA, procurement + signature. Procurement will
  not release signature until all four preceding tracks are
  clear.
- **Calendar realism** matters: 30–60 days for small mid-
  market, 60–90 for standard mid-market, 90–180 for
  enterprise, 180+ for regulated. Planning to the midpoint
  and communicating it upfront sets expectations both ways.
- **Security review is a gating item**; have a short trust
  document ready before your first pilot, and plan the SOC 2
  path early if enterprise deals will need it.
- **The CEO negotiates and signs; counsel drafts and
  reviews.** The founder owns commercial terms and the
  redline decision tree; counsel owns the legal opinion.
- The **first ACV is anchored by the pilot's success
  metric** — a quantified change in the buyer's world is
  what supports the price. Update the mod-002 economics
  with the actual price paid.

**Next:** the learning that only shows up when the founder
sells personally — the actual objections, the actual buyer,
the actual price — and how to feed it back into mod-001
discovery and mod-002 pricing — in
[chapter 06](./06-learning-only-founders-extract.md).
