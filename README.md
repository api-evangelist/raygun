# Raygun

Raygun is an application monitoring platform that combines **Crash Reporting**, **Real User Monitoring (RUM)**, and **Application Performance Monitoring (APM)** into a single observability product for web, mobile, and server applications. This repository is an API Evangelist profile of the Raygun developer surface — based on the publicly published OpenAPI 3.0 specification at [api.raygun.io](https://api.raygun.io/v3/swagger/index.html) plus the per-product documentation, ingestion endpoints, and the MindscapeHQ GitHub organization.

- **Provider portal:** https://raygun.com
- **API specifications (Swagger):** https://api.raygun.io/v3/swagger/index.html
- **Public v3 base URL:** `https://api.raygun.com/v3`
- **Crash ingestion endpoint:** `POST https://api.raygun.com/entries`
- **GitHub org:** https://github.com/MindscapeHQ
- **Status page:** https://status.raygun.com
- **Changelog:** https://raygun.com/changelog
- **Pricing:** https://raygun.com/pricing

## APIs

This profile catalogs **14 APIs** across the Raygun surface.

### Public v3 API (Personal Access Token, bearer)

| API | Operations | OpenAPI |
|---|---|---|
| Raygun Applications API | 4 | [openapi/raygun-applications-api-openapi.yml](openapi/raygun-applications-api-openapi.yml) |
| Raygun Errors API | 12 | [openapi/raygun-errors-api-openapi.yml](openapi/raygun-errors-api-openapi.yml) |
| Raygun Deployments API | 10 | [openapi/raygun-deployments-api-openapi.yml](openapi/raygun-deployments-api-openapi.yml) |
| Raygun Source Maps API | 6 | [openapi/raygun-source-maps-api-openapi.yml](openapi/raygun-source-maps-api-openapi.yml) |
| Raygun Sessions API | 2 | [openapi/raygun-sessions-api-openapi.yml](openapi/raygun-sessions-api-openapi.yml) |
| Raygun Pages API | 2 | [openapi/raygun-pages-api-openapi.yml](openapi/raygun-pages-api-openapi.yml) |
| Raygun Customers API | 2 | [openapi/raygun-customers-api-openapi.yml](openapi/raygun-customers-api-openapi.yml) |
| Raygun Metrics API | 3 | [openapi/raygun-metrics-api-openapi.yml](openapi/raygun-metrics-api-openapi.yml) |
| Raygun Flutter Symbols API | 5 | [openapi/raygun-flutter-symbols-api-openapi.yml](openapi/raygun-flutter-symbols-api-openapi.yml) |
| Raygun Teams API | 2 | [openapi/raygun-teams-api-openapi.yml](openapi/raygun-teams-api-openapi.yml) |
| Raygun Invitations API | 4 | [openapi/raygun-invitations-api-openapi.yml](openapi/raygun-invitations-api-openapi.yml) |
| Raygun Plans API | 1 | [openapi/raygun-plans-api-openapi.yml](openapi/raygun-plans-api-openapi.yml) |

A consolidated copy of the full Raygun OpenAPI 3.0 specification (all 53 operations across 12 tags) is at [openapi/raygun-public-api-openapi.yml](openapi/raygun-public-api-openapi.yml).

### Ingestion and legacy APIs

| API | Auth | Endpoint |
|---|---|---|
| Raygun Crash Reporting Ingestion API | `X-ApiKey` | `POST https://api.raygun.com/entries` |
| Raygun Pulse RUM API (Legacy) | `X-SessionKey` (15-min TTL) | `GET https://api.raygun.com/api/v1/pulse/*` |

## Naftiko Capabilities

Per-tag Naftiko capabilities are in [capabilities/](capabilities/). Each defines a `consumes` block bound to the Raygun v3 endpoint with bearer-token auth, a REST `exposes` adapter prefixed with `/v3`, and an MCP adapter with one tool per operation.

- `applications-applications.yaml` (4 ops)
- `errors-errors.yaml` (12 ops)
- `deployments-deployments.yaml` (10 ops)
- `source-maps-source-maps.yaml` (6 ops)
- `sessions-sessions.yaml` (2 ops)
- `pages-pages.yaml` (2 ops)
- `customers-customers.yaml` (2 ops)
- `metrics-metrics.yaml` (3 ops)
- `flutter-symbols-flutter-symbols.yaml` (5 ops)
- `teams-teams.yaml` (2 ops)
- `invitations-invitations.yaml` (4 ops)
- `plans-plans.yaml` (1 op)

## Commercial Surface

| Artifact | Purpose |
|---|---|
| [plans/raygun-plans-pricing.yml](plans/raygun-plans-pricing.yml) | API Commons Plans 0.1 — tiered plans for Crash Reporting, RUM, APM plus on-demand overages |
| [rate-limits/raygun-rate-limits.yml](rate-limits/raygun-rate-limits.yml) | API Commons Rate Limits 0.1 — v3 token limits, ingestion 128 KB payload cap, Pulse 50/day quota |
| [finops/raygun-finops.yml](finops/raygun-finops.yml) | FOCUS 1.3 / FinOps Framework alignment — events as the primary meter |

## Schemas, Linked Data, and Examples

- [json-schema/raygun-error-group-schema.json](json-schema/raygun-error-group-schema.json) — Error group plus the inbound crash-reporting payload schema (occurredOn + details).
- [json-schema/raygun-deployment-schema.json](json-schema/raygun-deployment-schema.json) — Deployment resource and SCM linkage fields.
- [json-ld/raygun-context.jsonld](json-ld/raygun-context.jsonld) — JSON-LD context mapping Raygun's core entities (Application, ErrorGroup, ErrorInstance, Deployment, SourceMap, Session, Page, Customer, Team, Plan, Invitation, FlutterSymbol) onto schema.org.
- [examples/raygun-crash-report-example.json](examples/raygun-crash-report-example.json) — Sample POST /entries payload with stack trace, breadcrumbs, environment, and user data.
- [examples/raygun-error-group-example.json](examples/raygun-error-group-example.json) — Sample error-group response.
- [examples/raygun-create-deployment-example.json](examples/raygun-create-deployment-example.json) — Sample deployment-create payload with SCM linkage.

## Governance

- [rules/raygun-rules.yml](rules/raygun-rules.yml) — Spectral ruleset enforcing Raygun conventions (kebab-case paths and operationIds, Title Case summaries, bearer auth, problem-details 4xx responses, 429 documentation).
- [vocabulary/raygun-vocabulary.yml](vocabulary/raygun-vocabulary.yml) — Raygun operational vocabulary covering applications, error groups, deployments, source maps, sessions, customers, plans, AI Error Resolution, spike protection, and inbound filters.

## SDKs and Tooling (MindscapeHQ)

| Repository | Language |
|---|---|
| [raygun4js](https://github.com/MindscapeHQ/raygun4js) | JavaScript |
| [raygun4net](https://github.com/MindscapeHQ/raygun4net) | C# / .NET |
| [raygun4node](https://github.com/MindscapeHQ/raygun4node) | Node.js / TypeScript |
| [raygun4python](https://github.com/MindscapeHQ/raygun4python) | Python |
| [raygun4ruby](https://github.com/MindscapeHQ/raygun4ruby) | Ruby |
| [raygun4php](https://github.com/MindscapeHQ/raygun4php) | PHP |
| [raygun4android](https://github.com/MindscapeHQ/raygun4android) | Kotlin / Android |
| [raygun4flutter](https://github.com/MindscapeHQ/raygun4flutter) | Dart / Flutter |
| [raygun4reactnative](https://github.com/MindscapeHQ/raygun4reactnative) | TypeScript / React Native |
| [raygun4maui](https://github.com/MindscapeHQ/raygun4maui) | .NET MAUI |
| [raygun4blazor](https://github.com/MindscapeHQ/raygun4blazor) | .NET Blazor |
| [raygun-cli](https://github.com/MindscapeHQ/raygun-cli) | Dart CLI |
| [raygun4node-aws-lambda](https://github.com/MindscapeHQ/raygun4node-aws-lambda) | AWS Lambda wrapper |
| [ember-cli-raygun](https://github.com/MindscapeHQ/ember-cli-raygun) | Ember add-on |

## Authentication Reference

| Surface | Header | Token |
|---|---|---|
| Public v3 API | `Authorization: Bearer <token>` | Personal Access Token |
| Crash ingestion (`/entries`) | `X-ApiKey: <key>` | Per-application API key |
| Pulse RUM (legacy) | `X-SessionKey: <key>` + `X-ApiKey: <key>` | Session key issued via OAuth-style Client ID/Secret exchange (15 min TTL) |

## Tier

**Tier-1** — Raygun publishes a real OpenAPI 3.0.3 specification (130 KB, 53 operations) at `https://api.raygun.io/v3/raygun-openapi-spec.json` with full schema definitions, parameter contracts, and a documented bearer-token security scheme.
