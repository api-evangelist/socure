# socure (socure)

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
