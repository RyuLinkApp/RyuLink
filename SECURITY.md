# Security Policy

RyuLink takes security reports seriously, especially issues involving authentication, account access, update integrity, relay abuse, or unintended exposure of user or server data.

## Reporting a security issue

Please **do not** publish exploit details, credentials, tokens, private keys, or sensitive server information in a public GitHub Issue.

Preferred reporting path:

1. If GitHub shows a **Report a vulnerability** option in the repository Security area, use that private reporting flow.
2. If private vulnerability reporting is not available, open a minimal public Issue with a title such as `Security report — private contact requested` and include **no sensitive technical details**. A maintainer can then arrange a private channel.

## What to include privately

When a private channel is available, please provide:

- A clear description of the issue
- Affected RyuLink version or service
- Reproduction steps or proof of concept
- Expected impact
- Any relevant logs with secrets removed
- Whether the issue is already public or known elsewhere

## Scope

Security reports may include, but are not limited to:

- Authentication or authorization bypass
- Account or entitlement abuse
- Remote code execution
- Update or package integrity issues
- Exposure of secrets or personal data
- Cross-room or cross-user isolation failures
- Server-side request abuse or denial-of-service vectors

Normal compatibility problems, connection failures, or game-specific bugs should use the regular Bug Report template instead.

## Disclosure

Please allow maintainers a reasonable opportunity to investigate and release a fix before publicly disclosing sensitive details.

RyuLink is currently in public beta, so security processes and supported versions may evolve as the project matures.
