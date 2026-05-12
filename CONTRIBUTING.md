# Contributing — Conventional Commits

This repository follows the "Conventional Commits" specification (v1.0.0).
For more information: https://www.conventionalcommits.org/en/v1.0.0/

Please format your commit messages according to the rules below. This helps keep the history readable, enables automated versioning, and simplifies changelog generation.

Basic format

type(scope?): subject

body?

footer?

Rules

- type: a lowercase word describing the change. Recommended types:
  - feat: add a new feature
  - fix: bug fix
  - docs: documentation changes
  - style: formatting, lint, whitespace, semicolons (no code change)
  - refactor: code changes that neither add a feature nor fix a bug
  - perf: performance improvement
  - test: adding or fixing tests
  - build: changes affecting the build system or dependencies
  - ci: changes to CI scripts or configurations
  - chore: maintenance tasks that don't modify production code
  - revert: revert a previous commit

- scope (optional): area affected (e.g., auth, api, cli)
- subject: short description (imperative), no trailing period
- body: detailed explanation if necessary (separated by a blank line)
- footer: metadata (issue references, BREAKING CHANGE, etc.)

BREAKING CHANGES

If a commit introduces incompatible changes, include in the footer:

BREAKING CHANGE: description of the incompatibility and required migrations

Examples

- feat(auth): add JWT token refresh
- fix(api): handle null pointer on user lookup
- docs: update contributing guide
- chore(deps): update eslint to v8
- feat: add CLI --init command
- fix: correct crash when file missing

Best practices

- Use the imperative mood for the subject (Add, Fix, Update)
- Keep the subject short (<= 50 characters preferred)
- Separate the body from the subject with a blank line
- Reference issues in the footer (e.g., Closes #123)

Tools

Consider using tools to validate commit messages: commitlint, husky, semantic-release, conventional-changelog, etc.

Reference

https://www.conventionalcommits.org/en/v1.0.0/

Thanks for your contributions!

```
