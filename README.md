<div align="center">

[![English](https://img.shields.io/badge/English-2f81f7?style=flat-square)](README.md)
[![简体中文](https://img.shields.io/badge/简体中文-d0d7de?style=flat-square)](README.zh-CN.md)

# Li Weipei · Leewwp

**Backend engineer — Go & Java.** I build the parts of an LLM application that have to survive production:
retrieval quality, agent orchestration, failure degradation, observability, and security boundaries.

<sub>Hong Kong</sub>

</div>

---

## Focus

| Area | In practice |
| --- | --- |
| **Retrieval & RAG** | Hybrid retrieval over pgvector / Elasticsearch / Qdrant · citation traceability · visibility filtering · degrading gracefully when a backend is unavailable |
| **Agent engineering** | Tool orchestration · MCP servers and clients · prompt lifecycle and versioning · structured-output contracts |
| **Production hardening** | End-to-end tracing · LLM cost accounting · tenant and permission boundaries · CI quality gates |

## Projects

**[OmniCraft](https://github.com/Leewwp/OmniCraft)** · Go · Next.js · PostgreSQL/pgvector · Redis Streams
A content-sharing platform whose core is a server-mediated, single-agent RAG workbench: citation re-checking, visibility filtering, degradation-capable hybrid retrieval, and a transactional-outbox async pipeline. Ships with offline evaluation, security gates, and full-trace observability.

**[polyu-agent](https://github.com/Leewwp/polyu-agent)** · Spring Boot 3 · pgvector / Elasticsearch · React · [polyuguide.com](https://polyuguide.com)
A bilingual Q&A agent for campus information at PolyU (unofficial). Domain-partitioned knowledge bases, citation traceability, and scheduled content refresh on a deterministic ingestion pipeline.

**[health_agent](https://github.com/Leewwp/health_agent)** · Java · Spring Boot
A unified health assistant covering three product categories. Deterministic multi-role workflow orchestration driven by an explicit state machine, contract-based degradation, hybrid-retrieval RAG, and an MCP server surface — backed by 900+ automated tests.

**[ppp-rpc](https://github.com/Leewwp/ppp-rpc)** · Java · Netty · ZooKeeper
A lightweight RPC framework built from the wire up: Netty transport, ZooKeeper-based service discovery, three load-balancing strategies, and retry policies.

<details>
<summary><b>Also built</b></summary>

- **[jewel-ar-tryon](https://github.com/Leewwp/jewel-ar-tryon)** — technical PoC for AR jewelry try-on in a WeChat Mini Program.
- **[Proactive-Diet-Shopping-Assistant](https://github.com/Leewwp/Proactive-Diet-Shopping-Assistant)** — Expo / React Native shopping assistant: barcode and vision recognition, allergen conflict detection, nutrition-compliance scoring.
- **[ADA_Project](https://github.com/Leewwp/ADA_Project)** — short-horizon air-quality forecasting: multivariate time-series ETL, feature engineering, multi-model comparison over the Open-Meteo API.
- **[ppp-blog](https://github.com/Leewwp/ppp-blog)** — Halo 2.x blog stack: Docker Compose deployment, GitHub Actions CI/CD, monitoring and alerting.

</details>

## Open source

Contributions to projects I depend on:

- **[docling-project/docling-core #766](https://github.com/docling-project/docling-core/pull/766)** — Markdown table serialization: row-header rows no longer leak into the table header block.
- **[elastic/beats #53159](https://github.com/elastic/beats/pull/53159)** — corrected wording defects in user-facing error messages (filebeat, winlogbeat).
- **[nageoffer/ragent #131](https://github.com/nageoffer/ragent/pull/131) [#132](https://github.com/nageoffer/ragent/pull/132) [#133](https://github.com/nageoffer/ragent/pull/133) [#136](https://github.com/nageoffer/ragent/pull/136)** — document-ingestion hardening (outbound validation, response size caps, no error-body echo), upload-endpoint rate limiting, parser/module cleanup, and a flaky-CI fix in the trace test suite.

## Stack

- **Languages** — Go · Java · TypeScript · Python
- **Backend** — Spring Boot 3 · Gin · Netty
- **LLM / Agent** — RAG (pgvector · Elasticsearch · Qdrant) · agent orchestration · MCP · DashScope / MiniMax / DeepSeek
- **Data** — PostgreSQL · MySQL · Redis / Redis Streams
- **Frontend** — Next.js / React · React Native
- **Engineering** — Docker · GitHub Actions · OpenTelemetry

## Elsewhere

- **Live product** — [polyuguide.com](https://polyuguide.com)

<div align="center">
<sub>Open to conversations about agent engineering, retrieval quality, and production LLM infrastructure.</sub>
</div>
