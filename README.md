# Agentic AI Systems Showcase

A single place to explore my production-grade agentic AI work. Each project includes a short summary, use cases, tech stack, and screenshots. Built to be skimmed by engineering leaders, execs, and recruiters.

Contact: oliveraellison@gmail.com • LinkedIn: https://www.linkedin.com/in/oellison/

---
> **Live Portfolio Grid:** https://aurelius-in.github.io/agentic-portfolio/  
> **Source of truth:** [docs/portfolio.json](docs/portfolio.json)
---

## Contents
- [Projects](#projects)
  - [Agentic AI Health Navigator](#agentic-ai-health-navigator)
  - [AutoOps Sentinel](#autoops-sentinel)
  - [Agentic Claims Triage AI](#agentic-claims-triage-ai)
  - [Enterprise Wellness AI (MindTrace)](#enterprise-wellness-ai-mindtrace)
  - [High-Volume Recruiter Agent (Hire Falcon)](#high-volume-recruiter-agent)

  - [AI Governance Dashboard](#ai-governance-dashboard)
  - [AI Document Agent (aiDa)](#ai-document-agent-aida)
- [Architecture One-Pagers](#architecture-one-pagers)
- [Demo Matrix](#demo-matrix)
- [License](#license)

---

## Projects

### Agentic AI Health Navigator
**Repo:** https://github.com/aurelius-in/AI-Health-Navigator-for-Patients

**Summary**  
Healthcare navigation with intelligent triage, provider matching, and personalized recommendations using multi-agent reasoning with memory (episodic, semantic, long-term) and cross-agent collaboration.

**Use cases**
- Symptom intake to recommended care path
- Provider matching and appointment guidance
- Benefit and coverage checks with safety and compliance context

**Tech stack**
- **Backend:** FastAPI, PyTorch, PostgreSQL, Redis, ChromaDB
- **Frontend:** React, TypeScript
- **Infra:** Docker, Kubernetes, Prometheus, Grafana; HIPAA-aware controls

**Screenshots**
<p>
  <img src="https://github.com/aurelius-in/AI-Health-Navigator-for-Patients/blob/main/assets/screen1.png" width="49%">
  <img src="https://github.com/aurelius-in/AI-Health-Navigator-for-Patients/raw/main/assets/screen2.png" width="49%">
</p>
<p>
  <img src="https://github.com/aurelius-in/AI-Health-Navigator-for-Patients/raw/main/assets/screen3.png" width="49%">
</p>

---

### AutoOps Sentinel
**Repo:** https://github.com/aurelius-in/AutoOps-Sentinel

**Summary**  
Agentic AIOps that ingests metrics and logs, detects anomalies, forecasts incidents, and executes safe auto-remediation with a modern React dashboard. Explains actions, answers questions, and quantifies cost avoided.

**Use cases**
- Proactive incident prevention and SLO burn detection
- Automated runbooks with policy guardrails
- Exec-ready narratives and value attribution

**Tech stack**
- **Backend:** FastAPI, Python
- **Frontend:** React, TypeScript (MUI)
- **ML:** Z-score, IsolationForest, MAD, Prophet
- **Ops:** Docker, GitHub Actions CI/CD, RBAC, Slack and Teams integration

**Screenshots**
<p>
  <img src="https://raw.githubusercontent.com/aurelius-in/AutoOps-Sentinel/main/aostab1.gif" width="49%">
  <img src="https://raw.githubusercontent.com/aurelius-in/AutoOps-Sentinel/main/aostab2.gif" width="49%">
</p>
<p>
  <img src="https://raw.githubusercontent.com/aurelius-in/AutoOps-Sentinel/main/aostab3.gif" width="49%">
</p>

---

### Agentic Claims Triage AI
**Repo:** https://github.com/aurelius-in/Claims-Triage-AI

**Summary**  
Agent-driven decision support for claims classification, risk scoring, routing, and compliance with explainable AI and human-in-the-loop oversight. React dashboards deliver analytics, audit trails, and visual model explanations.

**Use cases**
- Insurance claims intake and triage
- Healthcare prior authorization and medical necessity review
- Finance and legal case routing with policy-as-code

**Tech stack**
- **Backend:** FastAPI, PostgreSQL, Redis, Docker
- **AI/ML:** LLM and ML hybrid, SHAP explainability, retrieval, OPA for policies
- **Frontend:** React, TypeScript; Prometheus and Grafana observability

**Screenshots**
<p>
  <img src="https://github.com/aurelius-in/Claims-Triage-AI/raw/main/docs/images/claims-demo.gif" width="49%">
</p>

---

### Enterprise Wellness AI (MindTrace)
**Repo:** https://github.com/aurelius-in/MindTrace

**Summary**  
Enterprise wellness platform with five agents (Companion, Recommendation, Risk Detection, Analytics, Privacy) for organizational health, burnout detection, and resilience with a privacy-first design.

**Use cases**
- Employee wellness companion and mood journaling
- HR analytics on anonymized, privacy-safe signals
- Burnout risk prediction and intervention guidance

**Tech stack**
- **Backend:** FastAPI, PostgreSQL, Redis, ChromaDB or Pinecone
- **Frontend:** React, TypeScript
- **Integrations:** Slack, Teams, HRIS, Outlook
- **Ops:** Kubernetes and Helm, Prometheus and Grafana, OPA; differential privacy

**Screenshots**
<p>
  <img src="https://github.com/aurelius-in/MindTrace/raw/main/assets/demo.gif" width="49%">
</p>

---

### High-Volume Recruiter Agent

Repo: https://github.com/aurelius-in/high-volume-recruiter-ai-agent

Summary  
End-to-end recruiter flow (outreach → consent → screening → scheduling → ATS sync) with a live ops UI, real-time KPIs, and a signed, replayable audit trail. Runs offline for demos or in “real” mode via adapters, with capacity/SLA analytics and policy-checked messaging.

Use cases
- High-volume roles (retail, logistics, CX): scale outreach/screening/scheduling.
- Staffing & RPO teams: live ops console with agent assist and policy guardrails.
- Compliance & audit: signed ledger + replay for verification and incident review.

Tech stack
- Backend: Python 3.11, FastAPI, Uvicorn; SSE endpoints (`/events/stream`, `/chat/stream`); signed audit chain.
- Frontend: React + Vite + Material UI, Recharts, i18n (EN/AR/ZH), dark mode; “Ask” panel with streaming.
- Infra/QA: Docker + Render blueprint; Postgres-ready seams; pytest; structured logs + demo PII redaction.

Screenshots

![Tab 1](https://github.com/aurelius-in/high-volume-recruiter-ai-agent/raw/main/hiretab1.gif)
![Tab 2](https://github.com/aurelius-in/high-volume-recruiter-ai-agent/raw/main/hiretab2.gif)
![Tab 3](https://github.com/aurelius-in/high-volume-recruiter-ai-agent/raw/main/hiretab3.gif)

---

### AI Governance Dashboard
**Repo:** https://github.com/aurelius-in/AI-Governance

**Summary**  
Enterprise AI governance with an LLM proxy, policies-as-code, safety guardrails, automated compliance checks, and real-time cost monitoring. Built with production-grade MLOps and full observability.

**Use cases**
- Policy enforcement and redaction on LLM traffic
- Cost controls and vendor routing
- Trust, safety, and auditability for AI systems

**Tech stack**
- **Backend:** FastAPI, PostgreSQL, Redis
- **Governance:** OPA, guardrails, automated checks
- **Ops:** Docker and Kubernetes, Prometheus and Grafana; React frontend

**Screenshots**
<p>
  <img src="https://github.com/aurelius-in/AI-Governance/raw/main/assets/screen1.png" width="49%">
  <img src="https://github.com/aurelius-in/AI-Governance/raw/main/assets/screen2.png" width="49%">
</p>

---

### AI Document Agent (aiDa)
**Repo:** https://github.com/aurelius-in/Smart-Document-Bot

**Summary**  
Multi-agent document analysis for regulatory compliance and business intelligence. Ingest, classify, extract entities, assess risk, and monitor compliance with audit trails and live agent traces.

**Use cases**
- Regulatory document intake and QA
- Risk flagging and policy checks
- Interactive analytics and evidence export

**Tech stack**
- **Backend:** FastAPI, PostgreSQL, vector search
- **Frontend:** React, TypeScript
- **Observability:** OpenTelemetry; containerized deployment

**Screenshots**
<p>
  <img src="https://raw.githubusercontent.com/aurelius-in/Smart-Document-Bot/main/tab1.gif" width="49%">
  <img src="https://raw.githubusercontent.com/aurelius-in/Smart-Document-Bot/main/tab2.gif" width="49%">
</p>
<p>
  <img src="https://raw.githubusercontent.com/aurelius-in/Smart-Document-Bot/main/tab3.gif" width="49%">
  <img src="https://raw.githubusercontent.com/aurelius-in/Smart-Document-Bot/main/tab4.gif" width="49%">
</p>

---

## Architecture One-Pagers

Each project has a short, skimmable one-pager in `docs/`:
- Problem and business value
- Agent architecture and orchestration
- Data flow and storage
- Safety, privacy, and governance
- Deployability and ops notes
- Demo script and wow moments

---

## Demo Matrix

| Project | Core Agents | Key Models and Methods | Ops and Compliance | Frontend |
|---|---|---|---|---|
| Health Navigator | Planner, Triage, Memory, Provider-Match | LLM with retrieval, clinical triage heuristics | HIPAA awareness, RBAC, audit | React/TS |
| AutoOps Sentinel | Detector, Forecaster, Remediator, Explainer | Z-score, IsolationForest, MAD, Prophet | Runbooks, RBAC, CI/CD, Slack and Teams | React/MUI |
| Claims Triage | Classifier, Risk, Router, Compliance, Support | XGBoost+SHAP, retrieval, OPA | Audit, PII redaction, policies-as-code | React/TS |
| MindTrace | Companion, Recommender, Risk, Analytics, Privacy | Sentiment and risk models, DP analytics | HIPAA, GDPR, SOC2, OPA | React/TS |
| AI Governance | Proxy, Policy, Safety, Cost | Guardrails, OPA, usage telemetry | Cost and safety enforcement | React |
| aiDa | Orchestrator plus task agents | NER, QA, compare, translate | Audit, OpenTelemetry | React/TS |

---

## License
MIT
