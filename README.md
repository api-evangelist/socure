# Socure (socure)
Socure is the leading vertically-integrated digital identity verification and fraud-prevention platform, used by 3,000+ banks, fintechs, crypto exchanges, marketplaces, gaming operators, and public-sector agencies. The ID+ API exposes Socure's KYC, document verification (DocV), Sigma fraud models, RiskScore (email / phone / address), Global Watchlist screening, Deceased Check, eCBSV, Digital Intelligence (SigmaDevice), Graph Intelligence, Account Intelligence, Prefill, and Decision modules through a single multi-module REST call, complemented by the RiskOS orchestration platform, native mobile SDKs, and webhook event streams. Socure is headquartered in Incline Village, Nevada with origins in New York City.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/socure/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

- Identity Verification, Fraud Prevention, KYC, AML, Compliance, Watchlist, Document Verification, Biometrics, Decisioning, Bank Account Verification, Account Validation, Open Banking, Orchestration, Workflows

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Socure ID+ API
Unified multi-module REST surface. Submit a `modules` array — `kyc`, `ecbsv`, `sigma`, `synthetic`, `emailrisk`, `phonerisk`, `addressrisk`, `decision`, `watchlist`, `decasedcheck`, `devicerisk`, `graphintelligence`, `accountintelligence`, `prefill`, `docvtransaction` — in one POST and receive the combined response with `referenceId`, module result blocks, and an optional `decision` block.

