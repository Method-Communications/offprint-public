# Contributing

Thanks for contributing to a Method Communications project.

## Branching
- Branch off `main`: `feature/<short-name>`, `fix/<short-name>`, or `chore/<short-name>`.
- Keep pull requests small and focused.

## Pull requests
- `main` is protected — changes land via PR with at least one review, and code-owner
  approval where a `CODEOWNERS` file applies.
- Fill in the summary, testing notes, and risk. Resolve all review conversations before merge.
- CI must be green where configured.

## Commit messages
- Imperative mood, present tense: "add X", "fix Y". Reference issues where relevant (`#123`).

## Security
- Never commit secrets (`.env`, keys, service-account JSON). See `SECURITY.md`.
- Report vulnerabilities privately per `SECURITY.md` — do not open a public issue.
