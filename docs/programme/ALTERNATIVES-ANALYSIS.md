# Alternatives and Differentiation Analysis

Ops by Agent should not recreate mature tools merely to add an LLM interface. Each project must identify the gap it intends to address and show why integration, orchestration or a focused new capability is justified.

## Reference alternatives

These are starting points for evaluation, not endorsements or exhaustive comparisons.

| Area | Existing tools/services | Evaluation question |
|---|---|---|
| EKS operations | EKS APIs, kubectl, EKS console, EKS MCP Server | What operator workflow remains fragmented across resources and evidence? |
| Kubernetes analysis | K8sGPT | Does a troubleshooting agent add a demonstrable capability or should it integrate K8sGPT? |
| GitOps deployment | Argo CD, Flux | Can cross-system failure correlation reduce investigation effort? |
| Cost allocation | OpenCost, Kubecost, AWS Cost Explorer | Is the output actual billing, allocation, forecast or recommendation? |
| Security | Trivy, Kubescape, kube-bench, Kyverno, OPA Gatekeeper, Falco | Can an agent prioritize and explain scanner output without replacing scanners? |
| Observability | Prometheus, Grafana, Loki, CloudWatch, OpenTelemetry | Does the agent investigate signals rather than duplicate telemetry? |
| Autoscaling | HPA, VPA, Karpenter, Cluster Autoscaler, KEDA | Is the value diagnosis/advice rather than a competing controller? |
| Backup | Velero, Kasten, AWS Backup, EBS snapshots | Does it verify restore capability, not merely backup-job completion? |
| Incident management | PagerDuty, Rootly, Robusta, Grafana OnCall | Does it add evidence gathering while preserving operator authority? |
| Manifest analysis | KubeLinter, kube-score, Polaris, Checkov, Datree, Trivy | Does it contextualize established scanner results? |
| Runbooks | Backstage, Rundeck, StackStorm, SSM Automation | Are execution permissions, approvals and audit records safer? |

## Differentiation standard
A proposed agent must articulate:
1. Exact user and operational pain.
2. Workflow existing tools already support.
3. What remains unsolved or fragmented.
4. Why integration/orchestration is preferable to rebuilding.
5. Testable hypothesis for improvement.
6. Benchmark or scenario that can falsify the hypothesis.

Avoid vague claims such as "AI-powered", "intelligent", "autonomous" or "production-ready" without measurable behavior and evidence.

## Research hygiene
Record official documentation, repository links, release status, licensing, maintenance activity, integration mechanisms and limitations for material alternatives. Re-check current status before committing to a dependency. Treat previews and experimental APIs as optional until maturity and support boundaries are understood.
