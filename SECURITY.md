# Security Policy

## Reporting a vulnerability
Report suspected vulnerabilities privately to the Method engineering lead (or
security@methodcommunications.com) — do **not** open a public issue. Include
steps to reproduce and impact. We aim to acknowledge within 2 business days.

## Secrets
- **Never commit secrets.** Service-account JSON, `.env` files, API keys, and
  tokens are gitignored and must stay out of git history.
- If a secret is ever committed, **rotate it immediately** and notify the lead;
  removing the file is not enough (git history retains it).
- Provide secrets to deployments via environment variables / a secret manager,
  not the repo.
