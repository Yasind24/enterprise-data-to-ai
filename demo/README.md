# Public demonstration: what does “active customer” mean?

**Status:** Designed, not implemented. No live application or platform integration is available yet.

## The scenario

A fictional utility has electric and gas service points. Three reporting sources answer “How many active customers do we have?” differently:

| Fictional source | Definition | Result from seed data |
| --- | --- | --- |
| Dashboard A | Distinct accounts with at least one active service point | 3 accounts |
| Dashboard B | Active service points | 4 service points |
| Warehouse view C | Distinct accounts with an active service point, excluding test accounts | 2 accounts |

All three counts can be calculated from the data. They answer different questions. The demonstration should expose that distinction and help a user choose the intended business meaning.

## Intended visitor journey

1. Inspect the fictional sources and their definitions.
2. Compare grain, filtering, and scope.
3. Review a proposed metric definition and approve or revise it.
4. Inspect lineage from definition to source fields.
5. Ask a question and see the definition, evidence, and result.
6. Try an ambiguous or unsupported question and see clarification or an explicit limitation.

## Build boundaries

- Start with this single metric across electric and gas.
- Keep calculations deterministic and independently verifiable.
- Use AI to help interpret questions and compare logic; require review for business definitions.
- Label platform connectors as planned until they run against actual services.
- Distinguish simulated source artifacts from real Tableau, Power BI, or BigQuery exports.

## First implementation milestone

A locally runnable experience that loads the synthetic data, compares the three definitions, and shows reproducible counts. Add reviewed semantic definitions and conversational querying after that foundation works.

[Seed data](../data/README.md) · [Evaluation plan](../evaluation/README.md)
