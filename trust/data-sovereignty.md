---
title: Data sovereignty, privacy and trust
description: "The commitments that make health data trustworthy: UK hosting by default, full portability, preserved evidence and visible conflicts."
tags:
  - trust
  - privacy
  - data
status: canonical
---
# Data sovereignty, privacy and trust

Source: [Master Business Blueprint](../Inbox/health-records-365-business-blueprint.md) §27.

Health information is among the most sensitive information customers possess. Data control should be a **major trust advantage**.

## Core principle

> **Your medical history should not be locked to Health Records 365, our software or a foreign jurisdiction.**

## The commitments

**Default hosting** — a sensible default is UK/London-hosted infrastructure for customer records, subject to the final technical and compliance design.

**Portability** — customers should be able to export their complete record.

**Flexible hosting** — where commercially and operationally appropriate, other data-location arrangements or customer-controlled infrastructure can be supported.

**Preserve source evidence** — original documents remain available rather than being replaced by generated summaries.

**Traceability** — important derived information should be traceable back to its source.

**Preserve uncertainty** — suspected diagnoses must not become confirmed diagnoses simply because a system summarised them. See [uncertainty in the record](../product/uncertainty.md).

**Keep conflicts visible** — when the historical record contains disagreement, show it rather than manufacturing a clean answer.

**Customer control** — *your records remain yours.*

## Necessary, but not a differentiator

Many competitors already emphasise customer ownership, downloads, local-first data, source retention and privacy. *"Your records remain yours"* is good messaging — it is not a position. Data ownership is now [table stakes](../market/table-stakes.md).

Customers pay for continuity, completeness, confidence, convenience and **accountability**. Privacy is a trust *requirement*: its absence loses the sale, its presence does not win it.

## Why this is a strategy, not a compliance chore

The business should be defensible because of **trust, relationship and maintained continuity** — not because customers are trapped. Portability is a strength; see [business model thesis](../commercial/business-model.md).

How much customers actually care about UK hosting and portability is [an open question](../go-to-market/open-questions.md) worth testing early, since it affects infrastructure decisions.

## Outstanding work

- (TODO: needs source) The final compliance design — UK GDPR basis for processing special-category health data, DPIA, data-processor arrangements with any AI vendors, and retention policy — is not yet specified anywhere. This should be resolved before the first paying customer's records are handled.
- **Specialist UK privacy and regulatory advice must be obtained before handling customer records at production scale** ([Competitive Research](../Inbox/health-records-365-competitive-research.md) §15). This is step 9 of the [validation plan](../go-to-market/validation-plan.md).

## Related

- [The regulatory boundary](./regulatory-boundary.md)
- [AI positioning](../product/ai-positioning.md)
- [Technical decisions](../product/tech-decisions.md)
