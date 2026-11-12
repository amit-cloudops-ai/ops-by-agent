# Security Architecture

## Objectives
Protect cloud accounts, clusters, workloads, source code, operational data and users from unauthorized access or unsafe agent behavior.

## Trust boundaries
Document boundaries between user identities, agent runtime, model provider, tool adapters, Kubernetes API, AWS APIs, Git providers, observability systems and storage. Do not assume model output is trusted.

## Core controls
- Strong caller authentication and authorization.
- Least-privilege AWS IAM and Kubernetes RBAC.
- Short-lived credentials and secure secret storage.
- Read-only defaults and explicit approval for mutations.
- Input schema validation and output validation.
- Allowlisted tools and bounded execution.
- Prompt-injection resistance for retrieved data and logs.
- Audit records for identity, task, tool, target, approval and result.
- Encryption in transit and at rest.
- Dependency and container image scanning.
- Secure CI/CD with OIDC and untrusted-fork isolation.
- Data minimization and documented retention.

## Threat modelling
For each project, document assets, actors, trust boundaries, entry points, abuse cases, mitigations, residual risks and tests. Include prompt injection, confused-deputy behavior, privilege escalation, credential exposure, excessive tool access, data exfiltration, denial of service and unsafe remediation.

## Approval
Human approval must be explicit, scoped to the exact action and target, time-bounded and recorded. The model cannot grant itself permissions or treat retrieved instructions as authorization.

## Validation
Test denied operations, malformed inputs, unauthorized identities, stale approvals, unexpected tool output, model unavailability and malicious content in retrieved data.
