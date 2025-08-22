# Agentic AI Health Navigator — Architecture One-Pager

**Repo:** https://github.com/aurelius-in/AI-Health-Navigator-for-Patients  
**Contact:** oliveraellison@gmail.com • LinkedIn: https://www.linkedin.com/in/oellison/

A next-gen healthcare navigation platform that performs intelligent triage, provider matching, and personalized care recommendations using a multi-agent system with memory (episodic, semantic, long-term). Built to be demonstrably safe, explainable, and production-ready.

---

## 1) Problem & Business Value

**Problem.** Patients struggle to translate symptoms and benefits into the right next medical step, causing delays, ER overuse, and low satisfaction.

**Value.**
- Route to the right care the first time (lower avoidable cost, shorter time-to-care)
- Improve patient experience with clear “why” explanations and options
- Reduce clinician/agent load via self-service navigation and summary handoffs
- Enterprise-grade controls (auditability, privacy by design, observability)

---

## 2) Agent Architecture & Orchestration

**Agent roles (high level).**

| Agent | Purpose | Key Inputs | Key Outputs |
|---|---|---|---|
| **Intake** | Normalize symptoms & context | Free-text, forms, history | Structured case (ICD-like hints, risk flags) |
| **Triage** | Severity & urgency scoring | Intake case, clinical heuristics | Disposition (Urgent Care vs PCP vs ER) + confidence |
| **Evidence Retriever** | Grounded knowledge & benefits | KB, payer docs, provider directory | Citations, benefits, copays, constraints |
| **Planner** | Compose next-best actions | Triage + Evidence | Stepwise plan with alternatives |
| **Provider Matcher** | Find in-network providers | Directory, geo, availability | Ranked providers with fit rationale |
| **Benefit Verifier** | Coverage & pre-auth hints | Payer policy, member plan | Coverage summary, limits, pre-auth note |
| **Explainer** | Human-readable “why” | Full trace | Rationale, caveats, links |
| **Privacy/Consent** | PHI controls & redaction | Policy, consent | Enforced scopes, redacted payloads |
| **Orchestrator** | Tool & agent routing | All of the above | Deterministic agent graph execution |

**Orchestration (Mermaid).**
```mermaid
flowchart LR
U[User] -->|symptoms + profile| INT[Intake]
INT --> TRI[Triage]
TRI -->|disposition| PLN[Planner]
PLN --> RET[Evidence Retriever]
RET --> PLN
PLN --> PRV[Provider Matcher]
PLN --> BEN[Benefit Verifier]
PLN --> EXP[Explainer]
subgraph Controls
PRV -.->|policy check| PVC[Privacy/Consent]
RET -.-> PVC
EXP -.-> PVC
end
EXP --> UI[Care Plan + Why + Options]
UI --> AUD[Audit Log]
