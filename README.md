# Reusable Workflows

Reusable GitHub Actions workflows for a personal account (not organization-level).

Usage examples are documented as comments at the top of each workflow file.

## Workflows

- [`update-pr-branches.yml`](.github/workflows/update-pr-branches.yml) — Update open PR branches to keep them up to date with their base.
- [`update-flake-lock.yml`](.github/workflows/update-flake-lock.yml) — Open a PR that updates `flake.lock` (with an optional auto-merge).
- [`auto-assign.yml`](.github/workflows/auto-assign.yml) — Assign the PR author as the PR's assignee when a PR is opened.
- [`dependabot-auto-merge.yml`](.github/workflows/dependabot-auto-merge.yml) — Enable auto-merge on Dependabot PRs.
- [`claude.yml`](.github/workflows/claude.yml) — Run Claude Code when an issue or PR comment mentions @claude.
- [`claude-code-review.yml`](.github/workflows/claude-code-review.yml) — Automatically review pull requests with Claude Code.

## Prerequisites

`update-pr-branches`, `update-flake-lock`, and `auto-assign` require the gawakawa-bot GitHub App to be installed on the caller repository, with `BOT_APP_ID` and `BOT_PRIVATE_KEY` secrets configured.

`claude` and `claude-code-review` require a `CLAUDE_CODE_OAUTH_TOKEN` secret configured in the caller repository.
