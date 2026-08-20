---
title: Technical and product decisions
description: Decisions taken so far — notably not building the product on OpenKnowledge — and the paradigm worth keeping.
tags:
  - product
  - technical
  - decisions
status: canonical
---
# Technical and product decisions

Source: [Master Business Blueprint](../Inbox/health-records-365-business-blueprint.md) §35.

Technology is deliberately **not the current strategic focus**. The first goal is to prove the service and workflow — see the [validation plan](../go-to-market/validation-plan.md).

## Decision: do not build the product on OpenKnowledge

**Do not base the product on OpenKnowledge/Inkeep's OpenKnowledge interface.**

OpenKnowledge was useful for validating the interaction model — files/folders, readable content and chat — but the interface is not sufficiently clean or controllable for the intended premium customer experience.

Building the customer surface directly gives:

- complete control over UX
- no dependence on a GPL codebase for the product UI
- a cleaner service-first experience
- a simpler privacy and data-location story
- freedom to design health-native views rather than developer-oriented knowledge tooling

> Note: this knowledge base itself runs on OpenKnowledge. That is an internal working tool for the founding team and is unaffected by this decision, which concerns the customer-facing product only.

## The paradigm to keep

> **durable, understandable source material + structured history + conversational access**

— without making OpenKnowledge part of the product or business plan.

A conceptual portable record may eventually contain things equivalent to knowledge/narrative history, structured data, source documents, and metadata/provenance. Those are implementation details, not customer messaging.

## Related

- [Interface direction](./interface.md)
- [AI positioning](./ai-positioning.md)
- [Data sovereignty](../trust/data-sovereignty.md)
