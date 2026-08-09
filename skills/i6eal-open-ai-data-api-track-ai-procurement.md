---
name: Track German and EU public AI procurement
description: >-
  Pull the i6eal AI procurement chronicle and its revision trail to answer who is buying AI
  in the German and EU public sector, and what changed since you last looked.
api: openapi/i6eal-open-ai-data-api-openapi.json
operations:
  - getProcurementChronicleIndex
  - getProcurementChronicleEvents
  - getProcurementChronicleMethodology
  - getProcurementChronicleAtom
  - getProcurementObservedChangesIndex
  - getProcurementObservedChangesChanges
  - getProcurementObservedChangesArchive
  - getFederalAiBudgetMonitorTitles
generated: '2026-08-09'
method: generated
source: openapi/i6eal-open-ai-data-api-openapi.json + https://i6eal.de/llms.txt
---

# Track German and EU public AI procurement

Two datasets work as a pair: the **Procurement Chronicle** holds the durable procedure
chains, and **Observed AI Procurement Changes** holds the revision trail over them. Read
both; the chronicle alone will not tell you what moved.

## Steps

1. **Read the methodology first.** `getProcurementChronicleMethodology` →
   `GET /data/ki-auftragschronik/methodology.json`. It states the collection rules and the
   `sourcePolicy` (`officialOnly: true` plus an `allowedHosts` allowlist). Do not
   characterise the dataset without it.

2. **Fetch the chronicle index.** `getProcurementChronicleIndex` →
   `GET /data/ki-auftragschronik/index.json`. Note `schemaVersion`, `generatedAt`,
   `trackingSince` and `counts` before reading any figure. Procedures that were linked on an
   exact official identifier (TED/OCDS notice ids) are kept **separate** from isolated
   notices — that separation is the point of the dataset, so never merge the two counts.

3. **Take the flat table for analysis.** `getProcurementChronicleEvents` →
   `GET /data/ki-auftragschronik/events.csv` (RFC 4180, header row, UTF-8).

4. **Get the revision trail.** `getProcurementObservedChangesIndex` and
   `getProcurementObservedChangesChanges` cover newly published and materially changed
   procedure dossiers. A retrieval timestamp alone never creates an event in this dataset —
   only a material change does. `getProcurementObservedChangesArchive` holds superseded
   observations.

5. **Poll for change instead of re-downloading.** `getProcurementChronicleAtom` →
   `GET /data/ki-auftragschronik/atom.xml`, with `If-None-Match`. A `304` means nothing
   moved. Compare the index's `materialFingerprint` across fetches to confirm a real content
   change without diffing the payload.

6. **Optional — cross the money.** `getFederalAiBudgetMonitorTitles` →
   `GET /data/ki-haushaltsmonitor/titles.csv` gives federal budget titles with explicit AI
   references. **Only join on exact federal budget title numbers.** A shared or similar
   name never creates a link between a budget line and a procurement.

## Rules that govern the answer

- Appropriations, supplements, actuals and official revisions are kept separate in the
  budget monitor. Do not sum them into one "spend" number.
- Report source coverage and observation period separately. The chronicle's observation
  window began 2026-07-19; its source coverage reaches back to 2023-11-10.
- Every figure is quoted with its data state date. Cite as
  `i6eal (YEAR): DATASET NAME, data state YYYY-MM-DD. URL`.

## Conventions

No authentication. No rate limits published. Send conditional requests. A `404` returns an
HTML page, not a JSON error — see `errors/i6eal-open-ai-data-api-problem-types.yml`.
