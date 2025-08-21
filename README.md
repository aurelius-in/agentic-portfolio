# Agentic AI Systems Showcase

A single place to explore my production-grade, agentic AI work. Each project includes a short summary, use cases, tech stack, architecture notes, and screenshots. Perfect for quick evaluation by engineering leaders, execs, and recruiters.

> Contact: oliver@reliaable.ai • LinkedIn: linkedin.com/in/oliveraellison

---

## Contents
- [Projects](#projects)
  - [Agentic AI Health Navigator](#agentic-ai-health-navigator)
  - [AutoOps Sentinel](#autoops-sentinel)
  - [Agentic Claims Triage AI](#agentic-claims-triage-ai)
  - [Enterprise Wellness AI (MindTrace)](#enterprise-wellness-ai-mindtrace)
  - [AI Governance Dashboard](#ai-governance-dashboard)
  - [AI Document Agent (aiDa)](#ai-document-agent-aida)
- [Architecture One-Pagers](#architecture-one-pagers)
- [Demo Matrix](#demo-matrix)
- [How to Use This Portfolio](#how-to-use-this-portfolio)
- [License](#license)

---

## Projects

### Agentic AI Health Navigator
**Repo:** https://github.com/aurelius-in/AI-Health-Navigator-for-Patients

**Summary**  
Next-gen healthcare navigation with intelligent triage, provider matching, and personalized recommendations. Multi-agent reasoning with memory (episodic, semantic, long-term) and cross-agent collaboration for advanced decision support. :contentReference[oaicite:0]{index=0} :contentReference[oaicite:1]{index=1}

**Use cases**
- Symptom intake to recommended care path
- Provider matching and appointment guidance
- Benefit/coverage checks with safety/compliance context

**Tech stack**
- **Backend:** FastAPI, PyTorch, PostgreSQL, Redis, ChromaDB
- **Frontend:** React, TypeScript
- **Infra/ops:** Docker, Kubernetes, Prometheus, Grafana; HIPAA-aware controls :contentReference[oaicite:2]{index=2}

**Screenshots**  
> I’ll keep lightweight thumbnails here and full-size images in `assets/`.  
<p>
  <a href="https://github.com/aurelius-in/AI-Health-Navigator-for-Patients">
    <img src="https://opengraph.githubassets.com/1/aurelius-in/AI-Health-Navigator-for-Patients" width="49%">
  </a>
</p>

---

### AutoOps Sentinel
**Repo:** https://github.com/aurelius-in/AutoOps-Sentinel

**Summary**  
Agentic AIOps that ingests metrics/logs, detects anomalies, predicts incidents, and executes safe auto-remediation with a modern React dashboard. The built-in Agent explains actions, answers questions, and quantifies cost avoided. :contentReference[oaicite:3]{index=3}

**Use cases**
- Proactive incident prevention and SLO burn detection
- Automated runbooks with policy guardrails
- Exec-ready narratives and value attribution

**Tech stack**
- **Backend:** FastAPI, Python
- **Frontend:** React, TypeScript (MUI)
- **ML:** Z-score, IsolationForest, MAD, Prophet forecasting
- **Ops:** Docker Compose, GitHub Actions CI/CD, RBAC, Slack/Teams integration :contentReference[oaicite:4]{index=4}

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
Agent-driven decision support for claims classification, risk scoring, routing, and compliance with explainable AI and human-in-the-loop oversight. React dashboards deliver analytics, audit trails, and visual model explanations. :contentReference[oaicite:5]{index=5} :contentReference[oaicite:6]{index=6}

**Use cases**
- Insurance claims intake and triage
- Healthcare prior auth and medical necessity review
- Finance/legal case routing with policy-as-code

**Tech stack**
- **Backend:** FastAPI, PostgreSQL, Redis, Docker
- **AI/ML:** LLM+ML hybrid, SHAP explainability, RAG; OPA for policies
- **Frontend:** React, TypeScript; Prometheus/Grafana observability :contentReference[oaicite:7]{index=7}

**Screenshots**
<p>
  <a href="https://github.com/aurelius-in/Claims-Triage-AI">
    <img src="https://opengraph.githubassets.com/1/aurelius-in/Claims-Triage-AI" width="49%">
  </a>
</p>

---

### Enterprise Wellness AI (MindTrace)
**Repo:** https://github.com/aurelius-in/MindTrace

**Summary**  
Enterprise wellness platform with five agents (Companion, Recommendation, Risk Detection, Analytics, Privacy) for organizational health, burnout detection, and resilience with privacy-first design. :contentReference[oaicite:8]{index=8} :contentReference[oaicite:9]{index=9}

**Use cases**
- Employee wellness companion and mood journaling
- HR analytics on anonymized, privacy-safe signals
- Burnout risk prediction and intervention guidance

**Tech stack**
- **Backend:** FastAPI, PostgreSQL, Redis, ChromaDB/Pinecone
- **Frontend:** React, TypeScript
- **Integrations:** Slack/Teams, HRIS, Outlook
- **Ops:** Kubernetes/Helm, Prometheus/Grafana, OPA; differential privacy :contentReference[oaicite:10]{index=10}

**Screenshots**
<p>
  <a href="https://github.com/aurelius-in/MindTrace">
    <img src="https://opengraph.githubassets.com/1/aurelius-in/MindTrace" width="49%">
  </a>
</p>

---

### AI Governance Dashboard
**Repo:** https://github.com/aurelius-in/AI-Governance

**Summary**  
Enterprise AI governance with an LLM proxy, policies-as-code, safety guardrails, automated compliance checks, and real-time cost monitoring. Built with production-grade MLOps and full observability. :contentReference[oaicite:11]{index=11} :contentReference[oaicite:12]{index=12}

**Use cases**
- Policy enforcement and redaction on LLM traffic
- Cost controls and vendor routing
- Trust, safety, and auditability for AI systems

**Tech stack**
- **Backend:** FastAPI, PostgreSQL, Redis
- **Governance:** OPA, guardrails; compliance checks
- **Ops:** Docker/Kubernetes, Prometheus/Grafana; React frontend :contentReference[oaicite:13]{index=13}

**Screenshots**
<p>
  <a href="https://github.com/aurelius-in/AI-Governance">
    <img src="https://opengraph.githubassets.com/1/aurelius-in/AI-Governance" width="49%">
  </a>
</p>

---

### AI Document Agent (aiDa)
**Repo:** https://github.com/aurelius-in/Smart-Document-Bot

**Summary**  
Multi-agent document analysis for regulatory compliance and business intelligence. Ingest, classify, extract entities, assess risk, and monitor compliance with audit trails and live agent traces. :contentReference[oaicite:14]{index=14} :contentReference[oaicite:15]{index=15}

**Use cases**
- Regulatory doc intake and QA
- Risk flagging and policy checks
- Interactive analytics and evidence export

**Tech stack**
- **Backend:** FastAPI, PostgreSQL, vector search
- **Frontend:** React, TypeScript
- **Observability:** OpenTelemetry; containerized deployment :contentReference[oaicite:16]{index=16}

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

Each project in `docs/` has a short, skimmable one-pager:
- Problem & business value
- Agent architecture & orchestration
- Data flow & storage
- Safety, privacy, and governance
- Deployability and ops notes
- Demo script & wow moments

See: [`docs/`](docs/)

---

## Demo Matrix

| Project | Core Agents | Key Models/Methods | Ops & Compliance | Frontend |
|---|---|---|---|---|
| Health Navigator | Planner, Triage, Memory, Provider-Match | LLM+retrieval, clinical triage heuristics | HIPAA awareness, RBAC, audit | React/TS |
| AutoOps Sentinel | Detector, Forecaster, Remediator, Explainer | Z-score, IsolationForest, MAD, Prophet | Runbooks, RBAC, CI/CD, Slack/Teams | React/MUI |
| Claims Triage | Classifier, Risk, Router, Compliance, Support | XGBoost+SHAP, RAG, OPA | Audit, PII redaction, policies-as-code | React/TS |
| MindTrace | Companion, Recommender, Risk, Analytics, Privacy | Sentiment+risk models, DP analytics | HIPAA/GDPR/SOC2, OPA | React/TS |
| AI Governance | Proxy, Policy, Safety, Cost | Guardrails, OPA, usage telemetry | Cost & safety enforcement | React |
| aiDa | Orchestrator + 8 task agents | NER, QA, compare, translate | Audit, OpenTelemetry | React/TS |

---

## How to Use This Portfolio

### Local
```bash
git clone https://github.com/aurelius-in/agentic-portfolio
cd agentic-portfolio
