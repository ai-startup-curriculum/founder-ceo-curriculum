# Founder / CEO Curriculum — Module Spine

Stage-tagged, dependency-linked. Tags follow the canonical
[stage](https://github.com/ai-startup-curriculum/startup-foundations/blob/main/STARTUP_STAGES.md)
and [pillar](https://github.com/ai-startup-curriculum/startup-foundations/blob/main/FUNCTIONAL_CURRICULA.md)
taxonomies in `startup-foundations`.

## Modules

| Module | Stage | Pillar | Founder artifact you produce |
|---|---|---|---|
| [mod-001-customer-discovery](./lessons/mod-001-customer-discovery) | IDEA | product / discovery | A 20-interview discovery plan + a synthesis/insight memo |
| [mod-002-lean-business-modeling](./lessons/mod-002-lean-business-modeling) | IDEA→PRE-SEED | strategy / economics | A lean canvas + a unit-economics sheet |
| [mod-003-runway-and-financial-modeling](./lessons/mod-003-runway-and-financial-modeling) | SEED | finance | An 18-month operating plan / runway model |
| [mod-004-fundraising-preseed-to-seed](./lessons/mod-004-fundraising-preseed-to-seed) | PRE-SEED→SEED | fundraising | An investor funnel from 200 targets with conversion assumptions |
| [mod-005-equity-safes-cap-tables](./lessons/mod-005-equity-safes-cap-tables) | PRE-SEED→SEED | equity | A cap table: founders + option pool + SAFE + priced seed |
| [mod-006-founder-led-sales](./lessons/mod-006-founder-led-sales) | SEED | GTM / sales | A discovery→qualification→pilot→contract sales script |

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
autonomous research→author pipeline fills them oldest-gap-first, and the CTO
pathway is authored here until it graduates to its own repo.

---

<!-- aicg:maintained-by -->
Maintained by [VeriSwarm.ai](https://veriswarm.ai)
