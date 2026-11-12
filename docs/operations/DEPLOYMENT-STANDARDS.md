# Deployment Standards

## Before deployment
- Confirm project-level approval and deployment scope.
- Validate AWS account and region explicitly.
- Review cost estimate and test window.
- Review IAM, Kubernetes RBAC, networking and secrets.
- Validate infrastructure plans and artifacts.
- Confirm teardown and rollback procedures.

## Deployment
Prefer infrastructure as code for repeatability. Pin versions, avoid public exposure unless required, and use least-privilege workload identity. Do not embed credentials in images, manifests, state files or logs.

## Validation
Verify health, identity, tool authorization, normal workflows, error handling, audit records and operational telemetry. Capture reproducible evidence and distinguish smoke tests from full integration tests.

## Rollback
Document rollback triggers, supported steps, data/state implications and recovery verification.

## After deployment
Record resource identifiers in an appropriately protected project record, monitor cost and complete the approved teardown unless persistence has explicit approval.
