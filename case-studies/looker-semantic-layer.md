# From scattered business logic to a Looker semantic layer

**Status:** Current engagement; in progress. This narrative distinguishes ongoing work from intended integration.

## The business problem

Business meaning is distributed across Tableau and Power BI dashboards and BigQuery views. Questions about enterprise data depend on understanding that logic, rather than interpreting field names alone.

## My current work

I lead a cross-functional team building a semantic layer in Looker over BigQuery for four domain groups: electric; gas; customer and corporate functions; and supply chain and cybersecurity. The work began as a vendor build, and I now own the method, the architecture, and the team's delivery and training.

The work involves understanding business logic from existing dashboards and warehouse views, modelling that meaning in the semantic layer, and integrating it with an agentic platform. That platform is Gemini-powered, with domain-expert agents that use Looker as their source of business context before querying BigQuery.

## How the build is accelerated

I designed the process as a system of agent skills: a pre-run check that the metadata catalogue (Atlan) holds enough business context, automated extraction of dashboard logic and BigQuery lineage, LookML generation, an automated test suite, and one human review of the flags the process raises. The dashboards are then re-pointed at Looker so the enterprise source of truth stays in one place. This compresses a manual, multi-phase process substantially; subject-matter experts still validate the results.

## What the public demonstration will make tangible

The independent demonstration will focus on a small fictional dataset:

- Compare competing definitions of the same metric.
- Expose differences in grain, filters, and effective dates.
- Require review before accepting an extracted definition.
- Trace a metric to the fields and logic that support it.
- Show how those definitions shape a conversational answer.

These are demonstration goals, not claims that every capability has been implemented in the client engagement.

## Evidence to add

An original architecture visual, a synthetic business-logic example, a walkthrough of semantic modelling decisions, and validation results as the work progresses.

[Explore the planned public scenario](../demo/README.md) · [Back to the portfolio](../README.md)
