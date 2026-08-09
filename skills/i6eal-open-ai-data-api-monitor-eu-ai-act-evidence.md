---
name: Monitor EU AI Act supervision, standardisation, transparency and enforcement
description: >-
  Assemble the regulatory picture around the EU AI Act from the four i6eal monitors that
  cover who supervises, what is being standardised, which providers have published
  transparency evidence, and what has actually been enforced.
api: openapi/i6eal-open-ai-data-api-openapi.json
operations:
  - getAiSupervisionMonitorIndex
  - getAiSupervisionMonitorAuthorities
  - getAiSupervisionMonitorInstruments
  - getAiSupervisionMonitorRelationships
  - getAiStandardisationMonitorIndex
  - getAiStandardisationMonitorWorkItems
  - getAiStandardisationMonitorFeed
  - getEuAiTransparencyEvidenceMonitorProviders
  - getEuAiTransparencyEvidenceMonitorEvidence
  - getGermanyEuAiEnforcementMonitorActions
  - getGermanyEuAiEnforcementMonitorEvidence
  - getGermanyEuAiEnforcementMonitorFeed
generated: '2026-08-09'
method: generated
source: openapi/i6eal-open-ai-data-api-openapi.json + https://i6eal.de/llms.txt
---

# Monitor EU AI Act supervision, standardisation, transparency and enforcement

Four datasets answer four different questions. Keep them apart — the whole design of these
datasets is that visibility, conformity and effectiveness are separate things.

## 1. Who supervises — Supervision Monitor

- `getAiSupervisionMonitorIndex` → `GET /data/ki-aufsichtsmonitor/index.json`
- `getAiSupervisionMonitorAuthorities` → authorities.csv
- `getAiSupervisionMonitorInstruments` → instruments.csv (the legal instruments)
- `getAiSupervisionMonitorRelationships` → relationships.csv

Officially evidenced responsibilities and instruments only. **There is no compliance score
and no effectiveness rating in this dataset, and you must not construct one.**

## 2. What is being standardised — Standardisation Monitor

- `getAiStandardisationMonitorIndex`, `getAiStandardisationMonitorWorkItems`
- `getAiStandardisationMonitorFeed` → `feed.atom`, for change polling

The standardisation request, work items, lifecycle events and EU references are separate
evidence lanes. A work item existing is not the same as a harmonised standard being cited.

## 3. Who published transparency evidence — Transparency Evidence Monitor

- `getEuAiTransparencyEvidenceMonitorProviders` → providers.csv
- `getEuAiTransparencyEvidenceMonitorEvidence` → evidence.csv

Covers Articles 50 and 53. **Visibility and review progress are explicitly separate from
conformity** — a provider appearing here has published something, not been found compliant.

## 4. What has been enforced — Enforcement Monitor

- `getGermanyEuAiEnforcementMonitorActions` → actions.csv
- `getGermanyEuAiEnforcementMonitorEvidence` → evidence.csv
- `getGermanyEuAiEnforcementMonitorFeed` → `feed.atom`

Published investigations, orders, fines and remedies, with procedural stages kept separate
from the technology evidence that the matter was AI-related.

## Assembling an answer

1. Fetch each dataset's `index.json` first and record `generatedAt`, `trackingSince` and
   `counts`.
2. Join across the four only on exact official identifiers. A shared authority *name* or
   provider *name* is not a link.
3. Where the evidence does not join, say it does not join. `not_publicly_linked` is a
   finding, not a gap to paper over.
4. State each figure with its data state date and cite:
   `i6eal (YEAR): DATASET NAME, data state YYYY-MM-DD. URL`.
5. Note the small absolute counts where relevant — several of these monitors track tens, not
   thousands, of records. Present them as observed evidence, not as a census.

## Conventions

No authentication, no rate limits published, CORS open. Poll the Atom feeds with
`If-None-Match` rather than re-downloading. A `404` returns HTML, not a JSON error.
