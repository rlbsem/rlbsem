# Richard Butts

**Enterprise MarTech & Systems Architecture · GTM & Revenue Systems · Data & Analytics Engineering · Applied AI**

I architect and build governed systems across customer data, CRM, MarTech, revenue operations, analytics, and AI. My work connects commercial definitions to technical controls: canonical identity, field ownership, source provenance, durable state, reconciliation, and recovery when systems disagree or fail.

**Professional Experience & Engineering Scope:** My background combines enterprise ecommerce and B2B SaaS leadership with approximately 30 systems and data engagements through Groundbreakers, primarily across PE-backed, multi-brand operating environments. My work spans MarTech and GTM architecture, enterprise integrations, customer data infrastructure, analytics engineering, revenue integrity, and AI-enabled systems. I combine technical strategy and stakeholder leadership with hands-on architecture, Python, SQL, APIs, data modeling, implementation, and engineering governance.

**Connect:** [LinkedIn](https://www.linkedin.com/in/rbutts/)

## Explore by Engineering Discipline

Follow the engineering evidence most relevant to your role; the systems below use inspectable implementations, documented execution, and explicit verification boundaries.

- **Senior MarTech / Marketing Technology:** [First-Party Measurement Assurance](https://github.com/rlbsem/first-party-measurement-assurance) · [Customer Signal & Activation](https://github.com/rlbsem/customer-signal-activation) · [Temporal Customer Audiences](https://github.com/rlbsem/temporal-customer-audiences)
- **GTM Engineering / Revenue Systems:** [Customer Signal & Activation](https://github.com/rlbsem/customer-signal-activation) · [Enterprise MarTech / AI Control Plane](https://github.com/rlbsem/enterprise-martech-ai-control-plane) · [Enterprise Revenue Systems Lab](https://github.com/rlbsem/enterprise-revenue-systems-lab)
- **Marketing Data / Data Architecture:** [First-Party Measurement Assurance](https://github.com/rlbsem/first-party-measurement-assurance) · [MarTech Data Reliability](https://github.com/rlbsem/martech-data-reliability) · [Revenue Metrics Platform](https://github.com/rlbsem/revenue-metrics-platform)
- **Enterprise Integration / Systems Architecture:** [Enterprise MarTech / AI Control Plane](https://github.com/rlbsem/enterprise-martech-ai-control-plane) · [MarTech Migration Assurance](https://github.com/rlbsem/martech-migration-assurance) · [MarTech Estate Impact](https://github.com/rlbsem/martech-estate-impact)
- **Senior Analytics Engineering:** [Revenue Metrics Platform](https://github.com/rlbsem/revenue-metrics-platform) · [MarTech Data Reliability](https://github.com/rlbsem/martech-data-reliability) · [First-Party Measurement Assurance](https://github.com/rlbsem/first-party-measurement-assurance)
- **Applied AI / AI Systems Engineering:** [Enterprise Agent Runtime & Evaluation](https://github.com/rlbsem/enterprise-agent-runtime-evaluation) · [Customer Signal & Activation](https://github.com/rlbsem/customer-signal-activation) · [Enterprise MarTech / AI Control Plane](https://github.com/rlbsem/enterprise-martech-ai-control-plane)
- **Director-Level Technical-Commercial Leadership:** [MarTech Estate Impact](https://github.com/rlbsem/martech-estate-impact) · [Revenue Metrics Platform](https://github.com/rlbsem/revenue-metrics-platform) · [Enterprise MarTech / AI Control Plane](https://github.com/rlbsem/enterprise-martech-ai-control-plane)

## Selected Engineering Implementations

Three implementation-focused entry points spanning revenue and GTM systems, enterprise integration, and analytics engineering. Each repository links to architecture, executed tests, and technical evidence.

**1. [Customer Signal & Activation](https://github.com/rlbsem/customer-signal-activation)**  
**Problem:** Marketing, CRM, sales and finance can disagree about customer identity, appropriate sales actions and whether a deal produced collected cash. **System:** Consent-aware signals, verified accounts, intent and fit, ownership-safe activation, AI-assisted seller review and fulfillment-to-cash reconciliation. **Benefit:** Commercial decisions become traceable without treating scores or Closed Won opportunities as proof of cash. Includes a **real Salesforce Developer Edition API integration** tested with restricted synthetic review records, permissions, idempotency and failure recovery. [Native Salesforce evidence](https://github.com/rlbsem/customer-signal-activation/blob/main/docs/evidence/salesforce-native/README.md).

**2. [Enterprise MarTech / AI Control Plane](https://github.com/rlbsem/enterprise-martech-ai-control-plane)**  
**Problem:** Connected platforms can overwrite correct data, repeat uncertain actions or let AI act beyond its authority. **System:** Python/PostgreSQL governance for canonical identity, field ownership, consent, lifecycle changes, durable workflows, approvals and exceptions. **Benefit:** Integration failures can be recovered without silently rewriting authoritative state or duplicating effects. Includes executed recovery evidence and AWS deployment architecture. [Inspect the architecture](https://github.com/rlbsem/enterprise-martech-ai-control-plane/blob/main/docs/architecture.md).

**3. [Revenue Metrics Platform](https://github.com/rlbsem/revenue-metrics-platform)**  
**Problem:** Marketing sees pipeline, sales sees bookings and finance sees invoices or cash—different measures on different timelines. **System:** Governed SQL/dbt dimensional models, historical state, metric definitions and reconciliation bridges. **Benefit:** Commercial discrepancies become explainable with shared definitions and traceable sources. **Native Snowflake fixture acceptance passed** across three builds (15 models and 30 tests each); the larger synthetic enterprise scenario is locally validated, not cloud-benchmarked. [Snowflake execution evidence](https://github.com/rlbsem/revenue-metrics-platform/blob/main/docs/evidence/snowflake/fixture/README.md).

## Seven more enterprise systems

Together with the three implementations above, these make up **ten core engineering projects**. Each addresses a different enterprise failure or decision.

- **[First-Party Measurement Assurance](https://github.com/rlbsem/first-party-measurement-assurance)** — **Problem:** Browser and offline conversions can conflate signed contract value with actual deposits and payments. **System:** Consent-aware browser events, GTM-compatible data layers, source-authorized offline conversions and SQL/dbt reconciliation. **Benefit:** Missing, duplicated and overstated conversions become traceable. **Native BigQuery Studio execution** against Google's public GA4 sample confirmed 14 purchases versus 57 nested item rows, with two revenue disagreements preserved. [Google execution evidence](https://github.com/rlbsem/first-party-measurement-assurance/blob/main/docs/evidence/google-bigquery/README.md) · [Passing Windows/Linux CI](https://github.com/rlbsem/first-party-measurement-assurance/actions/runs/39007934132).
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
