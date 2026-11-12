# Project Scorecard and Portfolio Register

> Programme planning document. This is the approved candidate portfolio, not a release announcement. Every project still requires individual approval before implementation. Scores are preliminary prioritization judgments, not benchmark results or externally measured ratings; reassess as evidence changes.

## Scoring model

| Criterion | Weight |
|---|---:|
| Operational value | 25 |
| Technical depth | 20 |
| AI-agent suitability | 20 |
| Target-role relevance | 15 |
| Portfolio and demonstration value | 10 |
| Feasibility within a 48–72-hour build cycle | 10 |
| **Total** | **100** |

A high score does not establish novelty, safety or production readiness.

## Kubernetes candidate portfolio

| ID | Candidate | Score | Priority |
|---|---|---:|---|
| K01 | Cluster Intelligence Agent | 96 | P0 |
| K02 | Troubleshooting Agent | 98 | P0 |
| K03 | Security Auditor Agent | 97 | P0 |
| K04 | Deployment Intelligence Agent | 96 | P0 |
| K05 | Observability Investigation Agent | 97 | P0 |
| K06 | Resource Optimization Agent | 94 | P1 |
| K07 | Cost Intelligence Agent | 95 | P1 |
| K08 | Network Troubleshooting Agent | 93 | P1 |
| K09 | Autoscaling Advisor Agent | 94 | P1 |
| K10 | Configuration Drift Agent | 93 | P1 |
| K11 | Backup & Recovery Agent | 92 | P1 |
| K12 | Incident Response Agent | 97 | P1 |
| K13 | Manifest & Helm Review Agent | 92 | P2 |
| K14 | SRE Runbook Agent | 94 | P2 |
| K15 | Multi-Agent Kubernetes Operations Platform | 99 | P2 |

## Candidate briefs and alternatives to evaluate

### K01 — Cluster Intelligence Agent
Discover authorized EKS clusters and Kubernetes resources such as nodes, namespaces, pods, deployments, services and events. Produce a structured inventory and health report with evidence and timestamps.

Evaluate Kubernetes API/kubectl, AWS EKS APIs and console, Kubernetes dashboards and EKS MCP Server. Differentiation must come from cross-resource context, evidence provenance, operator-oriented summaries and repeatable evaluation—not merely wrapping list operations.

### K02 — Troubleshooting Agent
Investigate CrashLoopBackOff, ImagePullBackOff, Pending pods and failed probes. Correlate resource state, events, logs and telemetry; produce evidence-based hypotheses and next diagnostic steps.

Evaluate K8sGPT, kubectl, Kubernetes events/logs, Prometheus, Loki, CloudWatch and Robusta. K8sGPT already offers analyzers and LLM-assisted Kubernetes analysis, including Bedrock integration and MCP capabilities. Demonstrate a specific advantage or integrate it rather than reproduce it.

### K03 — Security Auditor Agent
Assess RBAC, service accounts, privileged containers, security contexts and network policy. Present prioritized findings, evidence and remediation guidance.

Integrate/compare Trivy, Kubescape, kube-bench, Kyverno, OPA Gatekeeper and Falco. Do not recreate scanners without a compelling reason.

### K04 — Deployment Intelligence Agent
Investigate failed CI/CD runs, rollout failures and GitOps synchronization issues. Correlate repository changes, workflow evidence, Argo CD state and cluster events.

Evaluate GitHub Actions, Argo CD, ECR, Kubernetes rollout status and CI/CD observability. Focus on cross-system diagnosis and traceable evidence.

### K05 — Observability Investigation Agent
Investigate alerts by querying approved metrics, dashboards and logs; correlate signals into a timeline and explain likely impact.

Evaluate Prometheus, Grafana, Loki, CloudWatch and OpenTelemetry. Complement observability platforms rather than replace telemetry or alerting.

### K06 — Resource Optimization Agent
Analyze CPU/memory requests and limits, utilization and pressure. Provide rightsizing recommendations with evidence and risk caveats.

Evaluate VPA, Goldilocks, Metrics Server, Prometheus and Kubecost. Distinguish observed utilization from safe workload capacity.

### K07 — Cost Intelligence Agent
Analyze AWS billing and EKS-related infrastructure costs, with namespace/workload attribution where defensible. Identify idle resources and optimization opportunities.

Evaluate OpenCost, Kubecost, AWS Cost Explorer, AWS Compute Optimizer and Karpenter. Distinguish actual billed costs from allocation estimates and forecasts.

### K08 — Network Troubleshooting Agent
Investigate DNS, service discovery, endpoints, connectivity and NetworkPolicy-related failures, including AWS VPC CNI context.

Evaluate CoreDNS, Cilium, Calico, Hubble, AWS VPC CNI and Kubernetes network diagnostics. Require safe, scoped probes and evidence.

### K09 — Autoscaling Advisor Agent
Analyze HPA/VPA configuration, pending workloads, node provisioning and scaling bottlenecks; recommend evidence-backed changes.

Evaluate HPA, VPA, Karpenter, Cluster Autoscaler and KEDA. Focus on diagnosis/advice rather than duplicating controllers.

### K10 — Configuration Drift Agent
Compare declared Git/IaC configuration with live cluster state, identify drift and explain impact. Remediation requires review and approval.

Evaluate Argo CD, Flux, Terraform plan and AWS Config. Add contextual explanation and traceability.

### K11 — Backup & Recovery Agent
Verify backup schedules and job results, inventory recovery points and help validate restore procedures for supported workloads and persistent volumes.

Evaluate Velero, Kasten, AWS Backup and EBS snapshots. Backup-job success is not proof of recoverability; restore testing is required.

### K12 — Incident Response Agent
Collect authorized diagnostic context after an alert, recommend severity, create an incident timeline and prepare a recovery plan and post-incident report.

Evaluate PagerDuty, Rootly, Robusta, Grafana OnCall and incident workflows. Human operators retain control of remediation.

### K13 — Manifest & Helm Review Agent
Review Kubernetes manifests and Helm values for security, reliability, resource and policy concerns. Offer traceable suggestions, ideally as GitHub pull-request feedback.

Evaluate KubeLinter, kube-score, Polaris, Checkov, Datree and Trivy. Integrate scanners and explain findings rather than replace them.

### K14 — SRE Runbook Agent
Retrieve context-relevant runbooks and guide approved diagnostic steps. Record evidence/actions and prepare an incident summary.

Evaluate Backstage, Rundeck, StackStorm, AWS Systems Manager Automation and incident runbook tooling. Execution must be allowlisted, authorized and audited.

### K15 — Multi-Agent Kubernetes Operations Platform
Coordinate specialized agents through a shared interface with scoped authorization, explicit human approval, audit history and consistent evaluation.

This is a capstone integration effort, not the starting point. Reuse validated agents and shared interfaces rather than bundling unproven agents.

## Portfolio governance
- This list is not a promise every candidate will be built exactly as described.
- Refresh alternatives research and confirm the operational gap before each project.
- Re-score when evidence materially changes feasibility or differentiation.
- Add projects to the root README only after release criteria are met.
- Record scope changes and decisions in project documentation and ADRs.
