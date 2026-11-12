# AWS Architecture

## Target environment
AWS is the target environment for project deployments and cloud validation. Local development may be used for editing, unit tests and fast feedback, but does not substitute for required AWS integration and operational validation.

## Candidate services
Select only what the approved project needs:
- Amazon EKS for Kubernetes workloads.
- Amazon Bedrock for managed model inference.
- Amazon ECR for container images.
- IAM and EKS access/RBAC mechanisms for scoped authorization.
- CloudWatch for AWS logs, metrics and alarms where appropriate.
- VPC networking and security groups designed for minimum exposure.
- S3, DynamoDB, SQS, EventBridge or Step Functions only when justified.

## Identity
Prefer short-lived credentials and workload identity mechanisms such as IAM roles and EKS Pod Identity where supported. GitHub Actions should use OIDC federation rather than long-lived AWS access keys. Never commit credentials.

## Region and service validation
Before deployment, verify regional availability, model access, quotas, service maturity, API versions and pricing. Do not assume a service or model is available in the chosen region.

## Cost controls
Every project requires a cost estimate before provisioning. Identify charges for control planes, compute, storage, networking, load balancers, logging, registries and model inference. Budgets and alerts are detection controls, not guaranteed spend caps.

Prefer temporary environments and provision only for a defined test window. Teardown must include dependencies and verification of remaining billable resources.

## Security
Use private networking where practical, least-privilege IAM, encryption in transit and at rest, secure secret management, restricted ingress and explicit data retention. Validate service-specific data handling for information sent to model providers.

## Repository-only setup
This documentation commit creates no AWS resources and makes no claim of AWS deployment or validation.
