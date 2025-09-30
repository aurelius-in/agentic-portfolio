# Agentic AI Systems Showcase

##### All software in this portfolio was designed and built by Oliver Ellison d/b/a Reliable AI Network, LLC ("RAIN").

A single place to explore production-grade agentic AI work. Each project includes a short summary, use cases, tech stack, and screenshots. Built to be skimmed by engineering leaders, execs, and recruiters.

Contact: **oliveraellison@gmail.com** • [LinkedIn](https://www.linkedin.com/in/oellison/)

---

> **Live Portfolio Grid:** https://aurelius-in.github.io/agentic-portfolio/  
> **Source of truth:** [docs/portfolio.json](docs/portfolio.json)

---

## Contents

* [Projects](#projects)
  * [Agentic AI Health Navigator](#agentic-ai-health-navigator)
  * [AutoOps Sentinel](#autoops-sentinel)
  * [Agentic Claims Triage AI](#agentic-claims-triage-ai)
  * [Enterprise Wellness AI (MindTrace)](#enterprise-wellness-ai-mindtrace)
  * [High-Volume Recruiter Agent (Hire Falcon)](#high-volume-recruiter-agent-hire-falcon)
  * [AI Governance Dashboard](#ai-governance-dashboard)
  * [AI Document Agent (aiDa)](#ai-document-agent-aida)
  * [MuseAgent](#museagent)
  * [AdOps Flightdeck](#adops-flightdeck)
  * [EdgeSight QA](#edgesight-qa)
  * [MyRiskAgent](#myriskagent)
  * [Perception Lab](#perception-lab)
  * [ACE Lab](#ace-lab)
* [Application Matrix](#application-matrix)
* [Demo Matrix](#demo-matrix)
* [Architecture One-Pagers](#architecture-one-pagers)
* [License](#license)

---

## Projects

### Agentic AI Health Navigator
**Repo:** https://github.com/aurelius-in/AI-Health-Navigator-for-Patients

**Summary**  
Healthcare navigation with intelligent triage, provider matching, and personalized recommendations using multi-agent reasoning with memory (episodic, semantic, long-term) and cross-agent collaboration.

**Use cases**
- Symptom intake to recommended care path
- Provider matching and appointment guidance
- Benefits and coverage checks with safety and compliance context

**Tech stack**
- **Backend:** FastAPI, PyTorch, PostgreSQL, Redis, ChromaDB
- **Frontend:** React, TypeScript
- **Infra:** Docker, Kubernetes, Prometheus, Grafana; HIPAA-aware controls

**Screenshots**
<p>
  <img src="https://raw.githubusercontent.com/aurelius-in/AI-Health-Navigator-for-Patients/main/assets/screen1.png" width="49%">
  <img src="https://raw.githubusercontent.com/aurelius-in/AI-Health-Navigator-for-Patients/main/assets/screen2.png" width="49%">
</p>
<p>
  <img src="https://raw.githubusercontent.com/aurelius-in/AI-Health-Navigator-for-Patients/main/assets/screen3.png" width="49%">
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
  <img src="https://raw.githubusercontent.com/aurelius-in/Claims-Triage-AI/main/docs/images/claims-demo.gif" width="49%">
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
  <img src="https://raw.githubusercontent.com/aurelius-in/MindTrace/main/assets/demo.gif" width="49%">
</p>

---

### High-Volume Recruiter Agent (Hire Falcon)
**Repo:** https://github.com/aurelius-in/high-volume-recruiter-ai-agent

**Summary**  
End-to-end recruiter flow (outreach → consent → screening → scheduling → ATS sync) with a live ops UI, real-time KPIs, and a signed, replayable audit trail. Runs offline for controlled demos or in real mode via adapters, with capacity/SLA analytics and policy-checked messaging.

**Use cases**
- High-volume roles (retail, logistics, CX): scale outreach, screening, scheduling
- Staffing and RPO teams: live ops console with agent assist and policy guardrails
- Compliance and audit: signed ledger and replay for verification and incident review

**Tech stack**
- **Backend:** Python 3.11, FastAPI, Uvicorn; SSE endpoints (`/events/stream`, `/chat/stream`); signed audit chain
- **Frontend:** React + Vite + Material UI, Recharts, i18n (EN, AR, ZH), dark mode; Ask panel with streaming
- **Infra/QA:** Docker; Postgres-ready seams; pytest; structured logs and PII redaction

**Screenshots**
<p>
  <img src="https://raw.githubusercontent.com/aurelius-in/high-volume-recruiter-ai-agent/main/hiretab1.gif" width="49%">
  <img src="https://raw.githubusercontent.com/aurelius-in/high-volume-recruiter-ai-agent/main/hiretab2.gif" width="49%">
</p>
<p>
  <img src="https://raw.githubusercontent.com/aurelius-in/high-volume-recruiter-ai-agent/main/hiretab3.gif" width="49%">
</p>

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
  <img src="https://raw.githubusercontent.com/aurelius-in/AI-Governance/main/assets/screen1.png" width="49%">
  <img src="https://raw.githubusercontent.com/aurelius-in/AI-Governance/main/assets/screen2.png" width="49%">
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

### MuseAgent
**Repo:** https://github.com/aurelius-in/MuseAgent

**Summary**  
A modular multi-agent music intelligence platform that ingests tracks, extracts spectral features, generates embeddings, tags mood, genre, and instrumentation, delivers explainable recommendations with visualizations, exports branded PDF reports, and includes optional enrichment and AI-powered music generation.

**Screenshots**
<p>
  <img src="https://raw.githubusercontent.com/aurelius-in/MuseAgent/main/assets/ma-ui.gif" width="60%">
</p>

---

### AdOps Flightdeck
**Repo:** https://github.com/aurelius-in/adops-flightdeck-multi-agent

**Summary**  
Production-grade multi-agent AdOps Flightdeck that orchestrates AI agents for planning, creative generation and safety, pacing, anomaly response, attribution, and auditable reporting on AWS.

**Screenshots**
<p>
  <img src="https://raw.githubusercontent.com/aurelius-in/adops-flightdeck-multi-agent/main/assets/adops-demo.gif" width="60%">
</p>

---

### EdgeSight QA
**Repo:** https://github.com/aurelius-in/EdgeSight-QA

**Summary**  
Modular, containerized edge computer-vision QA: multi-camera ingest to on-device inference to SCADA write-backs, with operator UI, metrics, and offline-safe logging.

**Screenshots**
<p>
  <img src="https://aurelius-in.github.io/agentic-portfolio/images/esqa-preview.gif?v=1" width="60%">
</p>

---

### MyRiskAgent
**Repo:** https://github.com/aurelius-in/MyRiskAgent

**Summary**  
Agentic risk analysis that ingests claims, filings, and OSINT to compute provider and company risk scores with peer-normalized outlier detection, SHAP explainability, and audit-ready evidence.

**Tech stack**  
FastAPI (Python 3.11), SQLModel/SQLAlchemy, DuckDB, Postgres/pgvector, Redis, React + TypeScript + Vite + MUI + TanStack Query + ECharts, OPA (Rego), Prometheus, Grafana, Docker Compose, Alembic; LangGraph-style orchestration.

**Screenshot**
<p>
  <img src="https://raw.githubusercontent.com/aurelius-in/reliable-ai-network/main/mra-placeholder.png" width="49%">
</p>

---

### Perception Lab
**Repo:** https://github.com/aurelius-in/perception-lab

**Summary**  
Interactive environment for exploring perception scenarios, running detection and fusion pipelines, monitoring performance metrics, and exporting evaluation reports.

**Screenshots**
<p>
  <img src="https://aurelius-in.github.io/agentic-portfolio/images/detect-ani-1.gif?v=2" width="60%">
</p>

---

### ACE Lab
**Repo:** https://github.com/aurelius-in/ACE-Lab

**Summary**  
Real-time WebGPU-first creative lab that blends agentic shader design, on-device image generation, and microservice video generation using AnimateDiff for motion and RIFE for interpolation, with generative fill, style transfer, and policy-safe WebM export via OPA in WASM.

**Screenshots**
<p>
  <img src="https://aurelius-in.github.io/agentic-portfolio/images/ace-lab.gif?v=1" width="60%">
</p>

---

## Application Matrix

| Project | Primary Domain | Core Agents | Signals and Models | Governance and Observability | Frontend |
|---|---|---|---|---|---|
| Health Navigator | Healthcare navigation | Planner, Triage, Memory, Provider-Match | LLM with retrieval, clinical triage heuristics | HIPAA awareness, RBAC, audit | React/TS |
| AutoOps Sentinel | AIOps | Detector, Forecaster, Remediator, Explainer | Z-score, IsolationForest, MAD, Prophet | Runbooks, RBAC, CI/CD, Slack and Teams | React/MUI |
| Claims Triage | Insurance and healthcare | Classifier, Risk, Router, Compliance, Support | XGBoost+SHAP, retrieval, OPA | Audit, PII redaction, policies-as-code | React/TS |
| MindTrace | Workforce wellness | Companion, Recommender, Risk, Analytics, Privacy | Sentiment and risk models, DP analytics | HIPAA, GDPR, SOC2, OPA | React/TS |
| High-Volume Recruiter | Recruiting ops | Outreach, Consent, Qualifier, Scheduler, ATS Sync | Policy checks, SSE streaming, multilingual i18n | Signed audit ledger, replay, SLA heatmaps | React/Vite/MUI |
| AI Governance | Governance platform | Proxy, Policy, Safety, Cost | Guardrails, OPA, usage telemetry | Cost and safety enforcement | React |
| aiDa | Document intelligence | Orchestrator plus task agents | NER, QA, compare, translate | Audit, OpenTelemetry | React/TS |
| MuseAgent | Music intelligence | Ingest, Feature Extractor, Embedder, Tagger, Generator | MFCC, mel, chroma, CLAP/OpenL3, RAG | Deterministic demo mode, Dockerized, eval reports | React/TS |
| AdOps Flightdeck | Advertising ops | Planner, Creative QA, Pacing, Anomaly, Attribution, Reporter | LangGraphJS, Bedrock models, anomaly detectors | AWS-native, OpenTelemetry, auditable reporting | React/TS |
| EdgeSight QA | Industrial CV | Ingest, Infer, QA, SCADA Writer, Monitor | ONNX/TensorRT, rules and thresholds | Offline logging, Prometheus, Grafana | React/Vite/MUI |
| MyRiskAgent | Risk and compliance | Ingest, Score, Explain, Policy Gate, Report | SHAP, peer normalization, OSINT retrieval | OPA, evidence bundles, immutable logs | React/TS |
| Perception Lab | Perception R&D | Detector, Fusion, Monitor, Evaluator | CV pipelines, COCO metrics, IDF1 | Audit-ready exports, Docker | React/TS |
| ACE Lab | Real-time creative | Shader, Generator, Video, Policy Gate | WebGPU/WGSL, AnimateDiff, RIFE | OPA to WASM, export safety | React/Vite |

---

## Demo Matrix

| Project | Quick Path To Show Value | Safe Mode Toggle | Wow Moment |
|---|---|---|---|
| Health Navigator | Run symptom intake flow with 2 scenarios and show provider matching | Disable external calls, use seeded retrieval | Cross-agent memory recalls prior visit to refine plan |
| AutoOps Sentinel | Replay a known incident, show forecast, trigger guarded remediation | Read-only mode for actions | Exec narrative quantifies cost avoided and MTTR delta |
| Claims Triage | Upload a sample claim set, view routing rationale and policy checks | Offline retrieval bundle only | SHAP plot explains why two claims diverged |
| MindTrace | Simulate anonymized weekly rollup with risk hotspots | Redacted PII and DP thresholds | Drilldown preserves privacy constraints while guiding action |
| High-Volume Recruiter | Start outreach batch, watch SSE stream, schedule 2 interviews | Offline adapter with signed logs | Replay a candidate’s full interaction from the audit ledger |
| AI Governance | Route prompts across two models with different policies | Sandbox policies file | Flip a policy switch and watch cost and safety metrics shift |
| aiDa | Ingest a policy PDF and run risk questions | Local chunked retrieval only | Export an evidence bundle for audit in one click |
| MuseAgent | Ingest 3 tracks, view features and similarity, export PDF | Deterministic seeds | Tag-aware playlist fit score surprises a skeptic |
| AdOps Flightdeck | Run a creative safety check and pacing adjustment | Dry-run events only | Attribution agent explains anomaly with tracebacks |
| EdgeSight QA | Play recorded line feed, see detections and SCADA writes | Offline queue only | Operator correction improves next-frame decision |
| MyRiskAgent | Score 5 providers, open SHAP explanations | OSINT disabled, use cached | Evidence bundle compiles in seconds for review |
| Perception Lab | Run two detectors on a clip, compare metrics | Local models only | Side-by-side mAP and IDF1 compare drives model choice |
| ACE Lab | Live shader edit with video gen export | Policy level: Safe | WebGPU render updates in real time while exporting compliant WebM |

---

## Architecture One-Pagers

Each project has or targets a skimmable one-pager in `docs/`:

- Problem and business value  
- Agent architecture and orchestration  
- Data flow and storage  
- Safety, privacy, and governance  
- Deployability and ops notes  
- Demo script and wow moments

File naming: `docs/<project-id>-onepager.md`  
Examples: `docs/health-navigator-onepager.md`, `docs/autoops-sentinel-onepager.md`, `docs/myriskagent-onepager.md`

---

## License
MIT
