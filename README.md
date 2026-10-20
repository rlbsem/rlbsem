# Richard Butts

**Enterprise MarTech & Systems Architecture · GTM & Revenue Systems · Data & Analytics Engineering · Applied AI**

I engineer commercial systems so customer identity, sales activity, operational commitments, financial outcomes and automated decisions stay trustworthy across platforms. The result is safer handoffs, accountable recovery and analytics leaders can use to make decisions.

**Enterprise delivery context:** My professional work spans **approximately 30 systems and data engagements**, roughly **80% supporting operating brands in private-equity-backed portfolios**, alongside independently operated multi-brand groups. The work includes acquisition/platform integrations, CRM-to-operations and finance handoffs, master-data authority, pipeline attribution, revenue reconciliation, data infrastructure and governed AI.

These public implementations are **selected technical demonstrations** from a much broader professional engineering career. They use synthetic or permitted public data and do not disclose confidential client deployments.

**Connect:** [LinkedIn](https://www.linkedin.com/in/rbutts/) · [Interactive evidence Lab](https://rlbsem.github.io/enterprise-revenue-systems-lab/)

## Engineering Implementations & Evidence

Four flagship implementations connecting enterprise business problems to working code, failure tests and inspectable execution evidence.

**1. [Customer Signal & Activation](https://github.com/rlbsem/customer-signal-activation)**

**Business outcome:** Turn scattered account signals into explainable, owner-safe seller actions without duplicate work or treating Closed Won as collected cash. This system combines verified identity, fit/intent scoring, approval-controlled CRM activation and fulfillment-to-cash measurement. **Engineering proof:** An executed **Salesforce ↔ Snowflake round-trip** recovered a lost acknowledgment without another create; independent read-back confirmed the effect, and CRM feedback changed the warehouse recommendation. Restricted reads and replay controls were also verified, alongside 352 passing local tests.

[Native integration evidence](https://github.com/rlbsem/customer-signal-activation/blob/main/docs/evidence/connected-integration/README.md) · [Salesforce permission and recovery tests](https://github.com/rlbsem/customer-signal-activation/blob/main/docs/evidence/salesforce-native/README.md)

**2. [Enterprise MarTech / AI Control Plane](https://github.com/rlbsem/enterprise-martech-ai-control-plane)**

**Business outcome:** Keep disconnected systems and AI automations from overwriting customer truth, bypassing permissions or repeating a commercial action when an API acknowledgment is lost. This Python/PostgreSQL control plane enforces identity, field ownership, consent, approval, durable execution and reconciliation. **Engineering proof:** Native AWS checks verified independent PostgreSQL receipts, duplicate safety and restricted reads; an RDS backup restore was observed available. The linked AWS report documents the unverified application-level restore check and unexecuted production deployment.

[AWS execution and cleanup](https://github.com/rlbsem/enterprise-martech-ai-control-plane/blob/main/docs/evidence/aws-readiness/retained-two-instance/native-outcome/README.md) · [Recovery tests](https://github.com/rlbsem/enterprise-martech-ai-control-plane/blob/main/docs/evidence/report.md) · [Architecture](https://github.com/rlbsem/enterprise-martech-ai-control-plane/blob/main/docs/architecture.md)

**3. [Revenue Metrics Platform](https://github.com/rlbsem/revenue-metrics-platform)**

**Business outcome:** Give Sales, Finance and executives comparable definitions for pipeline, bookings, invoicing, collected cash and ARR instead of competing dashboards. The SQL/dbt platform models distinct economic events, historical state and source-traceable reconciliation. **Engineering proof:** Native Snowflake acceptance completed three fixture builds, each with 15 models and 30 passing tests. The larger synthetic enterprise scenario was tested locally, not benchmarked in Snowflake.

[Snowflake execution evidence](https://github.com/rlbsem/revenue-metrics-platform/blob/main/docs/evidence/snowflake/fixture/README.md)

**4. [First-Party Measurement Assurance](https://github.com/rlbsem/first-party-measurement-assurance)**

**Business outcome:** Prevent Marketing from mistaking a website inquiry, signed commitment or deposit for the same economic conversion. This implementation connects consent-aware browser events, GTM data layers, durable offline conversion receipts and SQL/dbt reconciliation. **Engineering proof:** Native BigQuery queries against Google's public GA4 sample identified 14 purchase events behind 57 nested item rows and retained two unresolved revenue discrepancies. The local business scenarios are separately synthetic.

[BigQuery execution evidence](https://github.com/rlbsem/first-party-measurement-assurance/blob/main/docs/evidence/google-bigquery/README.md) · [Windows/Linux CI](https://github.com/rlbsem/first-party-measurement-assurance/actions/runs/39007934132)

## Six Additional Engineering Systems

These six repositories cover different failure modes and bring the core engineering portfolio to ten projects.

- **[MarTech Data Reliability](https://github.com/rlbsem/martech-data-reliability):** Contract-checked ingestion, quarantine and correction handling keep invalid loads from replacing validated reporting data.
- **[MarTech Migration Assurance](https://github.com/rlbsem/martech-migration-assurance):** Semantic parity, change catch-up and rollback gates expose migrations that preserve row counts but alter business meaning.
- **[Temporal Customer Audiences](https://github.com/rlbsem/temporal-customer-audiences):** Business-time and knowledge-time history account for late-arriving facts, corrected eligibility and auditable past decisions.
- **[Enterprise Agent Runtime & Evaluation](https://github.com/rlbsem/enterprise-agent-runtime-evaluation):** Local model inference, adversarial evaluation, source checks and release gates provide evidence before an AI version is promoted.
- **[MarTech Estate Impact](https://github.com/rlbsem/martech-estate-impact):** Dependency evidence and explicit uncertainty make platform retirement and consolidation decisions inspectable.
- **[MarTech Stack Economics](https://github.com/rlbsem/martech-stack-economics):** Constrained optimization tests proposed savings against cost, freshness, capacity and API quotas.

### Architecture capability map

How the ten projects relate across revenue, GTM controls, enterprise architecture and AI systems:

<img src="assets/capability-map.svg" alt="Capability map showing ten engineering projects grouped by revenue and analytics, GTM and control, enterprise architecture, and temporal and AI assurance" width="880">

[View the full-size diagram](assets/capability-map.svg).

## Explore engineering in action

**[Enterprise Revenue Systems Lab](https://rlbsem.github.io/enterprise-revenue-systems-lab/): interactive evidence explorer** · [Source code](https://github.com/rlbsem/enterprise-revenue-systems-lab)

For a closer look at selected implementation behaviors, the Lab now offers four investigations:

- **AI seller decisions:** Examine a model-generated recommendation, its supporting sources, a reviewed edit, approval and recorded delivery evidence.
- **Execution recovery:** Trace a lost acknowledgment and worker interruption through durable workflow state and independent receiver receipts, including duplicate prevention.
- **Revenue reconciliation:** Explore why installed ARR, bookings, invoices and collected cash differ, with a source-backed financial bridge.
- **Native Salesforce and Snowflake:** [Inspect the CRM-to-warehouse round trip](https://rlbsem.github.io/enterprise-revenue-systems-lab/?case=connected-roundtrip), including source authority, lost-acknowledgment recovery, independent CRM readback and the resulting warehouse decision.

**No installation is needed to explore.** The hosted site presents recorded, verifiable **synthetic evidence**; fresh inference and original-engine execution are available only through separate local workflows.

## Systems, technologies, and control patterns

**Enterprise platforms and business systems:** Salesforce · HubSpot · Salesforce Marketing Cloud · Marketing Cloud Account Engagement (Pardot) · Marketo · Segment · Clay · LinkedIn Sales Navigator · HighLevel (GoHighLevel) · LMN · Aspire · QuickBooks · Google Analytics 4 (GA4) · Google Tag Manager (GTM) · Adobe Analytics · Tableau · Power BI · Vapi · Dialpad · Make · n8n · Workato · Zapier

**Engineering, data platforms, and cloud:** Python · SQL · JavaScript / TypeScript · PostgreSQL · Snowflake · Supabase · dbt · DuckDB · SQLite · FastAPI · Streamlit · Airflow · Git · GitHub Actions / CI/CD · Docker · Terraform · AWS architecture (ECS/Fargate, RDS, ECR, IAM/OIDC)

**Data architecture and enterprise integration:** Dimensional modeling · SCD Type 2 · Bitemporal data · Governed metrics · Data contracts · Schema evolution · ETL / ELT · Reverse ETL / warehouse-to-CRM activation · Incremental processing · Backfills · REST APIs · Webhooks · OAuth 2.0 · Canonical identity · Entity resolution · Source lineage · GTM engineering · Lead scoring and routing · SDR/AE workflow automation · Sales engagement systems · Pipeline attribution · Meta Conversions API · Google Enhanced Conversions · Offline conversion tracking · Server-side measurement

**Reliability, governance, and AI systems:** Source authority · Field ownership · No-Regress Logic · Stateful middleware · Idempotency · Replay safety · Retry/backoff · Exception queues · RBAC · Consent governance · Audit logging · Revenue reconciliation · Failure recovery · Release gates · OpenAI / LLM APIs · Anthropic Claude · Qwen local inference · llama.cpp · Model Context Protocol (MCP) · Prompt engineering · Tool/function calling · Structured outputs · LLM evaluation · Human approval controls

## How to evaluate the work

The repositories include source code, tests, evidence and operating limits. Public examples use synthetic or vendor-neutral data; native execution is identified separately from local tests and production deployment.

**Tools execute. The control layer determines what is true.**
