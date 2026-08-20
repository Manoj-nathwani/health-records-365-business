---
title: The identity question
description: What business this actually is — the invariants, the three candidate identities, the recommended synthesis, and what would reverse it.
tags:
  - strategy
  - identity
  - decision
status: proposal
---
# The identity question

> **What business is this?** The question sounds answered — *a managed medical-history service* — but the [navigation](../product/navigation.md) and [concierge-led](../commercial/concierge-led.md) threads pull at it hard enough that it has to be re-asked properly rather than patched.

This doc is the review: what has survived every revision, the three identities on the table, the recommendation, and what would reverse it.

## The invariants

Eight things have survived every revision — blueprint, competitive research, reference implementation, clinical ladder, navigation. Whatever the identity is, it is built from these:

1. **The unit is the person, not the provider.** No system owns the whole story; we exist to be the continuity layer around the individual
2. **Accountability is the product.** Someone whose *job* it is. Features are [table stakes](../market/table-stakes.md)
3. **Independence.** No commissions, no stake in what the record says or where care happens. The trust position and the moat share a root
4. **The reconciled record is the substrate.** Every distinctive act — the nudge, the sequencing, the prepared consultation — comes out of it. Without it, everything else is a commodity
5. **We never diagnose.** Clinical judgement is bought from registered clinicians ([the ladder](./clinical-capability.md)) or not offered
6. **The customer is internationally mobile, carries real history, delegates willingly, and can pay**
7. **Service first, manual first.** Software follows real edge cases
8. **Distribution is partner-led**, after a small direct proof base

Nothing below contradicts these. The question is which *face* leads.

## Three candidate identities

### A — The record company

*"We build and maintain your complete medical history."* The original thesis.

**For:** bounded, batchable, defensible, legible to a chartered partner's diligence. The method is real and demonstrated.
**Against:** sells homework; anchors against [Chronicle at £399](../market/competitors/chronicle-health.md); stops at the moment of maximum need (*"so what do I do?"*); the deliverable is invisible when it works.

### B — The navigation company

*"We handle your healthcare logistics, anywhere."* The concierge face.

**For:** sells relief; anchors against [family offices at thousands](../market/competitors/sip-medical-family-office.md); felt on every use; matches the strongest [trigger](../market/triggers.md); the adviser sentence writes itself.
**Against:** without the record it is a booking agency — hotel-desk medicine with better manners; reactive, timezone-scattered ops; invites emergency expectations we must refuse.

### C — The stack: an independent medical office

Neither layer alone — **the stack is the identity.** The shape of a medical family office, minus the medicine, at mid-market price, grounded in a record none of them keep:

| Layer | Face | Status |
| --- | --- | --- |
| **The record** | Foundation — built at onboarding, because nothing else works without it | The moat |
| **Stewardship** | The membership — kept current, [loops tracked](../product/open-loops.md) | The relationship |
| **[Navigation](../product/navigation.md)** | The experienced service — research, itineraries, scripts, bookings | The sell |
| **[Partnered clinical](../product/record-review.md)** | The completion — a GP who has read the file, under their own registration | The ceiling-raiser |

## Why C is the answer

**The customer's real question selects it.** *"I left the system that nominally owned my care — who owns it now?"* No single layer answers that. The stack does. The functional job (history complete, care handled), the emotional job (relief, control) and the social job (*"I have people for that"*) are served by the stack and only partially by any layer.

**Each layer alone is occupied or copyable; the stack is empty.** DIY apps below, family offices above, [Chronicle](../market/competitors/chronicle-health.md) one-off, [VITALL](../market/competitors/vitall.md) managing records without navigation or cross-border. Nobody is *independent + mid-market + cross-border + record-grounded*. That is [the missing middle](../market/missing-middle.md), finally stated as an identity rather than a price gap.

**The layers defend each other.** Navigation without the record is a commodity; the record without navigation is homework; clinical without independence is a sales funnel. Together each fixes the others' weakness — which is what an identity is supposed to do and a product list does not.

**The economics prefer it.** Membership (onboard → annual → premium family) replaces the three-product menu. The record build becomes the initiation — *"we cannot plan your care without knowing your history"* — and the Chronicle comparison dissolves, because nobody compares an initiation fee to a rival's whole product.

**And it is what the founder already built for himself.** The [reference implementation](../operations/reference-implementation.md) is not a record with some trips attached; it is a record *driving* a multi-city care itinerary with scripts, fallbacks and dependency ordering. The company is the thing he made, productised.

## The position

> **Position (2026-08-20):** Health Records 365 is an **independent medical office for internationally mobile people** — the record is the foundation, membership is the product, navigation is the experienced service, and clinical judgement is partnered, never ours.
>
> **Why:** the stack is the only unoccupied position; the layers defend each other; the anchoring, the adviser sentence and the founder's own demonstrated use all point the same way.
>
> **Reverses if:** the first customers buy the record pack and decline membership; advisers report the unmet demand is records-out rather than care-handled; or planned-care navigation proves unservable by one person across timezones.

The [framing test](../commercial/concierge-led.md) and [the Sojourner's question](../go-to-market/sojourners-capital.md) are the ratification evidence, and both are already scheduled. **This is a position to sell from now, not a rebrand to execute today.**

## Tensions to resolve deliberately

**The name.** *Health Records 365* names the foundation layer, not the identity — the constraining word is "Records", while "365" fits the year-round handling well. A records-name has trust value (*we are the record people, not a clinic*) and renaming is expensive; parked, revisit after the first cohort. **Reopens if** prospects repeatedly mis-categorise us as a document service.

**"[What we are not](./what-we-are-not.md)" says not a Medical Family Office.** Still true, precisely: no staff physicians, no five-figure retainer, no medicine. We take the *architecture* of that world, not its scope. The doc needs one clarifying line, not a reversal.

**"One job" widens.** [The principles](./principles.md) say the job is *manage the person's medical history*; the identity widens it to *someone is handling my healthcare*. Same [accountability](../market/differentiation.md) promise, larger surface — the principle gets re-derived, not broken.

**The emergency boundary becomes existential.** A "medical office" invites 3am calls. **Planned and semi-planned care only** is now an identity-level exclusion, stated everywhere the concierge face appears — emergencies are International SOS's industry, not ours.

## What re-derives once ratified

In dependency order, per the KB's own rule that a conclusion is recomputed when its basis moves:

1. [North star](./north-star.md) — the definition widens; the promise likely becomes *your healthcare, handled, wherever life takes you*
2. [The proposition](./proposition.md) and [principles](./principles.md) — "one job" restated
3. [The three products](../commercial/layers.md) → the membership architecture
4. [Pricing](../commercial/pricing.md) — onboarding + annual + premium, with navigation the annual's content
5. [Site architecture](../website/strategy.md) and the hero — concierge face forward, method pages unchanged as the trust engine
6. [Adviser one-pager](../go-to-market/adviser-one-pager.md) — the improved sentence
7. [Risk register](../legal/risk-register.md) — add scope creep, reactive load, commission temptation, emergency-expectation management

Everything in [operations](../operations/), [trust](../trust/) and the [method pages](../website/how-it-works.md) stands unchanged — the engine is the engine regardless of which face leads.

## Related

- [Concierge-led selling](../commercial/concierge-led.md) — the hypothesis this review generalises
- [Clinical capability](./clinical-capability.md) — the ladder the top layer stands on
- [Differentiation](../market/differentiation.md) — accountability, unchanged throughout
