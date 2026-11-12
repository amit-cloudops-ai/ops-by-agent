# AWS Cost Management

## Policy
No AWS resource may be provisioned for a project until scope, region, estimated cost, test duration, owner and teardown plan have been reviewed and approved.

## Cost inventory
Consider applicable charges: EKS cluster/control-plane, EC2 or other compute, EBS volumes/snapshots, NAT gateways, public IPv4, data transfer, load balancers, CloudWatch logs/metrics/alarms/retention, ECR storage/transfer, Bedrock inference or provisioned throughput, S3, DynamoDB, queues, orchestration and supporting services.

Services and prices vary by region, configuration and date. Recalculate before deployment using current AWS pricing and service availability.

## Estimates and monitoring
Document assumptions, expected duration, usage volume and low/expected/high scenarios. Configure budgets and alerts where appropriate, but do not treat them as guaranteed hard spend limits.

Track actual usage and stop tests when the approved envelope is reached or unexpected charges appear.

## Temporary environments
Prefer short-lived environments. Record resource names/tags and ownership so cleanup is reliable. Do not leave clusters, NAT gateways, load balancers, volumes, snapshots or log groups unintentionally.

## Teardown verification
After cleanup, inspect relevant regions/account for remaining resources, dependencies and delayed charges. Save commands and evidence. Teardown is not complete merely because the primary stack was deleted.

## Approval record
Each estimate includes region, services, quantity, unit assumptions, duration, estimated total, uncertainty, cost alarms and teardown owner.
