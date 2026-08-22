# socure (socure)

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

Socure is the leading vertically-integrated digital identity verification and fraud-prevention platform, used by 3,000+ banks, fintechs, crypto exchanges, marketplaces, gaming operators, and public-sector agencies. The ID+ API exposes Socure's KYC, document verification (DocV), Sigma fraud models, RiskScore (email / phone / address), Global Watchlist screening, Deceased Check, eCBSV, Digital Intelligence (SigmaDevice), Graph Intelligence, Account Intelligence, Prefill, and Decision modules through a single multi-module REST call, complemented by the RiskOS orchestration platform, native mobile SDKs, and webhook event streams. Socure is headquartered in Incline Village, Nevada with origins in New York City.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/socure/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/socure/refs/heads/main/apis.yml)

## Scope

- **Position:** Consuming

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Socure ID+ API

The Socure ID+ API is the unified REST surface for the ID+ platform, exposing every module — KYC (Socure Verify), eCBSV, Sigma Identity Fraud, Sigma Synthetic, Sigma First-Party Fraud, Email/Phone/Address RiskScore, Digital Intelligence, Graph Intelligence, Global Watchlist Screening, Deceased Check, Account Intelligence, Prefill, and the Decision rules engine — through a single multi-module POST that returns a combined response with referenceId, decision, KYC, fraud, and risk score blocks.

