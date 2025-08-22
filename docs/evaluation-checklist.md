## Evaluation Checklist
#### A concise checklist for reviewers (engineering leaders, execs, recruiters) to assess the portfolio quickly.
**Problem & Outcome**
⦁	[ ] Problem statement and target users are clear
⦁	[ ] Business outcome(s) are stated (cost, risk, experience) and measurable
**Architecture & Agents**
⦁	[ ] Agent roles and orchestration are understandable at a glance
⦁	[ ] Data flow and storage choices are justified
⦁	[ ] External integrations/tools are listed (and bounded)
**Safety, Privacy, Governance**
⦁	[ ] Privacy considerations and redaction are explicit
⦁	[ ] Policies-as-code (OPA) and guardrails are present
⦁	[ ] Auditability and explainability are demonstrated
**Operations & Deployability**
⦁	[ ] Packaging (Docker), environment separation, and Helm/k8s readiness
⦁	[ ] Observability (OTEL/Prometheus/Grafana) summarized
⦁	[ ] CI/CD steps and basic tests described
**Demo Readiness**
⦁	[ ] Representative walkthrough is provided
⦁	[ ] Screens/animations match the walkthrough
⦁	[ ] Exportable artifacts (PDF/JSON) called out
**Code Quality Proxies**
⦁	[ ] Clear repo structure and README in each project
⦁	[ ] Config/secret handling is documented (no secrets committed)
⦁	[ ] Lint/test/format steps exist (or are sketched)
**Security & Access**
⦁	[ ] RBAC and scoped credentials are addressed
⦁	[ ] Vendor access and data egress are controlled
⦁	[ ] PII/PHI handling is explicit (if applicable)
