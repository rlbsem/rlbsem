# Richard Butts

**MarTech & Data Architecture · GTM & Revenue Systems · Integration & Migration · AI Systems**

I design and build governed systems across marketing technology, customer data, GTM and revenue operations, analytics, integrations, and AI. My work connects business definitions to technical control: canonical identity, source-of-truth rules, data quality, APIs, migration, reconciliation, and automation that can be trusted when systems disagree or fail.

My background spans enterprise ecommerce, B2B SaaS, and multi-brand operating environments, so I approach architecture from both sides: **how the systems work technically and how they affect acquisition, pipeline, attribution, revenue, and operating decisions.**

## Selected engineering work

Eight independent, executable portfolio implementations. Each uses synthetic data, links to reproducible evidence, and separates demonstrated behavior from production claims and known limitations.

| Project | Architecture problem | What the implementation demonstrates |
|---|---|---|
| **[Revenue Metrics Platform](https://github.com/rlbsem/revenue-metrics-platform)** | How can Marketing, Sales and Finance use consistent, explainable commercial metrics when pipeline, bookings, invoicing, cash and ARR represent different economic events? | Deterministic synthetic enterprise modeling at approximately $755M period-end ARR, dbt dimensional models with explicit fact grains and SCD2 history, governed commercial metrics, incremental/full-build equivalence, reconciliation, Streamlit and analyst consumption, CI/testing, and a Snowflake-ready execution path. |
| **[MarTech Data Reliability](https://github.com/rlbsem/martech-data-reliability)** | Can Marketing trust reporting when source feeds arrive late, repeat, change schema, or correct prior periods? | Content-addressed ingestion, closed data contracts, quarantine and rejection, revision-aware corrections, cross-grain SQL aggregation, freshness and reference gates, crash recovery, controlled backfills, independent reconciliation, and atomic publication. |
| **[Enterprise MarTech / AI Control Plane](https://github.com/rlbsem/enterprise-martech-ai-control-plane)** | Who owns customer truth, and what may an agent or workflow change? | Canonical identity, provenance and field authority, consent and approval boundaries, PostgreSQL-backed durable execution, idempotent downstream effects, retries, uncertain-result recovery, and audit trails. |
| **[MarTech Migration Assurance](https://github.com/rlbsem/martech-migration-assurance)** | Can we replace a platform without losing meaning or making rollback unsafe? | Consistent snapshots and change catch-up, versioned schema mappings, independent semantic reconciliation, evidence-bound cutover, process-crash recovery, reverse migration, and explicit rollback blockers. |
| **[Temporal Customer Audiences](https://github.com/rlbsem/temporal-customer-audiences)** | Who belonged in an audience at a given time, based on what we knew then? | Bitemporal customer facts, immutable original and restated audience decisions, time-driven expiry, selective reevaluation, coverage-gated activation, and destination reconciliation. |
| **[MarTech Estate Impact](https://github.com/rlbsem/martech-estate-impact)** | Before we retire or replace a marketing platform, what actually depends on it? | Evidence-backed estate reconstruction, provenance and conflict handling, typed dependencies, three-state impact analysis, counterfactual retirement/replacement, witness paths, and prerequisite sequencing across a synthetic 24-system estate. |
| **[Enterprise Agent Runtime & Evaluation](https://github.com/rlbsem/enterprise-agent-runtime-evaluation)** | How do we evaluate an agent and govern release rather than trusting its output? | Actual local LLM inference, evidence-grounded tool decisions, adversarial tests, regression gates, shadow/canary evaluation, observable rollback, and transparent reporting of failed model behavior. |
| **[MarTech Stack Economics](https://github.com/rlbsem/martech-stack-economics)** | How do we reduce integration cost without breaking freshness, capacity, or data requirements? | Mixed-integer configuration planning across shared fees, partial batches, API quotas, regional and capability constraints, and demand spikes. An independent accountant checks the solution; exhaustive enumeration confirms the optimum across 3,125 synthetic configurations. |

**Start with the problem closest to your team:** [commercial metrics and analytics engineering](https://github.com/rlbsem/revenue-metrics-platform), [data reliability and reconciliation](https://github.com/rlbsem/martech-data-reliability), [AI governance and controlled execution](https://github.com/rlbsem/enterprise-martech-ai-control-plane), [platform migrations](https://github.com/rlbsem/martech-migration-assurance), [customer data and audience correctness](https://github.com/rlbsem/temporal-customer-audiences), [estate discovery and change impact](https://github.com/rlbsem/martech-estate-impact), [agent testing and release](https://github.com/rlbsem/enterprise-agent-runtime-evaluation), or [stack optimization and cost](https://github.com/rlbsem/martech-stack-economics).

### The architecture questions behind the work

```mermaid
flowchart LR
    A[Business requirements] --> Q[Commercial metrics and analytics]
    A --> L[Estate impact and dependencies]
    A --> B[Stack economics]
    A --> E[Migration assurance]
    A --> C[Customer state governance]
    A --> R[Data reliability]
    A --> D[Agent runtime and evaluation]
    A --> F[Temporal audiences]

    Q --> O[Governed revenue measures and consumption]
    L --> M[Defensible change scope and prerequisites]
    B --> G[Defensible platform and cost choices]
    E --> J[Verified cutover and rollback]
    C --> H[Controlled data and automation]
    R --> N[Reconciled reporting and lineage]
    D --> I[Evidence-based agent releases]
    F --> K[Auditable audience decisions]

    classDef source fill:#dbeafe,stroke:#2563eb,color:#0f172a,stroke-width:2px;
    classDef capability fill:#93c5fd,stroke:#1e40af,color:#0f172a,stroke-width:2px;
    classDef output fill:#2563eb,stroke:#1e3a8a,color:#ffffff,stroke-width:2px;

    class A source;
    class B,C,D,E,F,L,Q,R capability;
    class G,H,I,J,K,M,N,O output;
```

*This is a map of independent engineering capabilities, not a claim that these eight repositories form one deployed production system.*

## Professional context

My background spans enterprise ecommerce, B2B SaaS, **MarTech and data architecture, GTM and revenue systems, analytics, and enterprise integration** across **Lorex Technology, LMN (Landscape Management Network), and Groundbreakers Digital**.

- **Enterprise ecommerce and commercial scale:** Managed more than **$65M in paid media and marketing investment** across my career. At Lorex, annual ecommerce revenue grew from approximately **$55M to $101M during my tenure**, while my work expanded across acquisition, attribution, web analytics, ecommerce, executive reporting, and enterprise marketing systems.
- **B2B SaaS and GTM systems:** At LMN, managed acquisition and performance analysis across an approximately **$350K/month USD multi-product program**, with CAC improvements of approximately **15–25%**. The environment included Salesforce, Pardot, Salesforce Marketing Cloud, GA/GA4, GTM, pipeline measurement, and recurring executive product reporting.
- **Data architecture and systems delivery:** Founded Groundbreakers Digital and led architecture and systems delivery across roughly **30 projects** for founder-owned and private-equity-backed businesses. The work spans canonical customer identity, source-of-truth governance, attribution, CRM and operating-system integration, finance/revenue reconciliation, APIs and webhooks, ETL/ELT, stateful middleware, idempotency, retry and exception handling, audit logging, multi-brand data architecture, and AI-driven workflows.
- **AI and automation:** Working with LLMs and AI systems since **2023**, building on longer-standing experience in marketing automation, analytics, integration, customer data, and governed workflow design.

**Professional systems and platforms:** Salesforce · HubSpot · Pardot · Salesforce Marketing Cloud · Marketo · Segment · Clay · Snowflake · GA4 / GTM · Adobe Analytics · Tableau · PostgreSQL · Supabase · QuickBooks Online · REST APIs · webhooks · ETL / ELT · Make · n8n · Workato · Zapier

**Technologies demonstrated in the public engineering work:** Python · SQL · dbt Core · PostgreSQL · DuckDB · SQLite · Streamlit · FastAPI · Airflow · SciPy / HiGHS · Docker · GitHub Actions · HTTP / REST · local LLM inference

## How to review the work

Each repository has a runnable entry point, documented architecture and assumptions, tests, generated evidence, and explicit limitations. The projects are **independent synthetic portfolio implementations**, not representations of client production data or claims of live vendor integrations. Professional experience and portfolio demonstrations are presented separately.

The underlying theme is straightforward: **tools execute; the control layer determines what is allowed to become true.**

[GitHub profile](https://github.com/rlbsem) · **Groundbreakers Digital:** Data Infrastructure · Revenue Integrity · M&A Systems Architecture
