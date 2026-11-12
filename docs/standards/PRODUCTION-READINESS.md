# Production-Readiness Standard

## Meaning
"Production-ready" is a claim about a specific version operating in a defined environment, under documented assumptions and ownership. It is not a synonym for "runs successfully" or "deployed to AWS."

## Required evidence

### Product and behavior
- Clear operational problem, users and supported workflows.
- Explicit scope, non-goals and limitations.
- Acceptance criteria and repeatable agent evaluations.
- Evidence-grounded outputs and safe uncertainty handling.

### Security
- Authentication and authorization.
- Least-privilege IAM and Kubernetes RBAC.
- Secret management and encryption.
- Threat model and security tests.
- Prompt-injection and untrusted-data controls.
- Auditable tool use and explicit human approval for side effects.

### Reliability
- Defined timeout, retry, rate-limit and error behavior.
- Health checks and dependency failure handling.
- Idempotency and recovery strategy where relevant.
- Backup/restore validation where state requires it.
- Rollback and upgrade procedure.

### Operations
- Structured logs, metrics, traces and actionable alerts.
- Runbooks, ownership and support expectations.
- Deployment and configuration documentation.
- Capacity, quotas and model availability considerations.
- Data retention and privacy decisions.

### Delivery and supply chain
- Automated tests and CI checks.
- Dependency and image scanning.
- Reproducible builds and release artifacts.
- Review of third-party licenses and notices.

### AWS and cost
- Real AWS deployment and integration evidence for AWS-dependent functionality.
- Reviewed IAM policies and network exposure.
- Cost estimate and measured usage where possible.
- Budget/alert configuration understood as detection rather than a hard cap.
- Verified teardown or explicit approval for persistent resources.

## Status labels
Report the highest evidenced level: implemented, locally tested, AWS deployed, AWS validated, released or production-ready. A project can be released without claiming production readiness.

## Review
Use a project-specific checklist. Record unmet controls as limitations or blockers; do not waive them silently.
