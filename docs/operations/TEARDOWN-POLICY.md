# Teardown Policy

## Default
Project infrastructure is temporary by default. Persistent AWS environments require explicit approval, an owner, a cost envelope and a reason to remain available.

## Teardown inventory
Enumerate resources created directly and indirectly, including EKS clusters, node groups, EC2 instances, EBS volumes/snapshots, load balancers, NAT gateways, public IPs, security groups, IAM roles/policies, ECR repositories/images, CloudWatch log groups, S3 buckets/objects, databases, queues, event rules and Bedrock-related provisioned resources where applicable.

## Safe sequence
1. Stop workloads and prevent new activity.
2. Preserve only approved evidence and artifacts.
3. Remove dependent services in dependency order.
4. Delete infrastructure stacks and standalone resources.
5. Verify resource absence in every region touched.
6. Review billing/cost data after service data becomes available.
7. Record completion and any residual resources or delayed charges.

## Safety
Do not delete shared or unrelated resources. Use explicit project tags and recorded resource identifiers. If ownership is ambiguous, stop and investigate.

## Completion record
Record timestamp, regions checked, commands/console evidence, resources removed, resources retained with approval and residual risk.
