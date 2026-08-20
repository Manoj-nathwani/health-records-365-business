---
title: The labour question
description: The biggest commercial unknown — how many human minutes it takes to build and maintain an excellent medical history.
tags:
  - gtm
  - operations
  - risk
  - unit-economics
status: active
---
# The labour question

Source: [Competitive Research](../Inbox/health-records-365-competitive-research.md) §25.

> **The biggest unknown in the business:** how many human minutes are required to build and maintain an excellent medical history?

Everything downstream depends on this. [Pricing](../commercial/pricing.md) cannot be set without it. The decision of what to automate cannot be made without it. Whether [the missing middle](../market/missing-middle.md) is a viable business rather than a viable *idea* depends on it.

## The first customers are an operational study

The first paying customers should double as a time-and-motion study. Track these **separately** — not as one blended "delivery time":

| Activity | Minutes | Notes |
| --- | ---: | --- |
| Onboarding | | |
| Record request | | |
| Chasing | | |
| Document processing | | |
| Reconciliation | | |
| QA | | |
| Customer support | | |
| Provider-pack preparation | | |
| Recurring maintenance (per month) | | |

Use one table per customer. The recurring row is the one that determines whether the annual price works.

## Then, and only then, automate

> Only after costly and repeatable operational workflows are understood should bespoke software be built.

This is the [strategic principle](../strategy/principles.md) "manual before overbuilding" with a measurement attached. See also [technical decisions](../product/tech-decisions.md).

## Why it is a real risk, not a formality

[Chasing](../product/stewardship-system.md) is unbounded work — a hospital trust that does not respond consumes time indefinitely with no natural stopping point. The [open-loop lifecycle](../product/open-loops.md) is similarly open-ended by design. Both are core to [our differentiation](../market/differentiation.md), which means the moat and the cost driver are the same thing.

A plausible failure mode: the service is genuinely valuable, customers happily pay £995, and it still loses money per customer.

## Related

- [Validation plan](./validation-plan.md)
- [Pricing hypotheses](../commercial/pricing.md)
