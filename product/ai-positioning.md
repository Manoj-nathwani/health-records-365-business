---
title: AI positioning
description: AI is used heavily underneath the service without becoming the product story.
tags:
  - product
  - ai
  - messaging
status: canonical
---
# AI positioning

Source: [Master Business Blueprint](../Inbox/health-records-365-business-blueprint.md) §28.

Modern AI can be heavily used underneath the service without becoming the product story.

Customer-facing language should generally be:

> **Modern technology helps us organise and understand complex medical histories while preserving the original records and their context.**

The customer does not need to know which language model is used. Specific vendors, model routing, embeddings and inference architecture are implementation details — unless they materially affect privacy, jurisdiction or contractual terms, in which case they belong in [data sovereignty](../trust/data-sovereignty.md).

Human oversight should be retained where it materially improves accuracy, trust or safety. How much human review a premium trust level actually requires is [an open question](../go-to-market/open-questions.md).

## The visible benefit

The strongest visible benefit of AI is not "AI-powered healthcare." It is the ability to naturally [ask useful questions of a complete, carefully maintained history](./ask-your-history.md).

## But AI is not a moat — it strengthens the stewardship thesis instead

**From the [competitive research](../Inbox/health-records-365-competitive-research.md) §§9–10.** Guava, KeepMD, exora and Tempus olivia already ship AI summaries and conversational Q&A; ChatGPT Health and Claude + HealthEx are moving directly into personal health records. "Ask your medical history" is an excellent experience and [table stakes](../market/table-stakes.md).

The valuable question becomes:

> **Is the medical history being queried actually complete and trustworthy?**

An AI model can reason only over what it has. It cannot reason over a hospital record never obtained, pathology stuck in another system, a Bangkok discharge note never supplied, an MRI whose provider has been forgotten, or old private letters sitting in email.

That moves the hard problem upstream, to [the stewardship system](./stewardship-system.md):

> **AI can reason over the records it has. Health Records 365 makes sure it has the right history.**

Commoditising AI is therefore good for us: it raises the value of the input we control.

## Constraints

- AI must not collapse [uncertainty](./uncertainty.md) into false confidence.
- AI output must stay inside [the regulatory boundary](../trust/regulatory-boundary.md).
- AI vocabulary stays out of customer-facing copy — see the [language guide](../brand/language.md).

## Related

- [Strategic principles](../strategy/principles.md) — "AI is infrastructure"
- [Competitive landscape](../market/competitors/landscape.md) — why "upload + chat" is not a moat
