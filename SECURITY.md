# Security Policy

## Reporting a security issue

If you discover a potential security vulnerability in Estimate Drift Watch for Jira, please report it privately by email:

souchet@wanadoo.fr

Please do not disclose security vulnerabilities publicly through GitHub Issues.

## Information to include

If possible, include:

- a description of the issue;
- steps to reproduce it;
- affected Jira functionality;
- screenshots or logs where relevant;
- the potential impact.

Do not include passwords, API tokens, credentials, or other secrets.

## Architecture

Estimate Drift Watch is built on Atlassian Forge.

The app does not use an external application backend or external database for Jira issue data.

Processing is performed using Atlassian-hosted Forge infrastructure and Jira APIs.

## Data handling

The app does not intentionally transmit Jira end-user data to external third-party services.

The app does not use external analytics or advertising trackers.

## Response

Security reports will be reviewed as soon as reasonably possible.

Confirmed vulnerabilities will be investigated and addressed according to their severity and impact.
