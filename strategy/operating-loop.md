---
title: The core operating loop
description: Collect, preserve, structure, reconcile, connect, surface, help use, update — the internal service loop and the recurring customer loop.
tags:
  - strategy
  - operations
  - service-design
status: canonical
---
# The core operating loop

Source: [Master Business Blueprint](../Inbox/health-records-365-business-blueprint.md) §6.

Internally, the service can be understood as:

**Collect → Preserve → Structure → Reconcile → Connect → Surface → Help use → Update**

```mermaid
flowchart LR
  A[Collect] --> B[Preserve]
  B --> C[Structure]
  C --> D[Reconcile]
  D --> E[Connect]
  E --> F[Surface]
  F --> G[Help use]
  G --> H[Update]
  H --> A
```

**Collect** — bring together the raw record. See [inputs](../product/inputs.md).

**Preserve** — keep original reports, letters, PDFs and source material.

**Structure** — organise information into meaningful health topics, episodes, results, medications, vaccinations and history.

**Reconcile** — identify conflicts, duplicate information, uncertain diagnoses and changing clinical opinions.

**Connect** — join information across providers and years when it relates to the same health thread.

**Surface** — make important unresolved or overlooked information visible. See [open and unresolved history](../product/open-loops.md).

**Help use** — prepare relevant information for appointments, specialists, second opinions, treatment or moves. See [outputs](../product/outputs.md).

**Update** — incorporate the outcome back into the history so the record becomes more useful over time.

## The recurring customer loop

Simpler, and the thing to actually say out loud:

> **Send us what happens next. We'll keep the history together.**

This is the loop that produces [recurring revenue](../commercial/business-model.md) and the [long-term retention effect](../commercial/retention-loop.md).

## Related

- [Customer experience](../product/customer-experience.md) — the same loop from the customer's side
- [Ongoing health record management](../commercial/offerings.md)
