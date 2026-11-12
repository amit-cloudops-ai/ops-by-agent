# Project Release Checklist

A project is ready to be announced only when applicable items have evidence.

## Scope and differentiation
- [ ] Project-level approval recorded.
- [ ] Operational problem, user and acceptance criteria clear.
- [ ] Existing alternatives evaluated.
- [ ] Differentiation or integration rationale documented.
- [ ] Non-goals and limitations explicit.

## Design and security
- [ ] Architecture and data flows documented.
- [ ] Threat model and trust boundaries documented.
- [ ] Authentication and authorization tested.
- [ ] IAM and Kubernetes RBAC are least-privilege.
- [ ] Tool schemas and inputs validated.
- [ ] Read-only defaults and mutation approval enforced.
- [ ] Prompt injection and untrusted-tool output addressed.
- [ ] Audit events and secret redaction verified.

## Implementation and quality
- [ ] Implementation complete against approved scope.
- [ ] Unit and contract tests pass.
- [ ] Integration tests pass where required.
- [ ] Failure and security scenarios exercised.
- [ ] Agent evaluation results recorded.
- [ ] Dependencies and licenses reviewed.
- [ ] CI checks pass.

## AWS and operations
- [ ] AWS region, services and deployment design documented.
- [ ] Cost estimate reviewed before provisioning.
- [ ] Actual deployed resources inventoried.
- [ ] AWS-dependent functionality validated in AWS.
- [ ] Logs, metrics and operational health checked.
- [ ] Rollback/recovery instructions documented.
- [ ] Teardown executed and verified, or persistence explicitly approved.

## Public release
- [ ] README and usage instructions accurate.
- [ ] Reproduction commands and prerequisites complete.
- [ ] Screenshots and diagrams reflect actual implementation.
- [ ] No secrets, customer data or unsafe sample configuration.
- [ ] Limitations and validation level stated honestly.
- [ ] Changelog/release notes updated.
- [ ] Root README updated only with demonstrated capability.
