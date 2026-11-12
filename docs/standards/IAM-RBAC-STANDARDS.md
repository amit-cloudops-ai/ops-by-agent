# IAM and Kubernetes RBAC Standards

## AWS IAM
- Use dedicated roles per workload and environment.
- Grant only required actions on the narrowest practical resources.
- Prefer short-lived role sessions and workload identity.
- Avoid static access keys and wildcard policies.
- Separate deployment, runtime and human operator roles.
- Review trust policies, permission boundaries and cross-account access.
- Record required actions and rationale.

## Kubernetes RBAC
- Use dedicated service accounts and namespace/resource scoping where possible.
- Prefer get/list/watch for inventory and analysis.
- Avoid wildcard verbs, resources and API groups.
- Separate read and write roles.
- Do not grant cluster-admin to an agent runtime.
- Validate impersonation and escalation paths.

## Human approval
An approver must be authorized for the target environment. Approval identifies the exact action, target, parameters and expiry.

## Verification
Test allowed and denied actions. Review effective permissions, not just policy intent. Revalidate when tools or workflows change.
