---
title: Health navigation
description: "The independent planner over the record: research the options, plan the visits, script the appointments, nudge toward the unfinished — never diagnose."
tags:
  - product
  - navigation
  - concierge
status: canonical
---
# Health navigation

**The record says what is unfinished. Navigation is everything we do about it short of clinical judgement:** research the options, compare providers and prices, plan the visits, prepare the words to say, and bring the outcomes home to the record.

The internal analogy is a **travel planner** — takes the customer's needs, does the research, builds the itinerary, books the thing, and is **totally independent**: no stake in which airline, no commission from the hotel. It plans the trip. It does not fly the plane.

This is steps 1–2 of [clinical capability](../strategy/clinical-capability.md) promoted from "take opportunistically" to **core product**. [The record review](./record-review.md) remains the optional clinical layer on top.

## What it looks like, concretely

Customer zero's own working files are the template — every element below exists in the [reference implementation](../operations/reference-implementation.md) as a real artifact:

| Element | What it is |
| --- | --- |
| **The nudge** | "The record shows a repeat test was recommended in 2024 and nothing later appears. Here is what closing it would involve" — a statement about the record, with a path attached |
| **The options research** | Which providers offer it, where, at what price, with what caveats — including "this is 5–8× cheaper in Bangkok than London, and here is the reliability trade-off" |
| **The itinerary** | Care sequenced around real life: what happens in which city, in which order, and the dependencies — *the baseline draw must precede stopping the supplement; the scope needs 5–7 days after* |
| **The script** | The exact words for the appointment: *"I completed a three-dose pre-exposure course in 2018 — I want a single booster, not a new primary course"* — and what to get in writing before leaving |
| **The booking** | Contact the provider, make the request, handle the back-and-forth |
| **The return** | Results and letters come back into the record, loops close, and the next nudge is better informed |

## The grammar of a safe nudge

Every nudge has the same three-part shape, and the shape is what keeps it inside [the boundary](../trust/regulatory-boundary.md):

1. **What the record shows** — factual, sourced: *ordered and no result held · recommended and never booked · abnormal and never repeated · lapsed without explanation*
2. **What acting on it would involve** — providers, prices, logistics, sequencing
3. **Who decides** — the customer and their clinician. *Whether* to act is never ours

So: ✓ *"Nothing in the record shows the 2021 finding was ever followed up; a gastroenterology consultation would address it, here are three options near you."* ✗ *"You should get a colonoscopy."* The first is librarianship plus logistics. The second is medicine.

**Independence is what makes the nudge trustworthy.** We take nothing from any provider we recommend — no commission, no kickback, no preferred-partner fee. The moment a nudge earns us money from the provider, it stops being information — same [firewall](./record-review.md) as the clinical layer, and worth stating publicly.

## Why this is the right core product

- **It is what the customer actually buys.** [Why customers pay](../market/why-customers-pay.md) lists time, expertise, convenience, preparation — navigation is all four in one deliverable
- **It closes the value gap without regulatory weight.** The *"so what do I do?"* moment gets a real answer — a researched plan — without anyone practising medicine
- **Nobody else can do it well**, because the plan is only as good as the record beneath it. A concierge without the history books appointments; we sequence care — the [moat](../market/differentiation.md) compounding
- **It generates its own retention.** Every executed plan returns documents, which improve the record, which sharpens the next nudge — [the loop](../commercial/retention-loop.md), self-feeding
- **Travel-agent independence is a position competitors cannot copy** — most health platforms monetise referrals; we structurally refuse to

## The unit of work: the episode of care

Navigation is delivered in **episodes**. An episode opens — a nudge acted on, an appointment needed, a move to plan — and closes only when its outcomes are home in the record:

```text
Opened (nudge, need, or move)
        ↓
Planned — options researched, sequenced against the record
        ↓
Booked — provider contacted, appointment made, script prepared
        ↓
Attended
        ↓
Outcomes home — results and letters into the record
        ↓
Closed — and the open loops it touched update
```

An episode without its outcomes home is not closed, however well the appointment went — the return leg is the half everyone skips, and it is the half that keeps the record true.

## Prepared to be taken seriously

Clinicians routinely discount patient-held records — a folder of photocopies and a verbal history get polite skimming, not attention. The handover pack has to clear a higher bar: **it must read like a clinical document, not a patient's scrapbook.**

What earns that:

- **Every claim traceable to an original document**, attached — the clinician can verify anything in one step
- **Clinical organisation** — the structure a doctor expects, leading with what matters for *their* specialty
- **Uncertainty stated in clinical terms** — *suspected, never confirmed* rather than a tidied narrative
- **Ten-minute readability** — the relevant subset, not the archive

A pack the clinician takes seriously changes the appointment itself: the customer stops being an unreliable narrator of their own history and starts being a well-documented patient. That is a large part of what the fee buys.

## The plan is core; the errand is optional

Navigation splits along one line, and the line decides what membership includes:

| | What it is | How it is sold |
| --- | --- | --- |
| **The plan** | What is lingering, what closing each item would involve, what to raise and with whom — plus the handover pack for any appointment | **Core membership.** It is the record speaking, and it costs little beyond the record itself |
| **The errand** | Researching facilities where the customer is, making the booking, handling the back-and-forth, scripting the visit | **Optional, per episode.** Real hours, wanted by some members often and by others never |

The split prices the unbounded thing: a member who arranges everything themselves pays membership; a member who wants it handled pays per episode handled. Nobody subsidises anybody, and "can you also…" gets a price instead of a boundary.

**The pitch still leads with the full capability.** *We can arrange everything, wherever you are* sells; the pricing page is where it becomes per-episode. Capability sells, usage pays.

[Premium and family membership](../commercial/layers.md) can include arranging — once real episode frequency is known, "arranging included" is the natural content of the top tier.

Provider research is transactional — prices and availability are **re-checked at the point of booking, never kept** — so arranging is delivered fresh each time rather than from a directory that rots.

## Boundaries

- **Never diagnose, never triage urgency.** "This looks unfinished" — yes. "This looks worrying" — no. If a record shows something a reasonable person would want a doctor to see soon, the nudge is *"take this to a clinician"*, not our assessment of severity
- **Research is not endorsement.** We present options with their trade-offs; the customer chooses
- **The clinical layer stays separate.** When a nudge needs a prescription or an order behind it, that is [the record review](./record-review.md) and the partner GP's judgement

## Related

- [Open and unresolved history](./open-loops.md) — where nudges come from
- [Clinical capability](../strategy/clinical-capability.md) — the ladder
- [What we do not do](../website/what-we-do-not-do.md) — the public statement of the same line
