---
title: Customer mandate
description: The signed authority that permits Health Records 365 to request records from providers on a customer's behalf.
tags:
  - legal
  - retrieval
  - consent
status: todo
---
# Customer mandate

**Status: not yet drafted.** Without it, [retrieval](../operations/retrieval-playbook.md) cannot happen at all.

## What this document has to do

- Authorise us to request records from named and as-yet-unknown providers on the customer's behalf
- Satisfy what GP practices, NHS trusts and private providers will actually accept — requirements differ by source and must be confirmed against real submissions
- Cover overseas providers, where the mechanism may be entirely different
- Establish informed consent for us to process the resulting [special-category data](./compliance.md)
- Be revocable, and state what happens to held records on revocation
- Be renewable, since [ongoing management](../commercial/layers.md) means requesting records indefinitely, not once

## The design question

A one-off authority is simpler to obtain but breaks membership. A standing authority supports [continuous stewardship](../product/stewardship-system.md) but is a harder thing to ask someone to sign, and a harder thing for a provider to accept. Resolve this before the first cohort.

The [office identity](../strategy/identity.md) settles the direction: membership means requesting records and **making bookings on the customer's behalf indefinitely**, so the mandate is standing by design — and must cover arranging appointments as well as requesting records, which may be two different authorities in a provider's eyes.

## Related

- [Compliance foundation](./compliance.md)
- [Terms and privacy policy](./terms.md)
