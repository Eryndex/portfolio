# ERYNDEX — Engineering Portfolio

This repository contains the ERYNDEX company website and a collection of engineering portfolio demonstrators across backend systems, applied AI, data engineering, workflow automation and web applications.

**Portfolio principle:** these projects are implementation samples for technical review. They are not presented as verified customer deployments, production service-level commitments, or independently validated commercial outcomes. Each project README documents its scope, setup and known limitations.

## Company website
- Main website: https://eryndex.net/
- Persian: https://eryndex.net/fa/
- Website source: [projects/eryndex-company-website](projects/eryndex-company-website/)
- Full company site and profile source mirror: [eryndex/](eryndex/)
- Upstream source: [arshiataheri851-ops/portfolio/eryndex](https://github.com/arshiataheri851-ops/portfolio/tree/main/eryndex)
- The `eryndex/` directory is synchronized from the personal portfolio by the scheduled GitHub Actions workflow.

The site is a static bilingual HTML/CSS/JavaScript application. GitHub Actions assembles the website and the RoutePilot and SignalDesk interactive demos for GitHub Pages. The contact form currently falls back to the visitor's email application until its secure backend is deployed and tested.

## Engineering portfolio
| Project | Summary | Source |
|---|---|---|
| **Agent Workflow Orchestrator** | Approval-aware DAG workflow engine with dependency scheduling, bounded retries, SQLite persistence and an append-only audit trail. | [Open](projects/agent-workflow-orchestrator/) |
| **Event Stream Processing Platform** | Event-ingestion reference implementation with schema validation, idempotent writes, dead-letter handling and windowed aggregation. | [Open](projects/event-stream-processing-platform/) |
| **Grounded Document Retrieval API** | Source-aware document retrieval baseline using TF-IDF, cosine similarity and a FastAPI interface. | [Open](projects/grounded-document-retrieval/) |
| **Intelligent Recommendation Platform** | Recommendation API with interaction feedback, cold-start fallback, seen-item suppression and explainable ranking. | [Open](projects/intelligent-recommendation-platform/) |
| **LLM Gateway Control Plane** | Provider-agnostic LLM gateway with routing policies, spend ceilings, bounded retries and a local mock mode. | [Open](projects/llm-gateway-control-plane/) |
| **Market Intelligence & Risk Analytics** | Educational OHLCV pipeline with validation, moving averages, daily-change monitoring and CSV reporting. | [Open](projects/market-intelligence-risk-engine/) |
| **ML Feature Store** | SQLite-backed feature store with typed schemas, versioned entity values, batch lookup and TTL freshness metadata. | [Open](projects/ml-feature-store/) |
| **ML Model Serving Platform** | Versioned scikit-learn model workflow with reproducible training, held-out evaluation and FastAPI inference. | [Open](projects/ml-model-serving-platform/) |
| **FarsiPulse** | Persian sentiment API with conservative text normalization, pretrained-model inference and batch processing. | [Open](projects/persian-sentiment-api/) |
| **AtlasRAG — Evidence Retrieval Platform** | Evidence-focused retrieval service using BM25 ranking, extractive evidence selection and retrieval evaluation; it does not claim LLM-generated answers. | [Open](projects/production-rag-service/) |
| **RoutePilot — Fleet & Delivery Operations** | Fleet and delivery MVP with FastAPI, SQLite, delivery tracking, proof-of-delivery metadata and simulated vehicle positions. | [Open](projects/routepilot/) |
| **SignalDesk — Service Operations Intelligence** | Service-desk MVP with ticket creation, assignment, SLA-risk filters, status changes and audit history. | [Open](projects/signaldesk/) |
| **STRIDE — Sportswear & Equipment Store** | Responsive sports retail storefront concept with product discovery, filters, wishlist, shopping bag and demo checkout. | [Open](projects/stride-store/) |
| **RelayForge — Reliable Webhook Delivery** | Webhook delivery core with idempotent ingestion, HMAC-SHA256 signatures, bounded retries and dead-letter handling. | [Open](projects/webhook-reliability-platform/) |
| **Workflow Orchestration Engine** | Dependency-aware DAG runner with cycle detection, topological execution, retries and per-step outcomes. | [Open](projects/workflow-orchestration-engine/) |
| **ERYNDEX Company Website** | Bilingual company website presenting ERYNDEX services, engineering portfolio, collaboration model and contact paths. | [Open](projects/eryndex-company-website/) |

## Repository structure
```text
.
├── .github/workflows/       # CI, evaluation and Pages deployment workflows
├── projects/                # Company website and engineering demonstrators
├── deploy/                  # Deployment and operations examples
├── docs/                    # Project review, setup and showcase documentation
├── compose.yaml             # Local multi-service demonstration stack
└── README.md
```

## Run selected services locally
```bash
docker compose up --build
```
Check each project's README for prerequisites, ports, environment variables, sample data and limitations. Do not expose demonstration services publicly without adding the security, authentication, persistence and operational controls required for the intended use.

## Engineering standards
- Prefer verifiable implementation details over marketing claims.
- Document assumptions, boundaries and known limitations.
- Keep setup reproducible and configuration explicit.
- Include tests and CI where appropriate to the project.
- Treat security, observability, maintainability and handover as part of engineering delivery.

## Contact
- Website: https://eryndex.net/
- Email: eryndexco@gmail.com
- GitHub: https://github.com/Eryndex
