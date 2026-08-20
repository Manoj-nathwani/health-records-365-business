---
title: Interface direction and philosophy
description: Seven interface principles plus the current three-pane UI direction, and the developer vocabulary to keep off-screen.
tags:
  - product
  - ui
  - ux
status: canonical
---
# Interface direction and philosophy

Source: [Master Business Blueprint](../Inbox/health-records-365-business-blueprint.md) §§33, 34.

Technology is an enabler, not the business proposition.

## Seven principles

**Simple** — customers should not need to learn a health-record management system.

**Already organised** — when they open Health Records 365, the work should already have been done for them.

**Transparent** — they can inspect underlying history and source documents.

**Conversational** — they can ask questions in normal language. See [ask your medical history](./ask-your-history.md).

**Portable** — the record should not depend on Health Records 365 existing forever. See [data sovereignty](../trust/data-sovereignty.md).

**Purpose-specific** — the same underlying history can produce different views for different healthcare situations.

**Health-native** — use interfaces designed for medical-history tasks: longitudinal lab tables and charts, open-item status, source-document provenance and narrative episodes.

Do not recreate a generic note-taking application.

## Current UI direction

A clean default interface can remain extremely small — three panes:

**Left — navigation** through the customer's medical history:

- My Health
- Overview
- History
- Health topics
- Results / Bloods
- Open items
- Medications
- Documents

**Centre — a clean readable health page:** narrative history, structured topic, result trend, provider pack or source document.

**Right — Ask Health Records 365:** conversational access to the history.

Advanced users may optionally browse underlying folders/files, but this should not define the mainstream experience.

## Keep off-screen

Markdown syntax, editor toolbars, Git concepts, developer terminology, plugin systems, workspace configuration, technical AI vocabulary.

## Related

- [Outputs](./outputs.md) — what the centre pane renders
- [Technical and product decisions](./tech-decisions.md)
- [Customer experience](./customer-experience.md)