- **Human URL:** [https://developer.socure.com/reference/idplus](https://developer.socure.com/reference/idplus)

#### Tags

- Identity Verification
- Fraud Prevention
- KYC
- Compliance
- AML

#### Properties

- [Documentation](https://developer.socure.com/reference/idplus)
- [Documentation](https://developer.socure.com/docs/id-plus/endpoints-and-apis/api-endpoints)
- [Documentation](https://developer.socure.com/reference/authentication)
- [OpenAPI](openapi/socure-idplus-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/socure-idplus-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/socure-idplus-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/socure-idplus-request-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/socure-idplus-response-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/socure-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Socure Predictive DocV API

Predictive Document Verification (DocV) verifies government-issued ID documents and matches them to a live selfie with liveness detection. Includes a session-orchestration REST API (create transaction, retrieve decision, manage uploads) and a webhook stream (`APP_OPENED`, `DOCUMENTS_UPLOADED`, `VERIFICATION_COMPLETED`, `SESSION_EXPIRED`) for asynchronous notification of session lifecycle events.

- **Human URL:** [https://developer.socure.com/docs/id-plus/modules/docv/docv-overview](https://developer.socure.com/docs/id-plus/modules/docv/docv-overview)

#### Tags

- Identity Verification
- Document Verification
- Biometrics
- Liveness

#### Properties

- [Documentation](https://developer.socure.com/docs/id-plus/modules/docv/docv-overview)
- [Documentation](https://developer.socure.com/docs/webhooks/docv-events)
- [OpenAPI](openapi/socure-docv-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/socure-docv-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/socure-docv-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/socure-docv-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)

### Socure Global Watchlist Monitoring API

Continuous monitoring of customers against global sanctions lists (OFAC, UN, EU, HMT, DFAT), PEP lists, and adverse media. Submit profiles for ongoing screening, retrieve match alerts, manage match dispositions, and receive webhook callbacks when a customer matches a newly added or updated list entry.

- **Human URL:** [https://developer.socure.com/docs/id-plus/modules/global-watchlist/configuration/watchlist-monitoring-overview](https://developer.socure.com/docs/id-plus/modules/global-watchlist/configuration/watchlist-monitoring-overview)

#### Tags

- AML
- Compliance
- Watchlist
- Sanctions
- PEP

#### Properties

- [Documentation](https://developer.socure.com/docs/id-plus/modules/global-watchlist/global-watchlist-overview)
- [Documentation](https://developer.socure.com/docs/id-plus/modules/global-watchlist/configuration/watchlist-monitoring-overview)
- [OpenAPI](openapi/socure-watchlist-monitoring-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/socure-watchlist-monitoring-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/socure-watchlist-monitoring-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/socure-watchlist-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)

### Socure Decision API

Socure's rule-based decisioning module returns a single deterministic outcome — accept, reject, review, refer, or resubmit — derived from ID+ module scores and customer-configured rules. Decision rules are authored in the Socure Console and applied on every ID+ call when the `decision.module` block is included in the request modules array.

- **Human URL:** [https://developer.socure.com/docs/id-plus/modules/decision](https://developer.socure.com/docs/id-plus/modules/decision)

#### Tags

- Decisioning
- Rules Engine
- Identity Verification

#### Properties

- [Documentation](https://developer.socure.com/docs/id-plus/modules/decision)
- [OpenAPI](openapi/socure-decision-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/socure-decision-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/socure-decision-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Socure Account Intelligence API

Real-time validation of US bank accounts — verifying open/closed status, ownership (name match), and account-type signals. Powers funding-account checks for fintech onboarding, payroll, and ACH origination flows without requiring micro-deposits or end-user credentials.

- **Human URL:** [https://developer.socure.com/docs/id-plus/modules/account-intelligence](https://developer.socure.com/docs/id-plus/modules/account-intelligence)

#### Tags

- Bank Account Verification
- Account Validation
- Open Banking

#### Properties

- [Documentation](https://developer.socure.com/docs/id-plus/modules/account-intelligence)
- [OpenAPI](openapi/socure-account-intelligence-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/socure-account-intelligence-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/socure-account-intelligence-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Socure RiskOS API

RiskOS is Socure's identity and fraud orchestration platform that combines ID+ modules, customer-configured workflows, case management, and a no-code rules editor under a unified API. RiskOS Enterprise supports custom workflow deployments; RiskOS Launch is the self-serve productized workflow offering. Note - the RiskOS API surface is gated behind customer onboarding; this profile tracks the documentation entry point only.

- **Human URL:** [https://help.socure.com/riskos/docs](https://help.socure.com/riskos/docs)

#### Tags

- Orchestration
- Workflows
- Identity Verification
- Fraud Prevention

#### Properties

- [Documentation](https://help.socure.com/riskos/docs)
- [Postman Collection](collections/socure-account-intelligence-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/socure-account-intelligence-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/socure-decision-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/socure-decision-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/socure-docv-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/socure-docv-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/socure-idplus-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/socure-idplus-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/socure-watchlist-monitoring-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/socure-watchlist-monitoring-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [Portal](https://www.socure.com)
- [Portal](https://developer.socure.com)
- [Documentation](https://developer.socure.com/docs)
- [Documentation](https://developer.socure.com/reference)
- [Getting Started](https://developer.socure.com/docs/id-plus/getting-started)
- [Getting Started](https://developer.socure.com/docs/id-plus/getting-started/quick-start-guide)
- [Authentication](https://developer.socure.com/reference/authentication)
- [Products Page](https://www.socure.com/products)
- [Pricing](https://www.socure.com/pricing)
- [About Us](https://www.socure.com/company/about)
- [Contact Us](https://www.socure.com/company/contact)
- [Blog](https://www.socure.com/blog)
- [Blog](https://www.socure.com/news)
- [Resource Center](https://www.socure.com/resources)
- [Case Studies](https://www.socure.com/customers)
- [Privacy Policy](https://www.socure.com/legal/privacy-policy)
- [Terms of Service](https://www.socure.com/legal/terms)
- [Trust Center](https://trust.socure.com)
- [Status Page](https://status.socure.com)
- [Careers](https://www.socure.com/careers)
- [GitHub Organization](https://github.com/socure-inc)
- [SDK](https://github.com/socure-inc/socure-docv-sdk-ios)
- [SDK](https://github.com/socure-inc/socure-docv-sdk-android)
- [SDK](https://github.com/socure-inc/socure-docv-demo-app-react-native)
- [SDK](https://github.com/socure-inc/socure-sigmadevice-sdk-ios)
- [SDK](https://github.com/socure-inc/socure-sigmadevice-sdk-android)
- [SDK](https://github.com/socure-inc/socure-sigmadevice-demo-app-react-native)
- [Tool](https://github.com/socure-inc/riskos-integration-skill)
- [LinkedIn](https://www.linkedin.com/company/socure-inc-)
- [Twitter](https://twitter.com/socure)
- [YouTube](https://www.youtube.com/c/Socure)
- [Webhooks](https://developer.socure.com/docs/webhooks/docv-events)
- [Support](https://help.socure.com)
- [Documentation](https://help.socure.com/riskos/docs)
- [Documentation](https://developer.socure.us)
- [Plans](plans/socure-plans-pricing.yml)
- [Rate Limits](rate-limits/socure-rate-limits.yml)
- [Fin Ops](finops/socure-finops.yml)
- [Vocabulary](vocabulary/socure-vocabulary.yml)
- [Spectral Rules](rules/socure-rules.yml)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
