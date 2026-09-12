# Richard Butts

**Data Architecture · MarTech Systems · AI Governance · Analytics Engineering · Enterprise Integration**

I build systems that determine what customer, commercial, and operational data is actually allowed to become true.

My work sits at the intersection of analytics engineering, enterprise MarTech architecture, AI/agent control systems, GTM infrastructure, and revenue-integrity architecture. I care about canonical identity, source authority, durable state, auditability, idempotency, failure recovery, and making cross-system truth defensible.

> **Signal vs. Noise.** The tools can execute. The control layer determines what is actually true.

## Selected engineering work

| Project | What it demonstrates |
|---|---|
| **[Enterprise MarTech / AI Control Plane](https://github.com/rlbsem/enterprise-martech-ai-control-plane)** | Governed customer identity, field authority, consent, AI action boundaries, human approval, durable execution, retries, uncertain-result recovery, auditability, Docker, PostgreSQL, FastAPI, and CI. |
| **[Game Telemetry Analytics Engineering](https://github.com/rlbsem/game-telemetry-analytics-engineering)** | Python, DuckDB, dbt, Airflow, event contracts, transactional ingestion, late-arriving telemetry, incremental models, launch monitoring, replay validation, testing, and CI. |

These are executable portfolio systems, not architecture-only case studies. Each repository separates what was actually run and tested from production-reference design and explicitly documents known limits.

## What I work on

```mermaid
flowchart LR
    A[Source systems / events] --> B[Identity + provenance]
    B --> C[Governed state]
    C --> D[Policy + validation]
    D --> E[Controlled execution]
    E --> F[Auditable business truth]
```

**Architecture themes:** canonical customer/entity identity · source provenance · field ownership · source-of-truth governance · No-Regress Logic · stateful middleware · idempotency · exception/retry handling · controlled AI actions · audit logging · cross-system reconciliation

**Core technologies demonstrated here:** Python · SQL · PostgreSQL · FastAPI · dbt · DuckDB · Airflow · Docker · GitHub Actions · REST APIs · webhooks

## Professional context

My background spans **Lorex Technology, LMN (Landscape Management Network), and Groundbreakers Digital**, across digital growth, analytics, RevOps, GTM systems, data architecture, and enterprise systems.

At **Groundbreakers Digital**, I work on Data Infrastructure, Revenue Integrity, and M&A Systems Architecture for home-services and acquisition environments. The focus is not moving data for its own sake. It is governing identity, commercial state, source provenance, and system boundaries so the resulting operating data can be trusted.

## Current portfolio direction

The portfolio is intentionally small. I would rather publish a few systems that can survive technical scrutiny than a large collection of toy projects.

Current focus areas include:

- enterprise MarTech and AI control architecture
- analytics engineering and event/data quality
- CRM → operations → billing → GL traceability
- revenue integrity and cross-system reconciliation
- post-acquisition integration and governed data migration

## Contact

- GitHub: [@rlbsem](https://github.com/rlbsem)
- Groundbreakers Digital: Data Infrastructure · Revenue Integrity · M&A Systems Architecture

I am especially interested in senior roles spanning **MarTech architecture, AI systems, analytics engineering, data architecture, GTM/RevOps systems, and enterprise integration**.
