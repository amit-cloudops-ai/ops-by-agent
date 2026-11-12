# AWS Account Safety

## Scope
Applies to project work that can read, create, modify or delete AWS resources.

## Preflight
- Confirm intended AWS account through an approved identity check.
- Confirm region and allowed services.
- Confirm project approval and deployment window.
- Review planned IAM permissions and network exposure.
- Estimate cost and identify uncertainty.
- Confirm resource tags/naming and teardown ownership.
- Verify changes will not affect unrelated workloads.

## Execution
Use explicit profiles/roles and regions. Prefer plan/preview modes before apply. Require human confirmation immediately before resource creation or destructive operations. Capture sanitized evidence.

## Stop conditions
Stop if account/region is ambiguous, costs exceed approval, permission scope expands unexpectedly, resource ownership is unclear, unexpected public exposure appears or unexpected charges are observed.

## Cleanup
Follow [Teardown Policy](TEARDOWN-POLICY.md). Verify all relevant regions and service dependencies. Do not delete unrelated resources.

## Repository setup
Repository initialization is a GitHub-only operation. It creates no AWS resources and requires no AWS credentials.
