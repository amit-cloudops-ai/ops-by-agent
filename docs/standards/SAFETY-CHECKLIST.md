# Kubernetes Agent Safety Checklist

A practical review checklist for engineers designing or operating an AI agent that can inspect Kubernetes or AWS environments.

This checklist is a starting point, not a certification or substitute for a project-specific threat model, security review or operational approval.

## 1. Identity and access

- [ ] Authenticate the human or workload that initiated the task.
- [ ] Bind each task to a clear principal and environment.
- [ ] Use a dedicated runtime IAM role.
- [ ] Use short-lived credentials; do not store static AWS keys in source code or images.
- [ ] Use a dedicated Kubernetes service account.
- [ ] Scope Kubernetes RBAC to only the resources and verbs required.
- [ ] Avoid wildcard permissions and cluster-admin.
- [ ] Test denied operations as deliberately as allowed ones.

## 2. Tool boundaries

- [ ] Expose only an explicit allowlist of tools.
- [ ] Define and validate input/output schemas.
- [ ] Enforce target cluster, namespace and resource scope in application code.
- [ ] Set timeouts, bounded retries, rate limits and payload limits.
- [ ] Classify tools as read-only or mutating.
- [ ] Do not expose unrestricted shell execution or a general-purpose cloud API proxy.
- [ ] Treat model output as untrusted input.

## 3. Human approval and side effects

- [ ] Keep read-only inspection as the default.
- [ ] Require explicit approval before changes to workloads, policies, IAM, networking or data.
- [ ] Bind approval to the exact action, target and parameters.
- [ ] Expire approvals and require a new one when parameters change.
- [ ] Record who approved, what was approved and the result.
- [ ] Provide a safe way to stop or disable execution.

## 4. Prompt injection and untrusted data

- [ ] Treat logs, annotations, labels, manifests, tickets and tool output as data—not instructions.
- [ ] Ensure retrieved text cannot override system policy or authorize actions.
- [ ] Test malicious instructions embedded in workload metadata and logs.
- [ ] Prevent tool output from injecting new tools or changing permissions.
- [ ] Separate observed facts, hypotheses and recommendations.

## 5. Secrets and sensitive data

- [ ] Keep credentials out of Git, logs, screenshots and issue reports.
- [ ] Store secrets in an appropriate secret manager.
- [ ] Redact tokens, private keys, passwords and personal data.
- [ ] Minimize data sent to model providers.
- [ ] Document retention, access and deletion behavior.
- [ ] Review model/service data-handling terms for the selected region and configuration.

## 6. Reliability and observability

- [ ] Handle unavailable clusters, APIs, models and telemetry sources.
- [ ] Use bounded retries and idempotency for applicable operations.
- [ ] Emit structured logs with correlation IDs.
- [ ] Record tool calls, outcomes, latency and model usage without leaking secrets.
- [ ] Alert on repeated failures, denied access and unexpected side effects.
- [ ] Document recovery and rollback behavior.

## 7. Evaluation

- [ ] Test normal tasks and ambiguous tasks.
- [ ] Test missing, stale and contradictory evidence.
- [ ] Test unauthorized identities and forbidden tool calls.
- [ ] Test prompt injection in retrieved data.
- [ ] Measure groundedness, task completion, tool selection and safe abstention.
- [ ] Record failures and false positives—not only successful examples.
- [ ] Track latency and inference cost.

## 8. AWS cost and cleanup

- [ ] Estimate charges before provisioning.
- [ ] Account for EKS, compute, storage, networking, load balancers, logs, registries and model inference where applicable.
- [ ] Define region, test window and owner.
- [ ] Configure cost alerts where appropriate; do not treat budgets as a hard spending cap.
- [ ] Tag or otherwise record resources created by the project.
- [ ] Execute teardown and verify dependent resources are removed.
- [ ] Record residual resources and delayed-cost risks.

## Final review

A checked box means there is evidence for the control in the specific project and environment. It is not enough that the design document mentions it.

**Review date:**  
**Project/version:**  
**Reviewer:**  
**Exceptions and residual risks:**  
**Evidence links:**  
