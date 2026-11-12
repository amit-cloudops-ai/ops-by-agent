# Security Policy

## Scope
Reports may concern application code, agent behavior, infrastructure definitions, IAM policies, deployment workflows, supply-chain risks, data handling or documentation that could lead to unsafe operation.

## Reporting
**Do not report exploitable vulnerabilities in public issues or pull requests.**

Use GitHub's private vulnerability reporting feature for this repository when available. If it is unavailable, contact the maintainer privately through the contact details on the maintainer's GitHub profile.

Include a concise description, impact, affected components/versions, reproduction steps, sanitized logs and suggested mitigation when possible.

Do not access, modify, destroy or exfiltrate data that is not yours. Do not disrupt live services or test infrastructure without explicit authorization.

## Response and disclosure
The maintainer will assess reports, request clarification where necessary and coordinate fixes and disclosure. No response-time SLA is promised at this stage.

## Secrets
If a credential is committed, revoke or rotate it immediately. Removing it from Git history does not make it safe. Report the exposure privately and review relevant access logs.
