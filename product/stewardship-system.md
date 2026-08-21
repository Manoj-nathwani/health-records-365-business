---
title: The stewardship system
description: The per-customer source map that makes accountability operational — the core internal asset, not the PDFs.
tags:
  - product
  - operations
  - stewardship
status: canonical
---
# The stewardship system

Source: [Competitive Research](../Inbox/health-records-365-competitive-research.md) §22.

> The core asset is not merely a collection of PDFs.

The underlying product is a **stewardship system**. What makes [accountability](../market/differentiation.md) real — rather than a marketing claim — is that we maintain an internal map of every source that should exist for a customer, and its current state.

## The source map

Each customer eventually has something like:

| Provider/source | Period | Status | Last action |
| --- | --- | --- | --- |
| GP practice A | 1994–2018 | Complete | Jun 2026 |
| GP practice B | 2018–2026 | Received | Aug 2026 |
| NHS hospital trust | 2021 | Incomplete | Chasing |
| Private gastroenterologist | 2023–2024 | Complete | Jul 2026 |
| Dubai provider | 2026– | Active | Continuous |
| Bangkok hospital | Dec 2026 | Expected | — |

This is the artefact no competitor in the [DIY software layer](../market/competitors/landscape.md) has, because it only exists when someone is *responsible* for completeness. It is also what lets us answer "is this history actually complete?" — the question AI cannot answer for itself.

## What sits on top

1. source documents
2. reconstructed longitudinal history
3. episodes/topics
4. medications and vaccinations
5. laboratory history
6. open and unresolved items — see [the open-loop lifecycle](./open-loops.md)
7. provider-specific output packs

These are the customer-visible [outputs](./outputs.md). The source map is mostly internal, though a simplified view of "what we have and what we're still chasing" is likely valuable to show.

## Why this is the product

> **AI can reason over the records it has. Health Records 365 makes sure it has the right history.**

Active completeness — knowing which sources *should* exist and pursuing the missing ones — is the first row of the [moat table](../market/differentiation.md) and the thing that cannot be replicated by shipping features.

## Open design questions

- How is the expected-source list built for a new customer? Interview, GP record inspection, or both?
- What triggers a chase, and how often?
- How much of the map should the customer see?
- What does "complete" mean when the customer cannot remember a provider?

These should be answered by delivering the first cohort — see [validation plan](../go-to-market/validation-plan.md).

## Related

- [Inputs](./inputs.md)
- [The labour question](../go-to-market/labour-economics.md) — the cost side of stewardship
- [The commercial architecture](../commercial/layers.md)
