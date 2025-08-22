# AutoOps Sentinel — Architecture One-Pager

**Repo:** https://github.com/aurelius-in/AutoOps-Sentinel  
**Contact:** oliveraellison@gmail.com • LinkedIn: https://www.linkedin.com/in/oellison/

Agentic AIOps that ingests metrics and logs, detects anomalies, forecasts incident risk, and executes safe auto-remediation via policy-driven runbooks. Includes exec-ready narratives that explain actions and quantify cost avoided.

---

## 1) Problem & Business Value

**Problem.** Ops teams drown in noisy alerts and manual runbooks, reacting late to incidents and SLO burn.

**Value.**
- Fewer pages and faster MTTR through proactive detection and guided auto-remediation
- Predictive visibility into risk and SLO burn to prevent outages
- Clear business translation of technical events into cost avoided and impact on availability
- Strong guardrails so automation is safe, auditable, and reversible

---

## 2) Agent Architecture & Orchestration

**Agent roles.**

| Agent | Purpose | Key Inputs | Key Outputs |
|---|---|---|---|
| **Detector** | Spot anomalies and regressions | Metrics, logs, baselines | Anomaly events with score and context |
| **Forecaster** | Predict incident risk and SLO burn | Recent metrics, seasonality | Risk horizon, burn estimate, confidence |
| **Planner** | Choose best remediation path | Events, policies, runbook catalog | Candidate plan with steps and prechecks |
| **Remediator** | Execute safe actions with guardrails | Plan, RBAC, approvals | Action results, rollback tokens |
| **Explainer** | Exec-friendly narrative and cost math | Events, actions, SLOs, rate cards | Storyboard: what happened, why, value |
| **Policy** | OPA policy checks and constraints | Runbook metadata, env rules | Allowed actions, blocked steps, justifications |
| **Orchestrator** | Route between agents and tools | All of the above | Deterministic graph execution and audit IDs |

**Orchestration (Mermaid).**
```mermaid
flowchart LR
SRC[Metrics & Logs] --> DET[Detector]
DET --> FRC[Forecaster]
DET --> PLN[Planner]
FRC --> PLN
PLN --> POL[Policy Checks]
POL -->|allow| REM[Remediator]
POL -->|deny| EXP[Explainer]
REM --> EXP
DET --> EXP
FRC --> EXP

```mermaid


EXP --> UI[Dashboard + Narrative + Cost Avoided]
UI --> AUD[Audit Log]
