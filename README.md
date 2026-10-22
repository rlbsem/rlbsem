# Richard Butts

**AI GTM Engineering · Enterprise Data & Systems Architecture · Applied AI · Revenue Integrity · MarTech**

I build AI-powered revenue and GTM systems that turn account signals and buyer interest into useful seller actions, connect CRM and marketing tools, and trace outcomes through pipeline and revenue. My work spans enterprise B2B SaaS, ecommerce, and founder-owned and PE-backed multi-brand operators. I write the Python, SQL, APIs and durable control logic needed when ordinary workflows cannot safely manage identity, ownership, consent, retries and system-of-record changes.

The repositories below show working code, test results and recorded execution evidence, including native Salesforce, Snowflake and BigQuery acceptance as well as actual local LLM inference. The public examples use synthetic or public sample data, with execution and commercial outcome boundaries documented.

**Start here for AI GTM engineering:** [AI Account Intelligence to Qualified Pipeline — interactive evidence](https://rlbsem.github.io/enterprise-revenue-systems-lab/?case=gtm-enterprise) · [GTM Pipeline Orchestration — code and executed proof](https://github.com/rlbsem/gtm-pipeline-orchestration) · [Enterprise Agent Runtime & Evaluation](https://github.com/rlbsem/enterprise-agent-runtime-evaluation)

**Connect:** [LinkedIn](https://www.linkedin.com/in/rbutts/)

**[Explore the full Engineering Evidence Lab](https://rlbsem.github.io/enterprise-revenue-systems-lab/).** The hosted investigation library covers AI seller decisions, GTM pipeline workflows, execution recovery, commercial reconciliation and actual native CRM/warehouse integration evidence.

## Engineering Implementations & Evidence

Five projects with detailed code, test results, and execution evidence.

**1. [GTM Pipeline Orchestration](https://github.com/rlbsem/gtm-pipeline-orchestration)**

This Python GTM system connects account research, fit/intent scoring, inbound routing, approved seller actions, and qualified-pipeline measurement. A **connected native Salesforce Developer Edition run** took a fictional buying signal through **fresh Qwen3 inference → exact seller review → one guarded Salesforce SDR Task → independent readback**, including lost-acknowledgment recovery and duplicate/authority rejection. The implementation includes **199 passing regression tests** and cross-platform CI. A separate **120-account, USD $3.46M synthetic qualified-pipeline scenario** illustrates downstream measurement; it is not real customer pipeline or AI uplift.

[Connected AI-to-Salesforce execution and architecture](https://github.com/rlbsem/gtm-pipeline-orchestration/blob/main/docs/connected-sdr.md) · [Actual Task and recovery evidence](https://github.com/rlbsem/gtm-pipeline-orchestration/blob/main/docs/evidence/connected/README.md) · [Earlier native Salesforce acceptance](https://github.com/rlbsem/gtm-pipeline-orchestration/blob/main/docs/evidence/salesforce-standard/README.md) · [Synthetic pipeline demo](https://github.com/rlbsem/gtm-pipeline-orchestration/blob/main/docs/evidence/enterprise-usd/README.md) · [Linux, Windows and container CI](https://github.com/rlbsem/gtm-pipeline-orchestration/actions/runs/39705273772)

**2. [Customer Signal & Activation](https://github.com/rlbsem/customer-signal-activation)**

This project takes customer signals into the CRM while checking identity, consent, field ownership, and approval first. It includes account verification, explainable fit and intent scoring, and fulfillment-to-cash reconciliation. In an **executed Salesforce ↔ Snowflake round-trip**, a lost Salesforce acknowledgment was recovered without creating another record. Independent read-back confirmed the effect, and CRM feedback changed the warehouse recommendation. Restricted reads and replay controls were also verified, alongside 352 passing local tests.

[Native integration evidence](https://github.com/rlbsem/customer-signal-activation/blob/main/docs/evidence/connected-integration/README.md) · [Salesforce permission and recovery tests](https://github.com/rlbsem/customer-signal-activation/blob/main/docs/evidence/salesforce-native/README.md)

**3. [Enterprise MarTech / AI Control Plane](https://github.com/rlbsem/enterprise-martech-ai-control-plane)**

This Python/PostgreSQL control plane checks canonical identity, field ownership, consent, and approval before changes move between systems. It keeps durable execution state so a retry cannot overwrite authoritative data or repeat an uncertain downstream action. Native AWS acceptance verified independent PostgreSQL receipts, duplicate safety, read-only permissions and a **retained-backup RDS restore observed available**. The restored-state fail-closed comparison was not recorded, and the production AWS architecture was not deployed.

[AWS execution and cleanup](https://github.com/rlbsem/enterprise-martech-ai-control-plane/blob/main/docs/evidence/aws-readiness/retained-two-instance/native-outcome/README.md) · [Recovery tests](https://github.com/rlbsem/enterprise-martech-ai-control-plane/blob/main/docs/evidence/report.md) · [Architecture](https://github.com/rlbsem/enterprise-martech-ai-control-plane/blob/main/docs/architecture.md)

**4. [Revenue Metrics Platform](https://github.com/rlbsem/revenue-metrics-platform)**

Bookings, invoices, collected cash, and ARR are not interchangeable. This platform uses SQL/dbt models, historical state and source-traceable reconciliation to keep those definitions consistent. **Native Snowflake acceptance** completed three fixture builds, each with 15 models and 30 tests. The larger synthetic enterprise scenario was tested locally rather than benchmarked in Snowflake.

[Snowflake execution evidence](https://github.com/rlbsem/revenue-metrics-platform/blob/main/docs/evidence/snowflake/fixture/README.md)

**5. [First-Party Measurement Assurance](https://github.com/rlbsem/first-party-measurement-assurance)**

Attribution breaks when browser events are lost or sales milestones are treated as collected revenue. This implementation combines consent-aware events, GTM data layers, durable offline conversion receipts and SQL/dbt reconciliation. **Native BigQuery queries** against Google's public GA4 sample distinguished 14 purchase events from 57 nested item rows and retained two revenue discrepancies. The Google sample and local synthetic business scenarios are documented separately.

A separate [local GA4 warehouse module](https://github.com/rlbsem/first-party-measurement-assurance/blob/main/docs/evidence/ga4-warehouse/README.md) verifies late corrections, replay safety and incremental/full-refresh parity; native dbt-bigquery remains unverified.

[BigQuery execution evidence](https://github.com/rlbsem/first-party-measurement-assurance/blob/main/docs/evidence/google-bigquery/README.md) · [Windows/Linux CI](https://github.com/rlbsem/first-party-measurement-assurance/actions/runs/39007934132)

## Six Additional Engineering Systems

Six more projects cover specific problems in data reliability, migrations, temporal history, AI evaluation, and platform governance.

- **[MarTech Data Reliability](https://github.com/rlbsem/martech-data-reliability):** Contract-checked ingestion, quarantine and correction handling keep invalid loads from replacing validated reporting data.
- **[MarTech Migration Assurance](https://github.com/rlbsem/martech-migration-assurance):** Semantic parity, change catch-up and rollback gates expose migrations that preserve row counts but alter business meaning.
- **[Temporal Customer Audiences](https://github.com/rlbsem/temporal-customer-audiences):** Business-time and knowledge-time history account for late-arriving facts, corrected eligibility and auditable past decisions.
- **[Enterprise Agent Runtime & Evaluation](https://github.com/rlbsem/enterprise-agent-runtime-evaluation):** Local model inference, adversarial evaluation, source checks and release gates provide evidence before an AI version is promoted.
- **[MarTech Estate Impact](https://github.com/rlbsem/martech-estate-impact):** Dependency evidence and explicit uncertainty make platform retirement and consolidation decisions inspectable.
- **[MarTech Stack Economics](https://github.com/rlbsem/martech-stack-economics):** Constrained optimization tests proposed savings against cost, freshness, capacity and API quotas.

### Architecture capability map

Where the projects fit across revenue systems, integration controls, enterprise architecture, and AI:

<img src="assets/capability-map.svg" alt="Capability map showing eleven engineering projects grouped by revenue and analytics, GTM and control, enterprise architecture, and temporal and AI assurance" width="880">

[View the full-size diagram](assets/capability-map.svg).

## Explore engineering in action

**[Enterprise Revenue Systems Lab](https://rlbsem.github.io/enterprise-revenue-systems-lab/): interactive evidence explorer** · [Source code](https://github.com/rlbsem/enterprise-revenue-systems-lab)

The interactive lab lets you walk through four cases:

- **AI seller decisions:** Examine a model-generated recommendation, its supporting sources, a reviewed edit, approval and recorded delivery evidence.
- **Execution recovery:** Trace a lost acknowledgment and worker interruption through durable workflow state and independent receiver receipts, including duplicate prevention.
- **Revenue reconciliation:** Explore why installed ARR, bookings, invoices and collected cash differ, with a source-backed financial bridge.
- **Native Salesforce and Snowflake:** [Inspect the CRM-to-warehouse round trip](https://rlbsem.github.io/enterprise-revenue-systems-lab/?case=connected-roundtrip), including source authority, lost-acknowledgment recovery, independent CRM readback and the resulting warehouse decision.

The hosted lab uses recorded **synthetic evidence**, not live production data. Running the underlying engines or fresh model inference requires the separate local workflows.

## Systems, technologies, and control patterns

**Enterprise platforms and business systems:** Salesforce · HubSpot · Salesforce Marketing Cloud · Marketing Cloud Account Engagement (Pardot) · Marketo · Segment · Clay · LinkedIn Sales Navigator · HighLevel (GoHighLevel) · LMN · Aspire · QuickBooks · Google Analytics 4 (GA4) · Google Tag Manager (GTM) · Adobe Analytics · Tableau · Power BI · Vapi · Dialpad · Make · n8n · Workato · Zapier

**Engineering, data platforms, and cloud:** Python · SQL · JavaScript / TypeScript · PostgreSQL · Snowflake · Supabase · dbt · DuckDB · SQLite · FastAPI · Streamlit · Airflow · Git · GitHub Actions / CI/CD · Docker · Terraform · AWS architecture (ECS/Fargate, RDS, ECR, IAM/OIDC)

**Data architecture and enterprise integration:** Dimensional modeling · SCD Type 2 · Bitemporal data · Governed metrics · Data contracts · Schema evolution · ETL / ELT · Reverse ETL / warehouse-to-CRM activation · Incremental processing · Backfills · REST APIs · Webhooks · OAuth 2.0 · Canonical identity · Entity resolution · Source lineage · GTM engineering · Lead scoring and routing · SDR/AE workflow automation · Sales engagement systems · Pipeline attribution · Meta Conversions API · Google Enhanced Conversions · Offline conversion tracking · Server-side measurement

**Reliability, governance, and AI systems:** Source authority · Field ownership · No-Regress Logic · Stateful middleware · Idempotency · Replay safety · Retry/backoff · Exception queues · RBAC · Consent governance · Audit logging · Revenue reconciliation · Failure recovery · Release gates · OpenAI / LLM APIs · Anthropic Claude · Qwen local inference · llama.cpp · Model Context Protocol (MCP) · Prompt engineering · Tool/function calling · Structured outputs · LLM evaluation · Human approval controls

## How to evaluate the work

Each repository documents its code, tests, and limits. The examples use synthetic or vendor-neutral data, and I distinguish native service execution from local tests and production deployment.

**Tools execute. The control layer determines what is true.**
