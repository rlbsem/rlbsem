# Richard Butts

**Enterprise MarTech & Systems Architecture · GTM & Revenue Systems · Data & Analytics Engineering · Applied AI**

I architect and build governed systems across customer data, CRM, MarTech, revenue operations, analytics, and AI. My work connects commercial definitions to technical controls: canonical identity, field ownership, source provenance, durable state, reconciliation, and recovery when systems disagree or fail.

**Connect:** [LinkedIn](https://www.linkedin.com/in/rbutts/)

## Engineering Implementations & Evidence

Four selected systems demonstrate how I approach enterprise failures: define the problem, implement the controls, and make the resulting behavior inspectable.

**1. [Customer Signal & Activation](https://github.com/rlbsem/customer-signal-activation)**

**Problem:** Fragmented customer identity, stale enrichment, unsafe sales handoffs and revenue outcomes that cannot be traced to collected cash.  
**Solution:** Consent-aware signals, verified accounts, explainable fit and intent scoring, owner-safe CRM activation, AI-assisted seller review and fulfillment-to-cash reconciliation.  
**Evidence:** Executed **native Salesforce ↔ Snowflake governed round-trip**: synthetic CRM state through warehouse decisions, one approval-bound Salesforce write with a deliberately lost acknowledgment, exact receipt recovery, independent read-back and feedback that changed the warehouse decision. Restricted Snowflake reads and replay/no-regress controls were verified; 352 local tests passed. [Inspect cross-platform execution evidence](https://github.com/rlbsem/customer-signal-activation/blob/main/docs/evidence/connected-integration/README.md) · [Salesforce permission and recovery evidence](https://github.com/rlbsem/customer-signal-activation/blob/main/docs/evidence/salesforce-native/README.md).

**2. [Enterprise MarTech / AI Control Plane](https://github.com/rlbsem/enterprise-martech-ai-control-plane)**

**Problem:** Connected platforms can overwrite authoritative data, repeat uncertain downstream actions or allow automation to exceed its permissions.  
**Solution:** Python/PostgreSQL governance for canonical identity, source authority, consent, field ownership, durable execution, human approval and exception handling.  
**Evidence:** Executed PostgreSQL governance and recovery tests plus **native AWS RDS acceptance**: private databases, 1-intent/1-receipt reconciliation, duplicate safety, read-only permission denials, and a real retained-backup restore observed available. Independent teardown was verified. Native restored-state fail-closed reconciliation remains unverified; the production AWS stack was not deployed. [Inspect AWS execution and cleanup evidence](https://github.com/rlbsem/enterprise-martech-ai-control-plane/blob/main/docs/evidence/aws-readiness/retained-two-instance/native-outcome/README.md) · [Recovery tests](https://github.com/rlbsem/enterprise-martech-ai-control-plane/blob/main/docs/evidence/report.md) · [Architecture](https://github.com/rlbsem/enterprise-martech-ai-control-plane/blob/main/docs/architecture.md).

**3. [Revenue Metrics Platform](https://github.com/rlbsem/revenue-metrics-platform)**

**Problem:** Pipeline, bookings, invoicing, cash and ARR are different economic measures, yet disconnected reports can treat them as interchangeable.  
**Solution:** Governed SQL/dbt dimensional models, historical state, consistent metric definitions and source-traceable reconciliation bridges.  
**Evidence:** **Native Snowflake fixture acceptance** passed across three builds, each with 15 models and 30 tests. The larger synthetic enterprise scenario was verified locally, not cloud-benchmarked. [Inspect Snowflake execution evidence](https://github.com/rlbsem/revenue-metrics-platform/blob/main/docs/evidence/snowflake/fixture/README.md).

**4. [First-Party Measurement Assurance](https://github.com/rlbsem/first-party-measurement-assurance)**

**Problem:** Browser and offline conversion reporting can miss events or overstate revenue by confusing proposals, signed contracts, deposits and payments.  
**Solution:** Consent-aware browser events, GTM-compatible data layers, source-authorized offline conversions, durable receipts and SQL/dbt reconciliation.  
**Evidence:** Executed browser and local warehouse workflows; **native BigQuery Studio queries against Google's public GA4 sample** exposed 14 purchase events versus 57 nested item rows and preserved two revenue discrepancies. This Google sample evidence is separate from the synthetic business scenario. [BigQuery execution evidence](https://github.com/rlbsem/first-party-measurement-assurance/blob/main/docs/evidence/google-bigquery/README.md) · [Passing Windows/Linux CI](https://github.com/rlbsem/first-party-measurement-assurance/actions/runs/39007934132).

## Six Additional Engineering Systems

Alongside the four implementations above, these complete **ten core engineering projects**. Each addresses a different enterprise failure or decision.

- **[MarTech Data Reliability](https://github.com/rlbsem/martech-data-reliability)** — **Problem:** Late, duplicate or corrected data can invalidate marketing reports. **System:** Contract-checked ingestion, quarantines, corrections and reconciliation. **Benefit:** A bad load cannot silently replace the last validated publication.
- **[MarTech Migration Assurance](https://github.com/rlbsem/martech-migration-assurance)** — **Problem:** Moving platforms can preserve row counts while corrupting business meaning. **System:** Semantic parity tests, change catch-up, cutover gates and evidence-bound rollback. **Benefit:** Unsafe migrations are stopped before customers' records are misrepresented.
- **[Temporal Customer Audiences](https://github.com/rlbsem/temporal-customer-audiences)** — **Problem:** Customer eligibility changes, and late-arriving facts may correct what was known yesterday. **System:** Business-time and knowledge-time history, restatements, expiry and activation reconciliation. **Benefit:** Audiences reflect current eligibility while earlier decisions remain auditable.
- **[Enterprise Agent Runtime & Evaluation](https://github.com/rlbsem/enterprise-agent-runtime-evaluation)** — **Problem:** AI output can sound reasonable while being unsafe or unsupported. **System:** Actual local model inference, adversarial tests, source checks and release gates. **Benefit:** Unsafe agent versions can be blocked instead of promoted on persuasive prose alone.
- **[MarTech Estate Impact](https://github.com/rlbsem/martech-estate-impact)** — **Problem:** Retiring a seemingly redundant platform can break hidden business workflows. **System:** Evidence-backed dependency maps and change-impact analysis that preserve uncertainty. **Benefit:** Consolidation decisions have inspectable justification.
- **[MarTech Stack Economics](https://github.com/rlbsem/martech-stack-economics)** — **Problem:** The cheapest integration design can miss deadlines or API limits during peak demand. **System:** Constrained, independently checked optimization across cost, capacity, quotas and freshness. **Benefit:** Proposed savings are evaluated against service requirements.

### Architecture capability map

An at-a-glance view of the ten implementations and the enterprise problems they address:

<img src="assets/capability-map.svg" alt="Capability map showing ten engineering projects grouped by revenue and analytics, GTM and control, enterprise architecture, and temporal and AI assurance" width="880">

[View the full-size diagram](assets/capability-map.svg).

## Explore engineering in action

**[Enterprise Revenue Systems Lab — browser-based evidence explorer](https://rlbsem.github.io/enterprise-revenue-systems-lab/)** · [Source code and reproduction](https://github.com/rlbsem/enterprise-revenue-systems-lab)

For a closer look at selected implementation behaviors, the Lab offers three independent investigations:

- **AI seller decisions:** Examine a model-generated recommendation, its supporting sources, a reviewed edit, approval and recorded delivery evidence.
- **Execution recovery:** Trace a lost acknowledgment and worker interruption through durable workflow state and independent receiver receipts, including duplicate prevention.
- **Revenue reconciliation:** Explore why installed ARR, bookings, invoices and collected cash differ, with a source-backed financial bridge.

**No installation is needed to explore.** The hosted site presents recorded, verifiable **synthetic evidence**; fresh inference and original-engine execution are available only through separate local workflows.

## Systems, technologies, and control patterns

**Enterprise platforms and business systems:** Salesforce · HubSpot · Salesforce Marketing Cloud · Marketing Cloud Account Engagement (Pardot) · Marketo · Segment · Clay · LinkedIn Sales Navigator · HighLevel (GoHighLevel) · LMN · Aspire · QuickBooks · Google Analytics 4 (GA4) · Google Tag Manager (GTM) · Adobe Analytics · Tableau · Power BI · Vapi · Dialpad · Make · n8n · Workato · Zapier

**Engineering, data platforms, and cloud:** Python · SQL · JavaScript / TypeScript · PostgreSQL · Snowflake · Supabase · dbt · DuckDB · SQLite · FastAPI · Streamlit · Airflow · Git · GitHub Actions / CI/CD · Docker · Terraform · AWS architecture (ECS/Fargate, RDS, ECR, IAM/OIDC)

**Data architecture and enterprise integration:** Dimensional modeling · SCD Type 2 · Bitemporal data · Governed metrics · Data contracts · Schema evolution · ETL / ELT · Reverse ETL / warehouse-to-CRM activation · Incremental processing · Backfills · REST APIs · Webhooks · OAuth 2.0 · Canonical identity · Entity resolution · Source lineage · GTM engineering · Lead scoring and routing · SDR/AE workflow automation · Sales engagement systems · Pipeline attribution · Meta Conversions API · Google Enhanced Conversions · Offline conversion tracking · Server-side measurement

**Reliability, governance, and AI systems:** Source authority · Field ownership · No-Regress Logic · Stateful middleware · Idempotency · Replay safety · Retry/backoff · Exception queues · RBAC · Consent governance · Audit logging · Revenue reconciliation · Failure recovery · Release gates · OpenAI / LLM APIs · Anthropic Claude · Qwen local inference · llama.cpp · Model Context Protocol (MCP) · Prompt engineering · Tool/function calling · Structured outputs · LLM evaluation · Human approval controls

## How to evaluate the work

Each repository provides implementation details, tests, execution evidence, and known limitations. The public systems use **synthetic or vendor-neutral data** so the architecture can be inspected without exposing private client environments. They demonstrate engineering patterns, **not a claim that any public repository was deployed unchanged into client production**.

**Tools execute. The control layer determines what is true.**
