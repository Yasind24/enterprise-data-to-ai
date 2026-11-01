# Cross-domain enterprise data exploration with Databricks

**Status:** Prior client engagement. This is a high-level account of my work; client assets and quantitative impact claims are not included.

## The business problem

Enterprise data was spread across domains, with fragmented metadata, lineage, and business context. Providing a conversational interface required a way to organise that context and help users navigate the data.

## My contribution

I architected the platform and built it with a small development team. Claude, through the Claude Agent SDK, orchestrated the experience. Beneath it, I created domain-specific Genie spaces in Databricks, coordinated by Databricks' Supervisor Agent. A web-search agent and MCP-connected tools added external context, so internal customer data and outside signals could be combined for sales research such as cross-sell, upsell, and renewals. A chatbot UI let users work with it.

The platform was piloted with a small group of sales users, and I moved to another engagement while it was being scaled up.

I also built an opportunity-discovery pipeline in the broader flow, covering electric and gas opportunities involving government utility entities and potential clients.

## Why the architecture matters

**Domain boundaries:** Separate workspaces provided domain-specific contexts for data exploration.

**Orchestration in two layers:** Databricks' Supervisor Agent coordinated the Genie spaces, and Claude orchestrated across that supervisor, a web-search agent, and other tools behind a single user experience.

**Application delivery:** A conversational UI made the platform accessible to users beyond its configuration surfaces.

## Two workflows to showcase

1. **Enterprise data exploration:** a user asks a question through the UI; domain workspaces and the supervisor support the interaction.
2. **Opportunity discovery:** a separate pipeline supports understanding electric and gas opportunities.

A future public walkthrough will use synthetic examples and explain each workflow separately.

## Evidence to add

- An original architecture visual reflecting the components I can discuss publicly.
- A recreated question-to-answer walkthrough.
- A clear account of design choices, limitations, and validation.
- Measured outcomes only where evidence is available and disclosure is authorised.

[Back to the portfolio](../README.md)
