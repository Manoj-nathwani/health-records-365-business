---
title: Reference implementation
description: A complete working personal health record already exists. What it supplies to the unwritten operations docs, and where it stops short of validating the service.
tags:
  - operations
  - customer-zero
  - evidence
status: canonical
---
# Reference implementation

A complete, working instance of the thing this business sells already exists: the founder's own health record, held as a directory of Markdown with a rules kernel governing it. It is not a prototype. It is 132 files, a four-stage pipeline, five enforcement checks and a 463-line rules document, run against a real fragmented history across the NHS, a hospital portal, Patients Know Best, private clinics in three countries and personal email.

**Source:** `/Users/manoj/local_projects/health-kb` — a separate knowledge base, deliberately siloed. Its own rules forbid cross-base links and moving facts between bases, so **nothing clinical from it is reproduced here**. What follows is method and evidence about the business.

## What it collapses

Several docs listed as unwritten in [the gameplan](../gameplan.md) already have a working answer.

| Unwritten doc | What already exists |
| --- | --- |
| [Deliverable specification](./deliverable-spec.md) | A root index structured as an International Patient Summary in prose, leading with prescribing warnings and event-triggered alerts, then the two things that matter, then active issues and exclusions |
| [QA standard](./qa-standard.md) | Two empirically discovered error shapes, below — neither of which any automated check catches |
| [The stewardship system](../product/stewardship-system.md) | A four-folder pipeline where each folder is a **contract**, not a category: staging, immutable source, re-derived conclusions, live threads |
| [Intake and source mapping](./intake.md) | Sources enumerated per provider with what each holds and what is permanently unavailable |
| [Uncertainty](../product/uncertainty.md) | A six-term certainty vocabulary in active use: confirmed, suspected, ruled out, historical, patient-observed, model synthesis |

## The method that has no equivalent in the field

The reference implementation's own competitive review found that comparable tools store Markdown and link it, but **almost nothing reconciles** — the common pattern is to append and let retrieval sort out contradictions later.

Four practices had no equivalent anywhere reviewed:

1. **Reconciliation at write time.** Every input is tested against what is already held: does it confirm, contradict, resolve, complete or change the current reading? A contradiction is resolved, not appended. The expensive work happens on the way in, not when a question is asked.
2. **Re-derivation of every index above a structural change**, as a stated obligation rather than a nicety.
3. **Questions must name what they unblock**, which is what stops an open-questions list becoming a wish list.
4. **Rules constraining the writing itself**, mechanically enforced — no filler, no announcing that a point has landed, no index whose claims rest on nothing.

This is a sharper statement of [our differentiation](../market/differentiation.md) than "accountability" alone. The product is not a store of documents. **It is the reconciliation, and the fact that someone did it on the way in.**

## The two error shapes, and why they matter for QA

Both were found by systematically re-checking every conclusion against the document beneath it.

**Shape one: a conclusion carried forward while its basis moved underneath it.** Not one error found was a mistyped number — transcription was accurate throughout, including where two laboratories a week apart agreed to the unit.

**Shape two, harder to see: the claim is true and cites a document that does not contain it.** The link resolves, the check passes, and a reader who follows it finds nothing — then doubts the sentence. A link checker proves a destination exists, never that it says what the sentence claims. **Only reading both does.**

The worst single instance is the one to put in front of anyone designing [the QA standard](./qa-standard.md): an index read *"he declined treatment"* where the source recorded **a consultant declining to treat him**. In a handover document read by a clinician who has never met the patient, those are two different patients.

A further finding, counter to expectation: **registers rot faster than conclusions do.** The lists assumed to be low-risk — medications, procedures, immunisations, measurements — held the highest density of errors, because a register is a list of current facts and current facts go stale fastest.

## A product surface we do not have

The reference implementation carries a `surveillance` topic holding **conditional triggers that fire on a future event rather than on a schedule** — dormant rules, several of which matter for decades, of the form *demand this genetic test before that drug class is ever prescribed*.

This is not an [open item](../product/open-loops.md): open items are unresolved. These are **resolved findings that must fire later**, possibly decades later, possibly in a country with no access to the record that generated them. Nothing in [outputs](./deliverable-spec.md) or the [open-loop lifecycle](../product/open-loops.md) covers it.

It is also the highest-value content in that record by its owner's own assessment, and it is kept deliberately in one scannable place because split across thirteen specialties nobody would ever see it as a set.

## A retrieval principle, learned by adopting and reverting

The reference implementation adopted OpenKnowledge and removed it the same day. It passed the survival test outright — plain Markdown in git, delete it and the record is byte-identical. **It was removed for what its search does to retrieval: it ranks source above conclusions, and no configuration changes that.**

A query returned six hits, five of them raw source documents including another person's result, while the indexes carrying the corrected conclusion never appeared.

> A tool whose primary way in ranks a superseded value above the conclusion that corrects it is not a neutral addition to a medical record — it is a second, louder answer.

This is a **safety requirement for our own retrieval design**, and it belongs in [ask your medical history](../product/ask-your-history.md). Any product doing naive similarity search over a document corpus has this failure. It is also a competitive observation: it is what most of the [AI-over-records layer](../market/competitors/landscape.md) is built on.

## What it does not validate

The gaps matter as much as the evidence.

**No timing data.** The record was built without measuring minutes per stage. [The critical unknown](../go-to-market/labour-economics.md) is still unknown, and it cannot be recovered retrospectively — it has to be instrumented on the next one.

**The founder is not a representative customer.** He can read his own histology, direct his own care and wrote the rules. A paying customer can do none of that. Cost extrapolated from this instance will **under**estimate, possibly severely.

**Nothing here was retrieved on behalf of another person.** Every document was obtained as the data subject, exercising his own access rights. The business requires acting as an agent for someone else, which is a different legal mechanism, a different provider interaction and a different failure mode — see [the customer mandate](../legal/customer-mandate.md). **This is the single largest untested assumption in the operational model**, and the reference implementation says nothing about it.

**Shape checks are silent about truth.** By its own account, every substantive error found was caught by a person supplying reality, not by a rule. This confirms the service model and confirms the [labour risk](../go-to-market/labour-economics.md) at the same time: the human is load-bearing and no amount of automation removes them.

**Completeness has a hard floor.** After exhaustive effort by a technically capable owner with full access rights, three documents remain permanently unobtainable. One of them is load-bearing: an entire diagnostic conclusion rests on a passage quoted verbatim inside a later letter, with no primary source behind it anywhere. This is direct evidence for the caveat [the terms](../legal/terms.md) must carry — **the honest promise is exhaustive pursuit, never guaranteed completeness.**

## Related

- [Gameplan](../gameplan.md)
- [Differentiation](../market/differentiation.md)
- [Delivery SOP](./delivery-sop.md)