**Human URL:** [https://developer.socure.com/reference/idplus](https://developer.socure.com/reference/idplus)

- [Documentation — API Reference](https://developer.socure.com/reference/idplus)
- [Documentation — API Endpoints](https://developer.socure.com/docs/id-plus/endpoints-and-apis/api-endpoints)
- [Documentation — Authentication](https://developer.socure.com/reference/authentication)
- [OpenAPI](openapi/socure-idplus-api-openapi.yml)
- [JSON Schema — Request](json-schema/socure-idplus-request-schema.json)
- [JSON Schema — Response](json-schema/socure-idplus-response-schema.json)
- [JSON-LD](json-ld/socure-context.jsonld)
- [Naftiko Capability — Identity Verification (KYC)](capabilities/idplus-identity-verification.yaml)
- [Naftiko Capability — Fraud Scoring](capabilities/idplus-fraud-scoring.yaml)
- [Naftiko Capability — Watchlist Screening](capabilities/idplus-watchlist-screening.yaml)

### Socure Predictive DocV API
Document Verification with biometric face match and liveness. Session-orchestrated REST API for creating transactions, uploading documents/selfies, and retrieving decisions, plus a webhook stream (`APP_OPENED`, `DOCUMENTS_UPLOADED`, `VERIFICATION_COMPLETED`, `SESSION_EXPIRED`) for asynchronous notifications.

**Human URL:** [https://developer.socure.com/docs/id-plus/modules/docv/docv-overview](https://developer.socure.com/docs/id-plus/modules/docv/docv-overview)

- [Documentation — DocV Overview](https://developer.socure.com/docs/id-plus/modules/docv/docv-overview)
- [Documentation — DocV Webhook Events](https://developer.socure.com/docs/webhooks/docv-events)
- [OpenAPI](openapi/socure-docv-api-openapi.yml)
- [AsyncAPI — DocV Webhooks](asyncapi/socure-docv-asyncapi.yml)
- [Naftiko Capability — Document Verification](capabilities/docv-document-verification.yaml)

### Socure Global Watchlist Monitoring API
Continuous monitoring of customer identities against sanctions (OFAC, UN, EU, HMT, DFAT), PEP, and adverse media lists with webhook alerts on new and updated matches.

**Human URL:** [https://developer.socure.com/docs/id-plus/modules/global-watchlist/configuration/watchlist-monitoring-overview](https://developer.socure.com/docs/id-plus/modules/global-watchlist/configuration/watchlist-monitoring-overview)

- [Documentation — Global Watchlist Overview](https://developer.socure.com/docs/id-plus/modules/global-watchlist/global-watchlist-overview)
- [Documentation — Watchlist Monitoring Webhooks](https://developer.socure.com/docs/id-plus/modules/global-watchlist/configuration/watchlist-monitoring-overview)
- [OpenAPI](openapi/socure-watchlist-monitoring-api-openapi.yml)
- [AsyncAPI — Watchlist Monitoring Webhooks](asyncapi/socure-watchlist-asyncapi.yml)
- [Naftiko Capability — Watchlist Monitoring](capabilities/watchlist-monitoring.yaml)

### Socure Decision API
Rule-based decisioning returning a deterministic accept/reject/review/refer/resubmit outcome derived from ID+ module scores and customer-configured rules authored in the Socure Console.

**Human URL:** [https://developer.socure.com/docs/id-plus/modules/decision](https://developer.socure.com/docs/id-plus/modules/decision)

- [OpenAPI](openapi/socure-decision-api-openapi.yml)
- [Naftiko Capability — Decisioning](capabilities/decision-decisioning.yaml)

### Socure Account Intelligence API
Real-time validation of US bank accounts — open/closed status, ownership name match, and account type signals — without micro-deposits or credentials.

**Human URL:** [https://developer.socure.com/docs/id-plus/modules/account-intelligence](https://developer.socure.com/docs/id-plus/modules/account-intelligence)

- [OpenAPI](openapi/socure-account-intelligence-api-openapi.yml)
- [Naftiko Capability — Bank Account Validation](capabilities/account-intelligence.yaml)

### Socure RiskOS API
Identity and fraud orchestration platform combining ID+ modules, customer-configured workflows, case management, and a no-code rules editor. RiskOS Enterprise (custom) and RiskOS Launch (self-serve) deployment models. The RiskOS API surface is gated behind customer onboarding; this profile tracks the documentation entry point.

**Human URL:** [https://help.socure.com/riskos/docs](https://help.socure.com/riskos/docs)

## Common Properties

- [Portal — socure.com](https://www.socure.com)
- [Portal — Socure DevHub](https://developer.socure.com)
- [Documentation — DevHub Docs](https://developer.socure.com/docs)
- [Documentation — API Reference](https://developer.socure.com/reference)
- [Documentation — GovCloud DevHub](https://developer.socure.us)
- [Documentation — RiskOS](https://help.socure.com/riskos/docs)
- [GettingStarted — ID+](https://developer.socure.com/docs/id-plus/getting-started)
- [GettingStarted — Quick Start Guide](https://developer.socure.com/docs/id-plus/getting-started/quick-start-guide)
- [Authentication](https://developer.socure.com/reference/authentication)
- [ProductsPage](https://www.socure.com/products)
- [Pricing](https://www.socure.com/pricing)
- [AboutUs](https://www.socure.com/company/about)
- [ContactUs](https://www.socure.com/company/contact)
- [Blog](https://www.socure.com/blog)
- [Blog — News](https://www.socure.com/news)
- [ResourceCenter](https://www.socure.com/resources)
- [CaseStudies — Customer Stories](https://www.socure.com/customers)
- [PrivacyPolicy](https://www.socure.com/legal/privacy-policy)
- [TermsOfService](https://www.socure.com/legal/terms)
- [TrustCenter](https://trust.socure.com)
- [StatusPage](https://status.socure.com)
- [Careers](https://www.socure.com/careers)
- [GitHubOrganization](https://github.com/socure-inc)
- [SDK — DocV iOS](https://github.com/socure-inc/socure-docv-sdk-ios)
- [SDK — DocV Android](https://github.com/socure-inc/socure-docv-sdk-android)
- [SDK — DocV React Native Demo](https://github.com/socure-inc/socure-docv-demo-app-react-native)
- [SDK — SigmaDevice iOS](https://github.com/socure-inc/socure-sigmadevice-sdk-ios)
- [SDK — SigmaDevice Android](https://github.com/socure-inc/socure-sigmadevice-sdk-android)
- [SDK — SigmaDevice React Native Demo](https://github.com/socure-inc/socure-sigmadevice-demo-app-react-native)
- [Tool — RiskOS Integration Skill](https://github.com/socure-inc/riskos-integration-skill)
- [Webhooks — DocV](https://developer.socure.com/docs/webhooks/docv-events)
- [Support — Help Center](https://help.socure.com)
- [LinkedIn](https://www.linkedin.com/company/socure-inc-)
- [Twitter](https://twitter.com/socure)
- [YouTube](https://www.youtube.com/c/Socure)

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Socure ID+ API](openapi/socure-idplus-api-openapi.yml)
- [Socure Predictive DocV API](openapi/socure-docv-api-openapi.yml)
- [Socure Global Watchlist Monitoring API](openapi/socure-watchlist-monitoring-api-openapi.yml)
- [Socure Decision API](openapi/socure-decision-api-openapi.yml)
- [Socure Account Intelligence API](openapi/socure-account-intelligence-api-openapi.yml)

### AsyncAPI

- [Socure DocV Webhooks](asyncapi/socure-docv-asyncapi.yml)
- [Socure Watchlist Monitoring Webhooks](asyncapi/socure-watchlist-asyncapi.yml)

### JSON Schema

- [Socure ID+ Request](json-schema/socure-idplus-request-schema.json)
- [Socure ID+ Response](json-schema/socure-idplus-response-schema.json)

### JSON Structure

- [Socure ID+ Structure](json-structure/socure-idplus-structure.json)

### JSON-LD

- [Socure Context](json-ld/socure-context.jsonld)

### Examples

- [ID+ KYC Request and Response](examples/socure-idplus-kyc-example.json)
- [DocV Create Transaction](examples/socure-docv-create-transaction-example.json)
- [DocV Webhook Event](examples/socure-docv-webhook-example.json)

### Capabilities (Naftiko)

- [ID+ Identity Verification (KYC)](capabilities/idplus-identity-verification.yaml)
- [ID+ Fraud Scoring](capabilities/idplus-fraud-scoring.yaml)
- [ID+ Watchlist Screening](capabilities/idplus-watchlist-screening.yaml)
- [Predictive DocV — Document Verification](capabilities/docv-document-verification.yaml)
- [Global Watchlist Monitoring](capabilities/watchlist-monitoring.yaml)
- [Decision — Decisioning](capabilities/decision-decisioning.yaml)
- [Account Intelligence — Bank Account Validation](capabilities/account-intelligence.yaml)

### Vocabulary

- [Socure Vocabulary](vocabulary/socure-vocabulary.yml)

### Spectral Rules

- [Socure API Style Ruleset](rules/socure-rules.yml)

### Commercial artifacts

- [Plans / Pricing](plans/socure-plans-pricing.yml)
- [Rate Limits](rate-limits/socure-rate-limits.yml)
- [FinOps Definition](finops/socure-finops.yml)

## Maintainers

**FN:** Kin Lane

**Email:** info@apievangelist.com
