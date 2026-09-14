# Richard Butts

**AI Systems Architecture · Data Architecture · MarTech / GTM Systems · Analytics Engineering · Enterprise Integration**

I design and build analytics, MarTech, GTM, AI, and enterprise integration systems with an emphasis on governed state, data quality, reliable automation, evaluation, and measurable business outcomes.

My work sits where software behavior meets business truth: what happened, what state is authoritative, what an automated system is allowed to change, whether an AI agent is actually safe and better enough to release, and whether a critical platform can be replaced without destroying meaning or reversibility.

## Selected engineering work

| Project | What it demonstrates |
|---|---|
| **[Enterprise Agent Runtime & Evaluation](https://github.com/rlbsem/enterprise-agent-runtime-evaluation)** | Agent regression testing, actual local LLM inference, structured tool decisions, evidence grounding, prompt-injection/adversarial evaluation, release gating, shadow/canary evaluation, rollback, runtime observability, and cross-platform CI. |
| **[MarTech Migration Assurance](https://github.com/rlbsem/martech-migration-assurance)** | System replacement, consistent snapshots, incremental change transfer, versioned mappings, semantic reconciliation, evidence-bound cutover, crash recovery, reverse migration, rollback safety, and cross-platform CI. |
| **[Enterprise MarTech / AI Control Plane](https://github.com/rlbsem/enterprise-martech-ai-control-plane)** | Governed customer identity, source and field authority, consent, AI action boundaries, human approval, durable execution, retries, uncertain-result recovery, idempotent downstream effects, auditability, PostgreSQL, FastAPI, Docker, and CI. |
| **[Game Telemetry Analytics Engineering](https://github.com/rlbsem/game-telemetry-analytics-engineering)** | Python, DuckDB, dbt, Airflow, event contracts, transactional ingestion, late-arriving telemetry, incremental models, replay validation, launch monitoring, testing, and CI. |

These are executable portfolio systems, not architecture-only case studies. Each repository separates demonstrated behavior from reference architecture, preserves unfavorable results where they matter, and documents its claim boundary and known limitations.

### Portfolio thesis

1. **Analytics truth:** What happened in the product?
2. **Governed enterprise truth:** What business state is authoritative, and what is automation allowed to make true?
3. **Agent-quality truth:** Is a candidate AI agent grounded, safe, and better enough to release?
4. **Migration truth:** Can a critical platform be replaced without losing meaning or reversibility?

## Architecture themes

```mermaid
flowchart LR
    A[Events / enterprise systems] --> B[Identity + provenance]
    B --> C[Governed state]
    C --> D[Reasoning + policy]
    D --> E[Controlled execution]
    E --> F[Evaluation + evidence]
    F --> G[Defensible business truth]
```

**Systems concerns:** canonical identity · source provenance · field ownership · source-of-truth governance · No-Regress Logic · durable state · idempotency · retries and exception handling · controlled AI actions · agent evaluation · adversarial testing · migration assurance · cutover and rollback safety · auditability · cross-system reconciliation

**Core technologies demonstrated here:** Python · SQL · PostgreSQL · FastAPI · SQLite / FTS5 · dbt · DuckDB · Airflow · Docker · GitHub Actions · REST APIs · webhooks · local LLM inference

## Professional context

My background spans **Lorex Technology, LMN (Landscape Management Network), and Groundbreakers Digital** across analytics, digital growth, RevOps, GTM systems, MarTech, data architecture, and enterprise systems.

At Lorex, annual ecommerce revenue grew from approximately **$55M to $101M** during my tenure. At LMN, I worked across an approximately **$350K/month USD acquisition program** spanning five B2B SaaS products, with CAC improvements of approximately **15–25%**.

At Groundbreakers Digital, I work on data infrastructure, revenue integrity, and M&A systems architecture for home-services and acquisition environments. The focus is not moving data for its own sake. It is governing identity, commercial state, source provenance, reconciliation, and system boundaries so operating and transaction data can be defended.

## Current focus

The portfolio is intentionally small. I would rather publish a few systems that can survive technical scrutiny than a large collection of toy projects.

Current areas of focus include:

- enterprise AI runtime, evaluation, and release governance
- MarTech / GTM architecture and governed automation
- analytics engineering and behavioral telemetry
- platform replacement, cutover, rollback, and migration assurance
- CRM → operations → billing → GL traceability
- revenue integrity and cross-system reconciliation
- post-acquisition integration and governed data migration

## Contact

- GitHub: [@rlbsem](https://github.com/rlbsem)
- Groundbreakers Digital: Data Infrastructure · Revenue Integrity · M&A Systems Architecture

I am especially interested in senior roles spanning **AI systems architecture, MarTech / GTM architecture, analytics engineering, data architecture, RevOps systems, and enterprise integration**.
