## Evaluation Checklist
*A concise checklist for reviewers (engineering leaders, executives, recruiters) to assess the portfolio quickly.*

### Problem & Outcome
- ✅ Problem statement and target users are clear
- ✅ Business outcomes (cost, risk, experience) are stated and measurable

### Architecture & Agents
- ✅ Agent roles and orchestration are understandable at a glance
- ✅ Data flow and storage choices are justified
- ✅ External integrations and tools are listed and scoped

### Safety, Privacy & Governance
- ✅ Privacy considerations and redaction are explicit
- ✅ Policies-as-code (OPA) and guardrails are present
- ✅ Auditability and explainability are demonstrated

### Operations & Deployability
- ✅ Packaging (Docker), environment separation, and Helm/Kubernetes readiness
- ✅ Observability (OpenTelemetry, Prometheus, Grafana) summarized
- ✅ CI/CD steps and basic tests described

### Walkthrough Readiness
- ✅ Representative walkthrough is provided
- ✅ UI previews (GIF/PNG) align with the walkthrough
- ✅ Exportable artifacts (PDF/JSON) are referenced

### Code Quality Proxies
- ✅ Clear repo structure and README in each project
- ✅ Config and secret handling documented (no secrets committed)
- ✅ Lint, test, and format steps exist (or are outlined)

### Security & Access
- ✅ RBAC and scoped credentials addressed
- ✅ Vendor access and data egress controlled
- ✅ PII/PHI handling explicit (if applicable)
