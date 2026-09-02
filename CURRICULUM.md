# Founder / CEO Curriculum — Module Spine

**Level:** 20 (Startup Leadership family) · **Total scope:** 226h (96h modules
+ 130h projects). Canonical plan: [`.aicg/curriculum-plan.json`](./.aicg/curriculum-plan.json).

Stage-tagged, dependency-linked. Tags follow the canonical
[stage](https://github.com/ai-startup-curriculum/startup-foundations/blob/main/STARTUP_STAGES.md)
and [pillar](https://github.com/ai-startup-curriculum/startup-foundations/blob/main/FUNCTIONAL_CURRICULA.md)
taxonomies in `startup-foundations`.

## Ownership rule

Assign primary coverage to the lowest-level role that genuinely requires the
skill. Higher-level tracks link to that owner rather than duplicating the
fundamentals; depth, architectural context, and leadership framing are what
higher levels add. See [`.aicg/curriculum-plan.json`](./.aicg/curriculum-plan.json)
`ownership_rule` for the full boundary map to peer and higher-level tracks.

## Modules

| Module | Hours | Stage | Pillar | Founder artifact you produce |
|---|---:|---|---|---|
| [mod-001-customer-discovery](./lessons/mod-001-customer-discovery) | 14 | IDEA | product / discovery | A 20-interview discovery plan + a synthesis/insight memo |
| [mod-002-lean-business-modeling](./lessons/mod-002-lean-business-modeling) | 16 | IDEA→PRE-SEED | strategy / economics | A lean canvas + a unit-economics sheet |
| [mod-003-runway-and-financial-modeling](./lessons/mod-003-runway-and-financial-modeling) | 18 | SEED | finance | An 18-month operating plan / runway model |
| [mod-004-fundraising-preseed-to-seed](./lessons/mod-004-fundraising-preseed-to-seed) | 20 | PRE-SEED→SEED | fundraising | An investor funnel from 200 targets with conversion assumptions |
| [mod-005-equity-safes-cap-tables](./lessons/mod-005-equity-safes-cap-tables) | 16 | PRE-SEED→SEED | equity | A cap table: founders + option pool + SAFE + priced seed |
| [mod-006-founder-led-sales](./lessons/mod-006-founder-led-sales) | 12 | SEED | GTM / sales | A discovery→qualification→pilot→contract sales script |

## Projects

| Project | Hours | Integrates | Deliverable |
|---|---:|---|---|
| [project-101 Founder Package: Idea → Fundable Plan](./projects) | 45 | mod-001, 002, 003 | Discovery memo + lean canvas + unit-economics sheet + 18-month operating model |
| [project-102 Round Package: Investor Funnel → Priced Seed Cap Table](./projects) | 45 | mod-003, 004, 005 | Investor funnel + pitch deck + cap-table walk + term-sheet redline |
| [project-103 Wedge → First Paying Customer: Founder-led Sales End-to-End](./projects) | 40 | mod-001, 002, 006 | Discovery call script + qualification rubric + pilot agreement + procurement response + learning-log |

## Dependency order

```
foundations (all of startup-foundations)
   └─► mod-001 Customer Discovery
          └─► mod-002 Lean Business Modeling
                 ├─► mod-003 Runway & Financial Modeling
                 │       └─► mod-004 Fundraising (needs a model to raise against)
                 │              └─► mod-005 Equity, SAFEs & Cap Tables
                 └─► mod-006 Founder-led Sales
```

## Status

`mod-001` is authored end-to-end (lesson + exercise + worked exemplar) as the
seed. `mod-002`–`mod-006` are stubbed with objectives + the target artifact; the
autonomous research→author pipeline fills them oldest-gap-first. The CTO and CPO
pathways now live in their own repos ([cto-curriculum](https://github.com/ai-startup-curriculum/cto-curriculum),
[cpo-curriculum](https://github.com/ai-startup-curriculum/cpo-curriculum)); this
repo is the Founder/CEO pathway.

---

<!-- aicg:maintained-by -->
Maintained by [VeriSwarm.ai](https://veriswarm.ai)
