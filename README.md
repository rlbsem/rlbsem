# Richard Butts

**MarTech & Data Architecture · GTM & Revenue Systems · Integration & Migration · AI Systems**

I design and build governed systems across marketing technology, customer data, GTM and revenue operations, analytics, integrations, and AI. My work connects business definitions to technical control: canonical identity, source-of-truth rules, data quality, APIs, migration, reconciliation, and automation that can be trusted when systems disagree or fail.

My background spans enterprise ecommerce, B2B SaaS, and multi-brand operating environments, so I approach architecture from both sides: **how the systems work technically and how they affect acquisition, pipeline, attribution, revenue, and operating decisions.**

**Commercial delivery context:** At Lorex, annual ecommerce revenue grew from approximately **$55M to $101M during my tenure**. At LMN, I managed approximately **$350K/month** in multi-product B2B SaaS acquisition with **15–25% CAC improvement**. Through Groundbreakers, I've led roughly **30 systems and data engagements**—approximately **80% supporting operating brands within PE-backed portfolios**, with much of the remainder involving founder-led, multi-brand holding companies.

## Featured engineering systems

**[Enterprise MarTech / AI Control Plane](https://github.com/rlbsem/enterprise-martech-ai-control-plane)** — Python and PostgreSQL control architecture for customer identity, field authority, durable processing, idempotency, crash recovery, audited exceptions and governed AI actions.

**[Customer Signal & Activation](https://github.com/rlbsem/customer-signal-activation)** — B2B account signals, verified enrichment, sales routing and CRM activation, plus a live Qwen3-14B seller workbench with source-linked evidence and approval-bound actions.

**[Revenue Metrics Platform](https://github.com/rlbsem/revenue-metrics-platform)** — SQL/dbt dimensional models, temporal history, ARR/bookings/invoicing/cash reconciliation, testable finance definitions and analytical review.

**Interactive evidence:** [Open Enterprise Revenue Systems Lab](https://rlbsem.github.io/enterprise-revenue-systems-lab/) ([source and reproduction](https://github.com/rlbsem/enterprise-revenue-systems-lab)) — a published browser explorer for seller decisions, uncertain API outcomes and commercial reconciliation. The Pages deployment passed; browser smoke-testing is still pending.

## Find the right engineering evidence

| If you're reviewing... | Start with | What you can verify |
|---|---|---|
| **AI-enabled GTM and seller productivity** | [Customer Signal & Activation](https://github.com/rlbsem/customer-signal-activation) · [Seller Workbench results](https://github.com/rlbsem/customer-signal-activation/blob/main/docs/evidence/seller/report.md) | Account evidence, local Qwen3-14B inference, guided recommendations, approval and CRM effects |
| **Enterprise systems and integration architecture** | [MarTech / AI Control Plane](https://github.com/rlbsem/enterprise-martech-ai-control-plane) · [Architecture](https://github.com/rlbsem/enterprise-martech-ai-control-plane/blob/main/docs/architecture.md) | Canonical identity, field ownership, PostgreSQL work queues, idempotency, failure recovery and cloud architecture |
| **Revenue analytics and data engineering** | [Revenue Metrics Platform](https://github.com/rlbsem/revenue-metrics-platform) · [dbt models](https://github.com/rlbsem/revenue-metrics-platform/tree/main/dbt/models) | Fact grains, temporal dimensions, governed metrics, finance bridges and reconciliation |
| **M&A, migration and platform change** | [Migration Assurance](https://github.com/rlbsem/martech-migration-assurance) · [Estate Impact](https://github.com/rlbsem/martech-estate-impact) | Provenance, dependency impact, cutover controls, semantic parity and rollback safety |
| **Data quality, temporal state and operational reliability** | [Data Reliability](https://github.com/rlbsem/martech-data-reliability) · [Temporal Audiences](https://github.com/rlbsem/temporal-customer-audiences) | Late or corrected records, immutable history, publication gates, selective reevaluation and destination reconciliation |

**Prefer a guided review?** The [Enterprise Revenue Systems Lab](https://github.com/rlbsem/enterprise-revenue-systems-lab) brings together inspectable evidence from three separate engines so you can follow a seller decision, an uncertain API outcome and a revenue discrepancy from source to result.

## Architecture at a glance

[View the capability map](assets/capability-map.svg) — nine core engineering implementations organized by the questions they answer: commercial metrics, GTM and control, enterprise change, and AI/data assurance.

## Selected engineering work

The table below highlights nine core engineering implementations, with a separate interactive Lab for exploring selected execution evidence.

| Project | Architecture problem | What the implementation demonstrates |
|---|---|---|
| **[Revenue Metrics Platform](https://github.com/rlbsem/revenue-metrics-platform)** | How can Marketing, Sales and Finance use consistent, explainable commercial metrics when pipeline, bookings, invoicing, cash and ARR represent different economic events? | Deterministic synthetic enterprise modeling at approximately $755M period-end ARR, dbt dimensional models with explicit fact grains and SCD2 history, governed commercial metrics, incremental/full-build equivalence, reconciliation, Streamlit and analyst consumption, CI/testing, and a Snowflake-ready execution path. |
| **[Customer Signal & Activation](https://github.com/rlbsem/customer-signal-activation)** | Which customer signals warrant seller action, and can the outcome be traced to collected cash? | Live Qwen3-14B seller workbench with source-linked account briefs, editable drafts and approval-bound durable CRM tasks; controlled identity, enrichment, consent, ownership and uncertain-result recovery; dbt-validated fulfillment-to-invoice-to-cash lineage and synthetic comparative model evaluation. |
| **[Enterprise MarTech / AI Control Plane](https://github.com/rlbsem/enterprise-martech-ai-control-plane)** | Who owns customer truth, and what may an agent or workflow change? | Customer-state authority and durable execution; Terraform AWS architecture with ECS/Fargate, RDS PostgreSQL and scoped IAM/OIDC; immutable releases and rollback, recovery reconciliation, and validated enterprise workloads. |
| **[MarTech Data Reliability](https://github.com/rlbsem/martech-data-reliability)** | Can Marketing trust reporting when source feeds arrive late, repeat, change schema, or correct prior periods? | Content-addressed ingestion, closed data contracts, quarantine and rejection, revision-aware corrections, cross-grain SQL aggregation, freshness and reference gates, crash recovery, controlled backfills, independent reconciliation, and atomic publication. |
| **[MarTech Migration Assurance](https://github.com/rlbsem/martech-migration-assurance)** | Can we replace a platform without losing meaning or making rollback unsafe? | Consistent snapshots and change catch-up, versioned schema mappings, independent semantic reconciliation, evidence-bound cutover, process-crash recovery, reverse migration, and explicit rollback blockers. |
| **[Temporal Customer Audiences](https://github.com/rlbsem/temporal-customer-audiences)** | Who belonged in an audience at a given time, based on what we knew then? | Bitemporal customer facts, immutable original and restated audience decisions, time-driven expiry, selective reevaluation, coverage-gated activation, and destination reconciliation. |
| **[Enterprise Agent Runtime & Evaluation](https://github.com/rlbsem/enterprise-agent-runtime-evaluation)** | How do we evaluate an agent and govern release rather than trusting its output? | Actual local LLM inference, evidence-grounded tool decisions, adversarial tests, regression gates, shadow/canary evaluation, observable rollback, and transparent reporting of failed model behavior. |
| **[MarTech Estate Impact](https://github.com/rlbsem/martech-estate-impact)** | Before we retire or replace a marketing platform, what actually depends on it? | Evidence-backed estate reconstruction, provenance and conflict handling, typed dependencies, three-state impact analysis, counterfactual retirement/replacement, witness paths, and prerequisite sequencing across a synthetic 24-system estate. |
| **[MarTech Stack Economics](https://github.com/rlbsem/martech-stack-economics)** | How do we reduce integration cost without breaking freshness, capacity, or data requirements? | Mixed-integer configuration planning across shared fees, partial batches, API quotas, regional and capability constraints, and demand spikes. An independent accountant checks the solution; exhaustive enumeration confirms the optimum across 3,125 synthetic configurations. |

## Professional context

My background spans enterprise ecommerce, B2B SaaS, **MarTech and data architecture, GTM and revenue systems, analytics, and enterprise integration** across **Lorex Technology, LMN (Landscape Management Network), and Groundbreakers Digital**.

- **Enterprise ecommerce and commercial scale:** Managed more than **$65M in paid media and marketing investment** across my career. At Lorex, annual ecommerce revenue grew from approximately **$55M to $101M during my tenure**, while my work expanded across acquisition, attribution, web analytics, ecommerce, executive reporting, and enterprise marketing systems.
- **B2B SaaS and GTM systems:** At LMN, managed acquisition and performance analysis across an approximately **$350K/month multi-product program**, with CAC improvements of approximately **15–25%**. The environment included Salesforce, Pardot, Salesforce Marketing Cloud, GA/GA4, GTM, pipeline measurement, and recurring executive product reporting.
- **Data architecture and systems delivery:** Founded Groundbreakers Digital and led architecture and systems delivery across roughly **30 projects** for founder-owned and private-equity-backed businesses. Much of that work connects acquired or independently run brands into shared CRM, operations, finance, and reporting infrastructure. The work spans canonical customer identity, source-of-truth governance, attribution, CRM and operating-system integration, finance/revenue reconciliation, APIs and webhooks, ETL/ELT, stateful middleware, idempotency, retry and exception handling, audit logging, multi-brand data architecture, and AI-driven workflows.
- **AI and automation:** Working with LLMs and AI systems since **2023**, building on longer-standing experience in marketing automation, analytics, integration, customer data, and governed workflow design.

**Professional systems and platforms:** Salesforce · HubSpot · Pardot · Salesforce Marketing Cloud · Marketo · Segment · Clay · Snowflake · GA4 / GTM · Adobe Analytics · Tableau · PostgreSQL · Supabase · QuickBooks Online · REST APIs · webhooks · ETL / ELT · Make · n8n · Workato · Zapier

**Technologies demonstrated in the public engineering work:** Python · SQL · dbt Core · PostgreSQL · DuckDB · SQLite · Streamlit · FastAPI · Airflow · SciPy / HiGHS · Docker · GitHub Actions · Terraform · AWS (ECS/Fargate, RDS, ECR, Secrets Manager, CloudWatch, IAM/OIDC) · HTTP / REST · local LLM inference

## How to review the work

The engineering repositories include runnable implementations, architecture notes, tests and execution evidence. Start with the interactive Lab or an implementation's validation results, then follow the code and diagrams. These public, synthetic and vendor-neutral implementations make architecture patterns used in Groundbreakers client work inspectable without publishing private client systems or data; they are not claims that the exact repositories were deployed unchanged into client production.

The underlying theme is straightforward: **tools execute; the control layer determines what is allowed to become true.**

[GitHub profile](https://github.com/rlbsem) · **Groundbreakers Digital:** Data Infrastructure · Revenue Integrity · M&A Systems Architecture
