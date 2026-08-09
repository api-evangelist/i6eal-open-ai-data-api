---
name: Discover i6eal datasets and resolve a distribution URL
description: >-
  Find which of the 16 i6eal AI-policy datasets answers a question, then resolve the exact
  JSON/CSV/Atom URL to fetch — using the DCAT catalogue as the map rather than guessing paths.
api: openapi/i6eal-open-ai-data-api-openapi.json
operations:
  - getOpenDataCatalogue
generated: '2026-08-09'
method: generated
source: openapi/i6eal-open-ai-data-api-openapi.json + https://i6eal.de/llms.txt
---

# Discover i6eal datasets and resolve a distribution URL

Use this before any other i6eal skill. The API has no query parameters and no search
endpoint — selection happens by choosing a URL, and the DCAT catalogue is the only
authoritative map of which URLs exist.

## Preconditions

- **No credentials.** The API requires no key, no registration and no headers. If you are
  building an auth step, you have misread the contract.
- Send `If-None-Match` with any ETag you already hold. The catalogue is rebuilt daily and a
  conditional GET returns `304` when nothing changed.

## Steps

1. **Fetch the catalogue.** `getOpenDataCatalogue` → `GET https://i6eal.de/data/catalog/dcat.jsonld`
   (`application/ld+json`). It is a `dcat:Catalog` holding 16 `dcat:Dataset` nodes and 82
   `dcat:Distribution` nodes.

2. **Pick the dataset by meaning, not by name match.** Read `dct:title` and
   `dct:description` — both carry a German and an English literal as `@value`/`@language`
   pairs. Read `dct:source` to see which official upstream registers feed it (TED,
   Bundeshaushalt, EUDAMED, CTIS, Eurostat, Bundestag DIP, and so on). If no dataset covers
   the question, say so; do not substitute a neighbouring dataset.

3. **Check the dataset is still being collected.** `i6eal:collectionState` (`active` on the
   datasets observed) and `i6eal:collectionCadence` (`daily`) tell you whether the numbers
   are current. `i6eal:observedSince` is when i6eal started watching; `dct:temporal` /
   `schema:temporalCoverage` is when the underlying events happened. **These are different
   dates and must never be conflated** — an older source date does not make the observation
   history older.

4. **Resolve the distribution.** Inside the chosen dataset, each `dcat:distribution` carries
   `dcat:accessURL`, `dcat:downloadURL`, `dct:format` and `dcat:mediaType`. Choose by format:
   - `application/json` `index.json` → the full projection, with counts and provenance
   - `text/csv` → a flat table for analysis
   - `application/atom+xml` → the change feed
   - `methodology.json` → what the dataset does and does not claim

5. **Map to an operation if you need the spec.** A distribution's `dcat:accessURL` path is
   the OpenAPI path verbatim, so it resolves 1:1 to an `operationId` in
   `openapi/i6eal-open-ai-data-api-openapi.json`.

## Rules that govern the answer

- **Quote every figure with its date.** Every number has a data state; a bare count is a
  misquote.
- **Absence is stated, never inferred.** `not_publicly_linked` means no public evidence of
  that link was found — it does not mean the link does not exist.
- **Cite it.** `i6eal (YEAR): DATASET NAME, data state YYYY-MM-DD. URL`
- **Licence.** CC BY 4.0 covers the i6eal compilation, structure and original descriptions
  only. Underlying records keep their source-specific rights — check the dataset's own
  `dct:rights` before redistributing.

## Failure handling

A `404` returns the site's **HTML** error page, not a JSON error. Branch on the status code
and `Content-Type`. Distribution URLs are stated to be permanent, so a 404 on a URL that
previously worked is a defect worth reporting to `ai@i6eal.de`, not an expected retirement.
