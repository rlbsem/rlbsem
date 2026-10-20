# Richard Butts

**Enterprise MarTech & Systems Architecture · GTM & Revenue Systems · Data & Analytics Engineering · Applied AI**

I design and build systems that keep customer, operational and revenue data reliable across platforms. My work focuses on source authority, identity, reconciliation, durable execution and recovery.

**Professional background:** I founded Groundbreakers Digital in 2023 and have delivered roughly 30 projects across founder-owned and PE-backed businesses, including CRM, operations and finance integration, data integrity and audit controls. Before that, I was promoted twice at Lorex, reaching Director of Digital Marketing as annual ecommerce revenue grew from approximately $55M to $101M. At LMN, I managed approximately US$350K per month in acquisition across multiple B2B SaaS products, with CAC reductions of approximately 15–25%.

These repositories demonstrate relevant engineering methods using public synthetic or vendor data. They are not representations of confidential client deployments.

**Connect:** [LinkedIn](https://www.linkedin.com/in/rbutts/) · [Interactive evidence Lab](https://rlbsem.github.io/enterprise-revenue-systems-lab/)

## Engineering Implementations & Evidence

Four implementations with working code, failure tests and execution records.

**1. [Customer Signal & Activation](https://github.com/rlbsem/customer-signal-activation)**

Customer signals are only useful when identity, consent and CRM ownership remain intact. This system combines verified accounts, explainable fit and intent scoring, approval-controlled activation and fulfillment-to-cash reconciliation. In an **executed Salesforce ↔ Snowflake round-trip**, a lost Salesforce acknowledgment was recovered without creating another record. Independent read-back confirmed the effect, and CRM feedback changed the warehouse recommendation. Restricted reads and replay controls were also verified, alongside 352 passing local tests.

[Native integration evidence](https://github.com/rlbsem/customer-signal-activation/blob/main/docs/evidence/connected-integration/README.md) · [Salesforce permission and recovery tests](https://github.com/rlbsem/customer-signal-activation/blob/main/docs/evidence/salesforce-native/README.md)

**2. [Enterprise MarTech / AI Control Plane](https://github.com/rlbsem/enterprise-martech-ai-control-plane)**

When CRM, operations or AI workflows disagree, authoritative customer data can be overwritten and uncertain requests can trigger duplicate actions. I built a Python/PostgreSQL control plane to enforce identity, field ownership, consent, approval and durable execution across those boundaries. Native AWS tests verified independent receipts, duplicate prevention, read-only restrictions and a **retained-backup RDS restore observed available**. The final native fail-closed comparison was not recorded; production AWS services were not deployed.

[AWS execution and cleanup](https://github.com/rlbsem/enterprise-martech-ai-control-plane/blob/main/docs/evidence/aws-readiness/retained-two-instance/native-outcome/README.md) · [Recovery tests](https://github.com/rlbsem/enterprise-martech-ai-control-plane/blob/main/docs/evidence/report.md) · [Architecture](https://github.com/rlbsem/enterprise-martech-ai-control-plane/blob/main/docs/architecture.md)

**3. [Revenue Metrics Platform](https://github.com/rlbsem/revenue-metrics-platform)**

Bookings, invoices, collected cash and ARR measure different events. This platform uses SQL/dbt models, historical state and source-traceable reconciliation to keep those definitions consistent. **Native Snowflake acceptance** completed three fixture builds, each with 15 models and 30 tests. The larger synthetic enterprise scenario was tested locally rather than benchmarked in Snowflake.

[Snowflake execution evidence](https://github.com/rlbsem/revenue-metrics-platform/blob/main/docs/evidence/snowflake/fixture/README.md)

**4. [First-Party Measurement Assurance](https://github.com/rlbsem/first-party-measurement-assurance)**

Attribution breaks when browser events are lost or sales milestones are treated as collected revenue. This implementation combines consent-aware events, GTM data layers, durable offline conversion receipts and SQL/dbt reconciliation. **Native BigQuery queries** against Google's public GA4 sample distinguished 14 purchase events from 57 nested item rows and retained two revenue discrepancies. The Google sample and local synthetic business scenarios are documented separately.

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
