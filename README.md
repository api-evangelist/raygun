# Raygun (raygun)

Raygun is an application monitoring platform that combines Crash Reporting, Real User Monitoring (RUM), and Application Performance Monitoring (APM) into a single observability product for web, mobile, and server applications. The Raygun Public API (v3) is a documented OpenAPI 3.0 surface at api.raygun.com/v3 covering applications, error groups, error instances, deployments, source maps, sessions, pages, customers, metrics, Flutter symbols, teams, invitations, and plans — authenticated with a Personal Access Token. A separate ingestion endpoint at api.raygun.com/entries accepts crash payloads from a broad fleet of native SDKs (JavaScript, .NET, Node, Python, Ruby, PHP, Android, Flutter, React Native, MAUI, Blazor) plus the Raygun CLI. Pricing is tiered (Basic, Team, Business, Enterprise) per product with on-demand per-event overages, 14-day free trial, and 180-day error retention.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/apis.yml)

## Scope

- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- Observability
- Crash Reporting
- Real User Monitoring
- Application Performance Monitoring
- Error Tracking
- Errors
- Monitoring
- DevOps
- Source Maps
- Deployments

## Timestamps

- **Created:** 2026-05-25T00:00:00.000Z
- **Modified:** 2026-05-30

## APIs

### Raygun Applications API

List, retrieve, and regenerate API keys for applications under your Raygun organization. Applications are the root resource — each owns its own error groups, deployments, source maps, sessions, pages, customers, and Flutter symbols.

