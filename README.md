# Richard Butts

**MarTech & Data Architecture · Enterprise Systems & Integration · Revenue Integrity · AI Governance**

I architect and build governed systems across customer data, CRM, MarTech, revenue operations, analytics, and AI. My work connects commercial definitions to technical controls: canonical identity, field ownership, source provenance, durable state, reconciliation, and recovery when systems disagree or fail.

**GTM AI and seller engineering:** I turn account signals, enrichment and commercial context into explainable sales actions, with governed CRM ownership, permission checks, durable execution and measurable downstream outcomes.

**Connect:** [LinkedIn](https://www.linkedin.com/in/rbutts/)

## Featured engineering implementations

These are the best starting points for evaluating the architecture, implementation, and technical controls behind my work.

**1. [Customer Signal & Activation](https://github.com/rlbsem/customer-signal-activation)**  
Controlled account identity, enrichment, scoring, CRM activation, and fulfillment-to-cash feedback. Includes an actual local Qwen3-14B seller workbench, source-linked recommendations, human approval, and durable action processing. [Inspect the seller-workbench evidence](https://github.com/rlbsem/customer-signal-activation/blob/main/docs/evidence/seller/report.md).

**2. [Enterprise MarTech / AI Control Plane](https://github.com/rlbsem/enterprise-martech-ai-control-plane)**  
Python and PostgreSQL architecture for canonical identity, field authority, consent, durable execution, No-Regress Logic, idempotency, audited exceptions, and governed AI actions. Includes recovery evidence and Terraform-based AWS architecture. [Architecture and implementation details](https://github.com/rlbsem/enterprise-martech-ai-control-plane/blob/main/docs/architecture.md).

**3. [Revenue Metrics Platform](https://github.com/rlbsem/revenue-metrics-platform)**  
SQL/dbt dimensional models, SCD2 history, governed ARR and revenue definitions, bookings–invoicing–cash reconciliation, incremental/full-build equivalence, and analytical review. Built against synthetic enterprise-scale data. [Inspect the dbt models](https://github.com/rlbsem/revenue-metrics-platform/tree/main/dbt/models).

**Optional interactive walkthrough:** [Enterprise Revenue Systems Lab](https://rlbsem.github.io/enterprise-revenue-systems-lab/) ([source and reproduction](https://github.com/rlbsem/enterprise-revenue-systems-lab)) — a browser-based review of recorded synthetic evidence from three independent engines: AI seller decisions, uncertain workflow recovery, and revenue reconciliation. Fresh engine execution remains a separate local workflow.

## Additional engineering systems

Together with the three implementations above, these make up **nine core engineering projects**, organized around distinct enterprise problems.

- **[MarTech Data Reliability](https://github.com/rlbsem/martech-data-reliability)** — Contract-checked ingestion, schema changes, quarantines, late corrections, recovery, reconciliation, and atomic reporting publication.
- **[MarTech Migration Assurance](https://github.com/rlbsem/martech-migration-assurance)** — Versioned mappings, semantic parity checks, safe cutover, crash recovery, reverse migration, and evidence-bound rollback.
- **[Temporal Customer Audiences](https://github.com/rlbsem/temporal-customer-audiences)** — Bitemporal customer state, historical restatement, expiry-driven reevaluation, coverage gates, and activation reconciliation.
- **[Enterprise Agent Runtime & Evaluation](https://github.com/rlbsem/enterprise-agent-runtime-evaluation)** — Actual local LLM inference, adversarial evaluation, regression gates, shadow/canary assessment, and safe release decisions.
- **[MarTech Estate Impact](https://github.com/rlbsem/martech-estate-impact)** — System and dependency discovery with source provenance, impact analysis, and retirement/replacement planning across a synthetic enterprise estate.
- **[MarTech Stack Economics](https://github.com/rlbsem/martech-stack-economics)** — Constrained integration-cost optimization across API quotas, freshness, capacity, and capabilities, with independent solution verification.

### Architecture capability map

An at-a-glance view of the nine implementations and the enterprise problems they address:

<img src="assets/capability-map.svg" alt="Capability map showing nine engineering projects grouped by revenue and analytics, GTM and control, enterprise architecture, and temporal and AI assurance" width="880">

[View the full-size diagram](assets/capability-map.svg).

## Systems, technologies, and control patterns

**Professional platforms:** Salesforce · HubSpot · Pardot · Salesforce Marketing Cloud · Marketo · Segment · Clay · LMN · Aspire · QuickBooks · GA4 / GTM · Adobe Analytics · Tableau · Snowflake · Supabase · REST APIs · webhooks · ETL / ELT · Make · n8n · Workato · Zapier

**Engineering stack demonstrated publicly:** Python · SQL · PostgreSQL · dbt Core · DuckDB · SQLite · FastAPI · Streamlit · Airflow · Docker · GitHub Actions · Terraform · AWS architecture (ECS/Fargate, RDS, ECR, IAM/OIDC) · local LLM inference

**Architecture and governance:** canonical entity identity · source authority · field ownership · No-Regress Logic · event provenance · temporal state · stateful middleware · idempotency · retry/exception queues · audit trails · revenue reconciliation · release gates

## How to evaluate the work

Each repository provides implementation details, tests, execution evidence, and known limitations. The public systems use **synthetic or vendor-neutral data** so the architecture can be inspected without exposing private client environments. They demonstrate engineering patterns, **not a claim that any public repository was deployed unchanged into client production**.

**Professional context:** Enterprise ecommerce, multi-product B2B SaaS, and PE-backed and founder-led multi-brand operating environments.

**Tools execute. The control layer determines what is true.**
