# AI Enterprise Engineering

Building production AI systems for enterprise — RAG pipelines, ERP integrations, LLM agents, and observability infrastructure.

> **Summer 2026 build log** — architecting an AI Financial Operations Copilot from the ground up, documenting every layer.

---

## What I'm building

A local-first **AI Financial Operations Copilot** connected to ERPNext that helps companies analyze financial operations, retrieve accounting documents, detect anomalies, and automate procurement workflows.

Not a chatbot demo. A production system with real architecture decisions behind it.

---

## Roadmap

| Phase | Period | Focus | Status |
|---|---|---|---|
| 1 — Engineering Core | May 24 – Jun 20 | FastAPI · PostgreSQL · Docker · CI/CD | 🔨 In progress |
| 2 — RAG Engineering | Jun 21 – Jul 18 | Embeddings · Qdrant · Hybrid search · Evaluation | ⏳ Upcoming |
| 3 — Agents + LLMOps | Jul 19 – Aug 8 | PydanticAI · LangGraph · Langfuse · Observability | ⏳ Upcoming |
| 4 — Final MVP | Aug 9 – Aug 24 | ERPNext integration · Full system · Deployment | ⏳ Upcoming |

---

## Projects

### [`backend-foundation`](https://github.com/ai-enterprise-engineering/backend-foundation)
Production-grade API template used as the base for all projects in this organization.
FastAPI · SQLAlchemy · Alembic · PostgreSQL · Redis · Docker · GitHub Actions · pytest

### [`financial-rag-system`](https://github.com/ai-enterprise-engineering/financial-rag-system)
Financial document intelligence — upload invoices and reports, run semantic search, get cited answers.
OpenAI SDK · Qdrant · pgvector · Hybrid search · PDF OCR · RAG evaluation

### [`procurement-agent`](https://github.com/ai-enterprise-engineering/procurement-agent)
Agentic pipeline: parse invoices → extract structured data → compare suppliers → draft ERP actions.
PydanticAI · LangGraph · Structured outputs · Tool calling

### [`llmops-dashboard`](https://github.com/ai-enterprise-engineering/llmops-dashboard)
Observability layer for LLM systems — token cost, latency, retrieval quality, agent traces.
Langfuse · OpenTelemetry · Grafana · Prometheus

### [`erp-ai-copilot`](https://github.com/ai-enterprise-engineering/erp-ai-copilot)
Final MVP — all services integrated into a deployable AI copilot for financial operations.
ERPNext · Frappe · FastAPI · RAG · Agents · Docker Compose

---

## Stack

**Backend** — Python · FastAPI · SQLAlchemy · PostgreSQL · Redis  
**AI** — OpenAI SDK · PydanticAI · LangGraph · Qdrant · pgvector  
**Infra** — Docker · Docker Compose · Nginx · GitHub Actions  
**Observability** — OpenTelemetry · Grafana · Langfuse · Prometheus  
**Enterprise** — ERPNext · Frappe  

---

## Engineering principles

Every repo in this organization follows the same standards:

- Clean architecture — `api/`, `domain/`, `services/`, `infrastructure/` separation
- One-command local setup via `docker-compose up`
- CI/CD on every PR — lint, test, build
- Architecture diagrams updated weekly in `docs/`
- No notebooks in production paths

---

*Building publicly. Last updated: May 2026.*
