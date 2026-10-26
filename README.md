# i6eal Open AI Data API (i6eal-open-ai-data-api)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

A free, no-authentication open-data REST API from i6eal (a German AI studio operated by Syka Ventures UG) exposing 16 AI-related datasets and monitors for Germany and the EU as static JSON/CSV/JSON-LD/Atom files served over HTTPS from CloudFront. Coverage spans public procurement, federal budget lines, case law, supervisory authorities, standardisation work items, EU AI Act transparency evidence, medical devices, clinical trials, platform automation, enforcement actions and adoption statistics. Backed by a live OpenAPI 3.0.3 contract with 83 GET operations, a DCAT JSON-LD catalogue of 16 datasets and 82 distributions, a provider-published llms.txt, and per-dataset Atom change feeds. No authentication, no registration, no published rate limit; CORS is open and responses carry ETag validators. The i6eal compilation is CC BY 4.0; underlying official records retain their source-specific rights.

**APIs.json:** [https://i6eal-open-ai-data-api.apievangelist.com/apis.yml](https://i6eal-open-ai-data-api.apievangelist.com/apis.yml)

## Tags

- Artificial Intelligence
- Open Data
- Public Policy
- Regulation
- Compliance
- EU AI Act
- Government
- Public Sector
- Legal
- Case Law
- Public Procurement
- Germany
- European Union

## Timestamps

- **Created:** 2026-08-05
- **Modified:** 2026-08-09

## APIs

### i6eal Open AI Data API AI Enforcement Monitor Germany & EU API

Officially published AI-related investigations, orders, fines and remedies with separate procedural stages and exact technology evidence.

- **Human URL:** [https://i6eal.de/en/tools/data/](https://i6eal.de/en/tools/data/)
- **Base URL:** `https://i6eal.de`

#### Tags

- AI Enforcement Monitor Germany & EU

#### Properties

- [OpenAPI](openapi/i6eal-open-ai-data-api-ai-enforcement-monitor-germany-eu-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/i6eal-open-ai-data-api-ai-enforcement-monitor-germany-eu-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/i6eal-open-ai-data-api-ai-enforcement-monitor-germany-eu-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](https://i6eal.de/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Documentation](https://i6eal.de/en/tools/data/)
- [JSON-LD](https://i6eal.de/data/catalog/dcat.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON-LD](json-ld/i6eal-open-ai-data-api-dcat.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Examples](examples/i6eal-open-ai-data-api-examples.yml)
- [Data Model](data-model/i6eal-open-ai-data-api-data-model.yml)

### i6eal Open AI Data API AI Parliamentary Accountability Monitor API

Parliamentary questions, answers and exactly linked proceedings from the Bundestag documentation system.

- **Human URL:** [https://i6eal.de/en/tools/data/](https://i6eal.de/en/tools/data/)
- **Base URL:** `https://i6eal.de`

#### Tags

- AI Parliamentary Accountability Monitor

#### Properties

- [OpenAPI](openapi/i6eal-open-ai-data-api-ai-parliamentary-accountability-monitor-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/i6eal-open-ai-data-api-ai-parliamentary-accountability-monitor-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/i6eal-open-ai-data-api-ai-parliamentary-accountability-monitor-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://i6eal.de/en/tools/data/)
- [JSON-LD](https://i6eal.de/data/catalog/dcat.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON-LD](json-ld/i6eal-open-ai-data-api-dcat.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Examples](examples/i6eal-open-ai-data-api-examples.yml)
- [Data Model](data-model/i6eal-open-ai-data-api-data-model.yml)

### i6eal Open AI Data API Catalogue API

Machine-readable index of every published dataset.

- **Human URL:** [https://i6eal.de/en/tools/data/](https://i6eal.de/en/tools/data/)
- **Base URL:** `https://i6eal.de`

#### Tags

- Catalogue

#### Properties

- [OpenAPI](openapi/i6eal-open-ai-data-api-catalogue-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/i6eal-open-ai-data-api-catalogue-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/i6eal-open-ai-data-api-catalogue-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://i6eal.de/en/tools/data/)
- [JSON-LD](https://i6eal.de/data/catalog/dcat.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON-LD](json-ld/i6eal-open-ai-data-api-dcat.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Examples](examples/i6eal-open-ai-data-api-examples.yml)
- [Data Model](data-model/i6eal-open-ai-data-api-data-model.yml)

### i6eal Open AI Data API EU AI Medical-Device Lifecycle Monitor API

Exact AI text evidence from the public EUDAMED software corpus with manufacturer, risk, version and registry attributes; software alone is never treated as AI evidence.

- **Human URL:** [https://i6eal.de/en/tools/data/](https://i6eal.de/en/tools/data/)
- **Base URL:** `https://i6eal.de`

#### Tags

- EU AI Medical-Device Lifecycle Monitor

#### Properties

- [OpenAPI](openapi/i6eal-open-ai-data-api-eu-ai-medical-device-lifecycle-monitor-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/i6eal-open-ai-data-api-eu-ai-medical-device-lifecycle-monitor-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/i6eal-open-ai-data-api-eu-ai-medical-device-lifecycle-monitor-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://i6eal.de/en/tools/data/)
- [JSON-LD](https://i6eal.de/data/catalog/dcat.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON-LD](json-ld/i6eal-open-ai-data-api-dcat.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Examples](examples/i6eal-open-ai-data-api-examples.yml)
- [Data Model](data-model/i6eal-open-ai-data-api-data-model.yml)

### i6eal Open AI Data API EU AI Studies Monitor API

Official CTIS lifecycles of medicinal clinical trials with exact AI text evidence and separate application, country-status, recruitment, safety and results events.

- **Human URL:** [https://i6eal.de/en/tools/data/](https://i6eal.de/en/tools/data/)
- **Base URL:** `https://i6eal.de`

#### Tags

- EU AI Studies Monitor

#### Properties

- [OpenAPI](openapi/i6eal-open-ai-data-api-eu-ai-studies-monitor-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/i6eal-open-ai-data-api-eu-ai-studies-monitor-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/i6eal-open-ai-data-api-eu-ai-studies-monitor-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://i6eal.de/en/tools/data/)
- [JSON-LD](https://i6eal.de/data/catalog/dcat.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON-LD](json-ld/i6eal-open-ai-data-api-dcat.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Examples](examples/i6eal-open-ai-data-api-examples.yml)
- [Data Model](data-model/i6eal-open-ai-data-api-data-model.yml)

### i6eal Open AI Data API EU AI Transparency Evidence Monitor API

Provider and document evidence for Articles 50 and 53; visibility and review progress remain explicitly separate from conformity.

- **Human URL:** [https://i6eal.de/en/tools/data/](https://i6eal.de/en/tools/data/)
- **Base URL:** `https://i6eal.de`

#### Tags

- EU AI Transparency Evidence Monitor

#### Properties

- [OpenAPI](openapi/i6eal-open-ai-data-api-eu-ai-transparency-evidence-monitor-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/i6eal-open-ai-data-api-eu-ai-transparency-evidence-monitor-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/i6eal-open-ai-data-api-eu-ai-transparency-evidence-monitor-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://i6eal.de/en/tools/data/)
- [JSON-LD](https://i6eal.de/data/catalog/dcat.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON-LD](json-ld/i6eal-open-ai-data-api-dcat.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Examples](examples/i6eal-open-ai-data-api-examples.yml)
- [Data Model](data-model/i6eal-open-ai-data-api-data-model.yml)

### i6eal Open AI Data API EU Platform Automation Monitor API

Monthly DSA statements on automated detection, decision automation and reported restrictions by platform; automation is not relabelled as AI.

- **Human URL:** [https://i6eal.de/en/tools/data/](https://i6eal.de/en/tools/data/)
- **Base URL:** `https://i6eal.de`

#### Tags

- EU Platform Automation Monitor

#### Properties

- [OpenAPI](openapi/i6eal-open-ai-data-api-eu-platform-automation-monitor-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/i6eal-open-ai-data-api-eu-platform-automation-monitor-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/i6eal-open-ai-data-api-eu-platform-automation-monitor-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://i6eal.de/en/tools/data/)
- [JSON-LD](https://i6eal.de/data/catalog/dcat.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON-LD](json-ld/i6eal-open-ai-data-api-dcat.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Examples](examples/i6eal-open-ai-data-api-examples.yml)
- [Data Model](data-model/i6eal-open-ai-data-api-data-model.yml)

### i6eal Open AI Data API German AI Case-Law Monitor API

Observed official federal corpus with decisions, exact passages and a material-change chronicle.

- **Human URL:** [https://i6eal.de/en/tools/data/](https://i6eal.de/en/tools/data/)
- **Base URL:** `https://i6eal.de`

#### Tags

- German AI Case-Law Monitor

#### Properties

- [OpenAPI](openapi/i6eal-open-ai-data-api-german-ai-case-law-monitor-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/i6eal-open-ai-data-api-german-ai-case-law-monitor-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/i6eal-open-ai-data-api-german-ai-case-law-monitor-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://i6eal.de/en/tools/data/)
- [JSON-LD](https://i6eal.de/data/catalog/dcat.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON-LD](json-ld/i6eal-open-ai-data-api-dcat.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Examples](examples/i6eal-open-ai-data-api-examples.yml)
- [Data Model](data-model/i6eal-open-ai-data-api-data-model.yml)

### i6eal Open AI Data API German AI Evidence Network API

Source-evidenced edges between actors, projects, outputs, systems, repositories, packages, procurements and budget titles.

- **Human URL:** [https://i6eal.de/en/tools/data/](https://i6eal.de/en/tools/data/)
- **Base URL:** `https://i6eal.de`

#### Tags

- German AI Evidence Network

#### Properties

- [OpenAPI](openapi/i6eal-open-ai-data-api-german-ai-evidence-network-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/i6eal-open-ai-data-api-german-ai-evidence-network-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/i6eal-open-ai-data-api-german-ai-evidence-network-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://i6eal.de/en/tools/data/)
- [JSON-LD](https://i6eal.de/data/catalog/dcat.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON-LD](json-ld/i6eal-open-ai-data-api-dcat.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Examples](examples/i6eal-open-ai-data-api-examples.yml)
- [Data Model](data-model/i6eal-open-ai-data-api-data-model.yml)

### i6eal Open AI Data API German & EU AI Adoption Atlas API

Official Eurostat observations of AI adoption by enterprises and individuals; statistical universes remain separate.

- **Human URL:** [https://i6eal.de/en/tools/data/](https://i6eal.de/en/tools/data/)
- **Base URL:** `https://i6eal.de`

#### Tags

- German & EU AI Adoption Atlas

#### Properties

- [OpenAPI](openapi/i6eal-open-ai-data-api-german-eu-ai-adoption-atlas-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/i6eal-open-ai-data-api-german-eu-ai-adoption-atlas-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/i6eal-open-ai-data-api-german-eu-ai-adoption-atlas-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://i6eal.de/en/tools/data/)
- [JSON-LD](https://i6eal.de/data/catalog/dcat.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON-LD](json-ld/i6eal-open-ai-data-api-dcat.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Examples](examples/i6eal-open-ai-data-api-examples.yml)
- [Data Model](data-model/i6eal-open-ai-data-api-data-model.yml)

### i6eal Open AI Data API German & EU AI Procurement Chronicle API

Official procurement signals as durable procedure chains, separating exactly linked procedures from isolated notices.

- **Human URL:** [https://i6eal.de/en/tools/data/](https://i6eal.de/en/tools/data/)
- **Base URL:** `https://i6eal.de`

#### Tags

- German & EU AI Procurement Chronicle

#### Properties

- [OpenAPI](openapi/i6eal-open-ai-data-api-german-eu-ai-procurement-chronicle-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/i6eal-open-ai-data-api-german-eu-ai-procurement-chronicle-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/i6eal-open-ai-data-api-german-eu-ai-procurement-chronicle-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://i6eal.de/en/tools/data/)
- [JSON-LD](https://i6eal.de/data/catalog/dcat.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON-LD](json-ld/i6eal-open-ai-data-api-dcat.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Examples](examples/i6eal-open-ai-data-api-examples.yml)
- [Data Model](data-model/i6eal-open-ai-data-api-data-model.yml)

### i6eal Open AI Data API German & EU AI Standardisation Monitor API

Standardisation request, work items, lifecycle events and EU references as separate inspectable evidence lanes.

- **Human URL:** [https://i6eal.de/en/tools/data/](https://i6eal.de/en/tools/data/)
- **Base URL:** `https://i6eal.de`

#### Tags

- German & EU AI Standardisation Monitor

#### Properties

- [OpenAPI](openapi/i6eal-open-ai-data-api-german-eu-ai-standardisation-monitor-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/i6eal-open-ai-data-api-german-eu-ai-standardisation-monitor-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/i6eal-open-ai-data-api-german-eu-ai-standardisation-monitor-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://i6eal.de/en/tools/data/)
- [JSON-LD](https://i6eal.de/data/catalog/dcat.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON-LD](json-ld/i6eal-open-ai-data-api-dcat.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Examples](examples/i6eal-open-ai-data-api-examples.yml)
- [Data Model](data-model/i6eal-open-ai-data-api-data-model.yml)

### i6eal Open AI Data API German & EU AI Supervision Monitor API

Officially evidenced responsibilities, legal instruments and observations, without a compliance or effectiveness score.

- **Human URL:** [https://i6eal.de/en/tools/data/](https://i6eal.de/en/tools/data/)
- **Base URL:** `https://i6eal.de`

#### Tags

- German & EU AI Supervision Monitor

#### Properties

- [OpenAPI](openapi/i6eal-open-ai-data-api-german-eu-ai-supervision-monitor-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/i6eal-open-ai-data-api-german-eu-ai-supervision-monitor-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/i6eal-open-ai-data-api-german-eu-ai-supervision-monitor-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://i6eal.de/en/tools/data/)
- [JSON-LD](https://i6eal.de/data/catalog/dcat.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON-LD](json-ld/i6eal-open-ai-data-api-dcat.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Examples](examples/i6eal-open-ai-data-api-examples.yml)
- [Data Model](data-model/i6eal-open-ai-data-api-data-model.yml)

### i6eal Open AI Data API German Federal AI Budget Monitor API

Machine-readable federal budget titles with explicit AI references, keeping appropriations, supplements, actuals and official revisions separate.

- **Human URL:** [https://i6eal.de/en/tools/data/](https://i6eal.de/en/tools/data/)
- **Base URL:** `https://i6eal.de`

#### Tags

- German Federal AI Budget Monitor

#### Properties

- [OpenAPI](openapi/i6eal-open-ai-data-api-german-federal-ai-budget-monitor-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/i6eal-open-ai-data-api-german-federal-ai-budget-monitor-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/i6eal-open-ai-data-api-german-federal-ai-budget-monitor-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://i6eal.de/en/tools/data/)
- [JSON-LD](https://i6eal.de/data/catalog/dcat.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON-LD](json-ld/i6eal-open-ai-data-api-dcat.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Examples](examples/i6eal-open-ai-data-api-examples.yml)
- [Data Model](data-model/i6eal-open-ai-data-api-data-model.yml)

### i6eal Open AI Data API German State AI Evidence Layers API

State dossiers assembled from three separate evidence layers: infrastructure, public systems and procurement signals.

- **Human URL:** [https://i6eal.de/en/tools/data/](https://i6eal.de/en/tools/data/)
- **Base URL:** `https://i6eal.de`

#### Tags

- German State AI Evidence Layers

#### Properties

- [OpenAPI](openapi/i6eal-open-ai-data-api-german-state-ai-evidence-layers-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/i6eal-open-ai-data-api-german-state-ai-evidence-layers-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/i6eal-open-ai-data-api-german-state-ai-evidence-layers-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://i6eal.de/en/tools/data/)
- [JSON-LD](https://i6eal.de/data/catalog/dcat.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON-LD](json-ld/i6eal-open-ai-data-api-dcat.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Examples](examples/i6eal-open-ai-data-api-examples.yml)
- [Data Model](data-model/i6eal-open-ai-data-api-data-model.yml)

### i6eal Open AI Data API Observed AI Procurement Changes API

Revision trail for newly published and materially changed procedure dossiers; retrieval timestamps alone never create an event.

- **Human URL:** [https://i6eal.de/en/tools/data/](https://i6eal.de/en/tools/data/)
- **Base URL:** `https://i6eal.de`

#### Tags

- Observed AI Procurement Changes

#### Properties

- [OpenAPI](openapi/i6eal-open-ai-data-api-observed-ai-procurement-changes-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/i6eal-open-ai-data-api-observed-ai-procurement-changes-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/i6eal-open-ai-data-api-observed-ai-procurement-changes-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://i6eal.de/en/tools/data/)
- [JSON-LD](https://i6eal.de/data/catalog/dcat.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON-LD](json-ld/i6eal-open-ai-data-api-dcat.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Examples](examples/i6eal-open-ai-data-api-examples.yml)
- [Data Model](data-model/i6eal-open-ai-data-api-data-model.yml)

### i6eal Open AI Data API Public AI System Evidence Pass API

Inspectable system profiles and source-evidenced links to repositories and technical inventories only.

- **Human URL:** [https://i6eal.de/en/tools/data/](https://i6eal.de/en/tools/data/)
- **Base URL:** `https://i6eal.de`

#### Tags

- Public AI System Evidence Pass

#### Properties

- [OpenAPI](openapi/i6eal-open-ai-data-api-public-ai-system-evidence-pass-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/i6eal-open-ai-data-api-public-ai-system-evidence-pass-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/i6eal-open-ai-data-api-public-ai-system-evidence-pass-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://i6eal.de/en/tools/data/)
- [JSON-LD](https://i6eal.de/data/catalog/dcat.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON-LD](json-ld/i6eal-open-ai-data-api-dcat.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Examples](examples/i6eal-open-ai-data-api-examples.yml)
- [Data Model](data-model/i6eal-open-ai-data-api-data-model.yml)

## Common Properties

- [M C P Server](mcp/i6eal-open-ai-data-api-mcp.yml)
- [Domain Security](security/i6eal-open-ai-data-api-domain-security.yml)
- [Website](https://i6eal.de/)
- [Developer Portal](https://i6eal.de/en/tools/data/)
- [Documentation](https://i6eal.de/en/tools/data/)
- [API Reference](https://i6eal.de/openapi.json)
- [Support](https://i6eal.de/kontakt/)
- [Blog](https://i6eal.de/newsroom/)
- [GitHub Organization](https://github.com/i6eal)
- [Terms of Service](https://i6eal.de/nutzungsbedingungen/)
- [Privacy Policy](https://i6eal.de/datenschutz/)
- [License](https://i6eal.de/tools/daten/)
- [About](https://i6eal.de/ueber-uns/)
- [L L Ms Txt](llms/i6eal-open-ai-data-api-llms.txt)
- [Authentication](authentication/i6eal-open-ai-data-api-authentication.yml)
- [Conventions](conventions/i6eal-open-ai-data-api-conventions.yml)
- [Error Catalog](errors/i6eal-open-ai-data-api-problem-types.yml)
- [Lifecycle](lifecycle/i6eal-open-ai-data-api-lifecycle.yml)
- [Conformance](conformance/i6eal-open-ai-data-api-conformance.yml)
- [Data Model](data-model/i6eal-open-ai-data-api-data-model.yml)
- [Examples](examples/i6eal-open-ai-data-api-examples.yml)
- [Packages](packages/i6eal-open-ai-data-api-packages.yml)
- [Overlay](overlays/i6eal-open-ai-data-api-overlay.yaml)
- [Agent Skill](skills/_index.yml)

## Maintainers

**FN:** i6eal
**Email:** ai@i6eal.de
**URL:** https://i6eal.de/kontakt/
