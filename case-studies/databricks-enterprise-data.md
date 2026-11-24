# Cross-domain enterprise data exploration

**Status:** Architecture pattern. A generalised approach, not an account of any specific organisation.

## The business problem

Enterprise data is often spread across domains, with fragmented metadata, lineage, and business context. A conversational interface needs a way to organise that context and help users navigate the data.

## The pattern

Create domain-specific data workspaces (for example, Genie spaces in Databricks), coordinated by a supervisor agent. Above that, an orchestration agent (for example, built with the Claude Agent SDK) works across the supervisor, a web-search agent, and MCP-connected tools, so internal data and outside context can be combined behind a single chat interface.

## Why the architecture matters

**Domain boundaries:** Separate workspaces give each domain its own context for data exploration.

**Orchestration in two layers:** A supervisor agent coordinates the domain workspaces, and an orchestration agent works across that supervisor, external search, and other tools behind one user experience.

**Application delivery:** A conversational UI makes the platform usable beyond its configuration surfaces.

## Evidence to add

- An original architecture visual.
- A recreated question-to-answer walkthrough using synthetic data.
- A clear account of design choices, limitations, and validation.

[Back to the portfolio](../README.md)
