# New Chat: Start Here

Use this document as the starting point for every new Ops by Agent project conversation.

## Copy/paste prompt

I am continuing the Ops by Agent programme in this public GitHub repository:

https://github.com/amit-cloudops-ai/ops-by-agent

**The repository is the source of truth. Do not rely on previous ChatGPT conversation history.**

Read the root `README.md`, then the programme overview, technical decisions, build cadence, shared architecture and the relevant security, testing, production-readiness, AWS cost, deployment and teardown standards.

For the first build, the selected candidate is K01 — Cluster Intelligence Agent. Do not assume implementation scope is approved merely because the programme is approved. First prepare a concise K01 project brief, alternatives/differentiation assessment, AWS architecture, cost estimate, acceptance criteria and test/evaluation plan. Wait for explicit project approval before code changes or AWS provisioning.

The programme builds AI agents for real operational engineering. Kubernetes is the first domain. AWS is the deployment/validation target; Amazon Bedrock is the preferred inference service subject to project-specific model, region, security and cost checks.

Local development and tests are useful, but they do not replace AWS integration and operational validation. Do not provision, modify or delete AWS resources without explicit project-specific approval and a reviewed cost estimate. Never commit credentials.

Your first response should summarize the repository's current state and identify the next concrete step. Do not restart broad research or create another planning checklist where the repository already supplies the answer.

## Before ending a project chat

Update the repository with current implementation status, exact commands and test results, commit/branch references, AWS resources and teardown state, decisions, defects, limitations and one next action. Ensure the next chat can resume from those files alone.
