# Technology Catalogue

This catalogue records technologies under consideration. It is not a mandate to use every tool. Select the simplest combination meeting approved project requirements, security posture, evaluation needs and cost envelope.

## Cloud and infrastructure
- **AWS:** target cloud environment.
- **Amazon EKS:** managed Kubernetes for Kubernetes-domain builds.
- **Amazon Bedrock:** managed foundation-model inference, subject to model, region, quota, data handling and cost validation.
- **Amazon ECR:** container image storage when required.
- **Amazon CloudWatch:** AWS logs, metrics and alarms where appropriate.
- **Terraform:** infrastructure as code where operational fit is justified.

## Agent runtime and orchestration
Evaluate LangGraph, Amazon Bedrock AgentCore and direct application orchestration against actual requirements. Compare persistence, tool calling, human approval, identity, observability, deployment complexity, failure semantics and cost. Do not commit solely because a framework is popular.

## Kubernetes access
Evaluate Kubernetes API/Python client, AWS EKS APIs, kubectl automation and MCP interfaces. Default to narrowly scoped read-only access. Validate every tool's permissions and side effects.

The Amazon EKS MCP Server was identified during programme research as a preview capability at the time of review. Treat it as optional and subject to change; do not make it a critical production dependency without a fresh readiness assessment.

## Language and interfaces
Python is the initial implementation-language candidate. FastAPI, CLI interfaces and GitHub integrations may be selected when useful. Keep interfaces typed, validated and documented.

## Observability and evaluation
Evaluate OpenTelemetry, Prometheus, Grafana, Loki, CloudWatch and task-specific evaluation harnesses. Evaluate groundedness, correctness, tool selection, safe refusal, authorization boundaries, latency and cost.

## Selection process
For each project document required capabilities/constraints, candidate tools and alternatives, selection rationale, security/data implications, operational complexity, AWS/model cost assumptions, limitations and fallback behavior.

Revalidate service/model availability, regional support, quotas, pricing and preview/GA status before implementation.
