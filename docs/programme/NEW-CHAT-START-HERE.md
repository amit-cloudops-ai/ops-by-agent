# New Chat: Start Here

Use this document as the starting point for every new Ops by Agent project conversation.

## Copy/paste prompt

I am continuing the Ops by Agent programme in this public GitHub repository:

https://github.com/amit-cloudops-ai/ops-by-agent

**The repository is the source of truth. Do not rely on previous ChatGPT conversation history.**

Before project work, read:
1. `README.md`
2. `docs/programme/PROGRAMME-OVERVIEW.md`
3. `docs/programme/MASTER-ROADMAP.md`
4. `docs/programme/TECHNICAL-DECISIONS.md`
5. `docs/programme/BUILD-CADENCE.md`
6. `docs/architecture/SYSTEM-ARCHITECTURE.md`
7. Relevant files in `docs/architecture/`, `docs/standards/` and `docs/operations/`
8. The selected project's approval record, plan, handoff, status, testing, deployment, cost and next-steps documents.

The programme builds AI agents for real operational engineering. Kubernetes is the first domain. AWS is the deployment/validation target; Amazon Bedrock is the preferred inference service subject to project-specific model, region, security and cost checks.

Do not assume any planned project is approved. Do not provision, modify or delete AWS resources without explicit project-specific approval and a reviewed cost estimate. Never commit credentials.

Your first response should summarize repository project status and identify the next concrete task from the project's handoff. Do not restart research or create another planning checklist if the repository already answers it.

## Before ending a project chat

Update the repository with current implementation status, exact commands and test results, commit/branch references, AWS resources and teardown state, decisions, defects, limitations and one next action. Ensure the next chat can resume from those files alone.