- **Human URL:** [https://api.raygun.io/v3/swagger/index.html](https://api.raygun.io/v3/swagger/index.html)

#### Tags

- Observability
- Applications

#### Properties

- [Documentation](https://api.raygun.io/v3/swagger/index.html)
- [OpenAPI](openapi/raygun-applications-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/raygun-applications-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-applications-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON-LD](json-ld/raygun-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Raygun Errors API

Triage error groups and instances — list, get, resolve, activate, ignore, permanently ignore, and comment on grouped errors. Drill into individual error instances with full stack-trace, environment, request, and breadcrumb context.

- **Human URL:** [https://api.raygun.io/v3/swagger/index.html](https://api.raygun.io/v3/swagger/index.html)

#### Tags

- Observability
- Crash Reporting
- Errors
- Error Groups

#### Properties

- [Documentation](https://api.raygun.io/v3/swagger/index.html)
- [OpenAPI](openapi/raygun-errors-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/raygun-errors-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-errors-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/raygun-error-group-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Example](examples/raygun-error-group-example.json)
- [Example](examples/raygun-crash-report-example.json)

### Raygun Deployments API

Record release markers and correlate them with error groups. Supports SCM integration (GitHub, GitLab, Bitbucket, Azure DevOps), commit reprocessing, latest-deploy lookup, and the api-key shortcut variant for CI pipelines.

- **Human URL:** [https://api.raygun.io/v3/swagger/index.html](https://api.raygun.io/v3/swagger/index.html)

#### Tags

- Observability
- Deployments
- Release Tracking

#### Properties

- [Documentation](https://api.raygun.io/v3/swagger/index.html)
- [OpenAPI](openapi/raygun-deployments-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/raygun-deployments-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-deployments-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/raygun-deployment-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Example](examples/raygun-create-deployment-example.json)

### Raygun Source Maps API

Upload, list, retrieve, update, and delete JavaScript source maps for symbolicating minified front-end stack traces in Crash Reporting and RUM error data.

- **Human URL:** [https://api.raygun.io/v3/swagger/index.html](https://api.raygun.io/v3/swagger/index.html)

#### Tags

- Observability
- Source Maps
- JavaScript

#### Properties

- [Documentation](https://api.raygun.io/v3/swagger/index.html)
- [OpenAPI](openapi/raygun-source-maps-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/raygun-source-maps-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-source-maps-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Raygun Sessions API

List and retrieve Real User Monitoring sessions captured for an application. Each session contains page views, custom timings, and the errors a user experienced during that browsing period.

- **Human URL:** [https://api.raygun.io/v3/swagger/index.html](https://api.raygun.io/v3/swagger/index.html)

#### Tags

- Observability
- Real User Monitoring
- Sessions

#### Properties

- [Documentation](https://api.raygun.io/v3/swagger/index.html)
- [OpenAPI](openapi/raygun-sessions-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/raygun-sessions-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-sessions-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Raygun Pages API

List and retrieve monitored pages for an application — the per-URL aggregation surface for RUM timing, Core Web Vitals, and page-level error rates.

- **Human URL:** [https://api.raygun.io/v3/swagger/index.html](https://api.raygun.io/v3/swagger/index.html)

#### Tags

- Observability
- Real User Monitoring
- Pages
- Core Web Vitals

#### Properties

- [Documentation](https://api.raygun.io/v3/swagger/index.html)
- [OpenAPI](openapi/raygun-pages-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/raygun-pages-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-pages-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Raygun Customers API

List and retrieve customer (end-user) records associated with sessions and error instances. Supports both identified and anonymous user records.

- **Human URL:** [https://api.raygun.io/v3/swagger/index.html](https://api.raygun.io/v3/swagger/index.html)

#### Tags

- Observability
- Real User Monitoring
- Customers
- Users

#### Properties

- [Documentation](https://api.raygun.io/v3/swagger/index.html)
- [OpenAPI](openapi/raygun-customers-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/raygun-customers-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-customers-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Raygun Metrics API

Query time-series and histogram metrics for page performance and error rates with flexible bucket, range, and filter parameters. Powers custom dashboards and external observability exports.

- **Human URL:** [https://api.raygun.io/v3/swagger/index.html](https://api.raygun.io/v3/swagger/index.html)

#### Tags

- Observability
- Metrics
- Real User Monitoring
- Time Series

#### Properties

- [Documentation](https://api.raygun.io/v3/swagger/index.html)
- [OpenAPI](openapi/raygun-metrics-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/raygun-metrics-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-metrics-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Raygun Flutter Symbols API

Upload and manage Flutter debug-symbol artifacts so Raygun can symbolicate native crashes from Flutter mobile applications across iOS and Android builds.

- **Human URL:** [https://api.raygun.io/v3/swagger/index.html](https://api.raygun.io/v3/swagger/index.html)

#### Tags

- Observability
- Crash Reporting
- Flutter
- Mobile
- Symbols

#### Properties

- [Documentation](https://api.raygun.io/v3/swagger/index.html)
- [OpenAPI](openapi/raygun-flutter-symbols-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/raygun-flutter-symbols-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-flutter-symbols-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Raygun Teams API

List and retrieve teams in your Raygun organization. Teams group members and grant shared access to a curated set of applications.

- **Human URL:** [https://api.raygun.io/v3/swagger/index.html](https://api.raygun.io/v3/swagger/index.html)

#### Tags

- Observability
- Administration
- Teams

#### Properties

- [Documentation](https://api.raygun.io/v3/swagger/index.html)
- [OpenAPI](openapi/raygun-teams-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/raygun-teams-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-teams-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Raygun Invitations API

Send, list, retrieve, and revoke organization-member invitations. Used to programmatically onboard and offboard users from your Raygun account.

- **Human URL:** [https://api.raygun.io/v3/swagger/index.html](https://api.raygun.io/v3/swagger/index.html)

#### Tags

- Observability
- Administration
- Invitations

#### Properties

- [Documentation](https://api.raygun.io/v3/swagger/index.html)
- [OpenAPI](openapi/raygun-invitations-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/raygun-invitations-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-invitations-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Raygun Plans API

List the available Raygun subscription plans so dashboards and automations can inspect entitlement levels and current allotments per product.

- **Human URL:** [https://api.raygun.io/v3/swagger/index.html](https://api.raygun.io/v3/swagger/index.html)

#### Tags

- Observability
- Administration
- Plans
- Billing

#### Properties

- [Documentation](https://api.raygun.io/v3/swagger/index.html)
- [OpenAPI](openapi/raygun-plans-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/raygun-plans-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-plans-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Raygun Crash Reporting Ingestion API

POST /entries ingestion endpoint at api.raygun.com used by all language SDKs and providers to submit crash payloads. X-ApiKey authenticated; 128 KB payload ceiling; 202 on accept, 400/403/413/429 on error.

- **Human URL:** [https://raygun.com/documentation/product-guides/crash-reporting/api/](https://raygun.com/documentation/product-guides/crash-reporting/api/)

#### Tags

- Observability
- Crash Reporting
- Ingestion

#### Properties

- [Documentation](https://raygun.com/documentation/product-guides/crash-reporting/api/)
- [JSON Schema](json-schema/raygun-error-group-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Example](examples/raygun-crash-report-example.json)
- [Postman Collection](collections/raygun-applications-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-applications-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-customers-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-customers-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-deployments-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-deployments-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-errors-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-errors-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-flutter-symbols-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-flutter-symbols-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-invitations-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-invitations-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-metrics-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-metrics-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-pages-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-pages-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-plans-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-plans-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-public-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-public-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-sessions-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-sessions-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-source-maps-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-source-maps-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-teams-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-teams-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Raygun Outbound Webhooks

Outbound webhook surface that POSTs JSON events to a customer-configured HTTPS endpoint when error notifications fire (NewErrorOccurred, ErrorReoccurred for regression detection, and the 1/5/10/30/60-minute follow-up cadence) and when error-group activity occurs (StatusChanged, AssignedToUser, CommentAdded). The same event vocabulary drives the managed Slack and Microsoft Teams integrations. Requires Team plan or higher.

- **Human URL:** [https://raygun.com/documentation/product-guides/crash-reporting/integrations/webhooks/](https://raygun.com/documentation/product-guides/crash-reporting/integrations/webhooks/)

#### Tags

- Observability
- Crash Reporting
- Webhooks
- Event-Driven
- Regression Detection
- Slack
- Microsoft Teams

#### Properties

- [Documentation](https://raygun.com/documentation/product-guides/crash-reporting/integrations/webhooks/)
- [Documentation](https://raygun.com/documentation/product-guides/crash-reporting/integrations/slack/)
- [Documentation](https://raygun.com/documentation/product-guides/integrations/microsoft-teams-plan-integration/)
- [AsyncAPI](openapi/raygun-webhooks-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [Postman Collection](collections/raygun-applications-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-applications-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-customers-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-customers-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-deployments-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-deployments-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-errors-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-errors-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-flutter-symbols-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-flutter-symbols-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-invitations-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-invitations-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-metrics-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-metrics-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-pages-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-pages-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-plans-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-plans-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-public-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-public-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-sessions-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-sessions-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-source-maps-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-source-maps-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-teams-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-teams-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Raygun Pulse RUM API (Legacy)

Legacy enterprise-only Real User Monitoring read API at api.raygun.com/api/v1/pulse. Uses a Client ID/Secret-issued X-SessionKey with 15-minute TTL. Default rate limit 50 calls/day/application. Most new workloads use the v3 Sessions/Pages/Metrics APIs instead.

- **Human URL:** [https://raygun.com/documentation/product-guides/real-user-monitoring/api/](https://raygun.com/documentation/product-guides/real-user-monitoring/api/)

#### Tags

- Observability
- Real User Monitoring
- Pulse
- Legacy

#### Properties

- [Documentation](https://raygun.com/documentation/product-guides/real-user-monitoring/api/)
- [Postman Collection](collections/raygun-applications-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-applications-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-customers-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-customers-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-deployments-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-deployments-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-errors-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-errors-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-flutter-symbols-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-flutter-symbols-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-invitations-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-invitations-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-metrics-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-metrics-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-pages-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-pages-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-plans-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-plans-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-public-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-public-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-sessions-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-sessions-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-source-maps-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-source-maps-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/raygun-teams-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/raygun-teams-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [Portal](https://raygun.com)
- [Documentation](https://raygun.com/documentation/)
- [Documentation](https://raygun.com/documentation/product-guides/public-api/)
- [Documentation](https://api.raygun.io/v3/swagger/index.html)
- [OpenAPI](https://api.raygun.io/v3/raygun-openapi-spec.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Documentation](https://raygun.com/documentation/product-guides/crash-reporting/api/)
- [Documentation](https://raygun.com/documentation/product-guides/real-user-monitoring/api/)
- [Status Page](https://status.raygun.com)
- [Changelog](https://raygun.com/changelog)
- [Blog](https://raygun.com/blog/)
- [Getting Started](https://raygun.com/documentation/)
- [Pricing](https://raygun.com/pricing)
- [Sign Up](https://app.raygun.com/signup)
- [Support](https://raygun.com/contact)
- [Terms of Service](https://raygun.com/terms)
- [Privacy Policy](https://raygun.com/privacy)
- [Security](https://raygun.com/platform/security-and-compliance)
- [GitHub Organization](https://github.com/MindscapeHQ)
- [SDK](https://github.com/MindscapeHQ/raygun4js)
- [SDK](https://github.com/MindscapeHQ/raygun4net)
- [SDK](https://github.com/MindscapeHQ/raygun4node)
- [SDK](https://github.com/MindscapeHQ/raygun4python)
- [SDK](https://github.com/MindscapeHQ/raygun4ruby)
- [SDK](https://github.com/MindscapeHQ/raygun4php)
- [SDK](https://github.com/MindscapeHQ/raygun4android)
- [SDK](https://github.com/MindscapeHQ/raygun4flutter)
- [SDK](https://github.com/MindscapeHQ/raygun4reactnative)
- [SDK](https://github.com/MindscapeHQ/raygun4maui)
- [SDK](https://github.com/MindscapeHQ/raygun4blazor)
- [Tool](https://github.com/MindscapeHQ/raygun-cli)
- [Tool](https://github.com/MindscapeHQ/raygun4node-aws-lambda)
- [Plugin](https://github.com/MindscapeHQ/ember-cli-raygun)
- [Integrations](undefined)
- [Plans](plans/raygun-plans-pricing.yml)
- [Rate Limits](rate-limits/raygun-rate-limits.yml)
- [Fin Ops](finops/raygun-finops.yml)
- [Vocabulary](vocabulary/raygun-vocabulary.yml)
- [Spectral Rules](rules/raygun-rules.yml)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
