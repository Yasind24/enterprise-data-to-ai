# From scattered business logic to a semantic layer

**Status:** Architecture pattern. A generalised approach, not an account of any specific organisation.

## The business problem

In many enterprises, business meaning is spread across BI dashboards (such as Tableau and Power BI) and warehouse views. Answering questions about enterprise data depends on understanding that logic, not on interpreting field names alone.

## The pattern

Build a semantic layer (for example, Looker over BigQuery) that captures business meaning once, organised by business domain. Model the logic found in existing dashboards and warehouse views, then let domain-expert AI agents use the semantic layer as their source of business context before they query the warehouse.

## Accelerating the build with agent skills

The modelling work can be run as a system of agent skills:

- A pre-run check that the metadata catalogue holds enough business context.
- Automated extraction of dashboard logic and warehouse lineage.
- Generation of semantic-model code (such as LookML).
- An automated test suite.
- One human review of the flags the process raises.

Dashboards can then be re-pointed at the semantic layer so the source of truth stays in one place. Subject-matter experts still validate the results.

## What the public demonstration will make tangible

The independent demonstration will focus on a small fictional dataset:

- Compare competing definitions of the same metric.
- Expose differences in grain, filters, and effective dates.
- Require review before accepting an extracted definition.
- Trace a metric to the fields and logic that support it.
- Show how those definitions shape a conversational answer.

## Evidence to add

An original architecture visual, a synthetic business-logic example, a walkthrough of semantic modelling decisions, and validation results from the demonstration.

[Explore the planned public scenario](../demo/README.md) · [Back to the portfolio](../README.md)
