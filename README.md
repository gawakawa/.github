# Reusable Workflows

Reusable GitHub Actions workflows for a personal account (not organization-level).

Usage examples are documented as comments at the top of each workflow file.

## Workflows

- [`update-pr-branches.yml`](.github/workflows/update-pr-branches.yml) — Update open PR branches to keep them up to date with their base.
- [`update-flake-lock.yml`](.github/workflows/update-flake-lock.yml) — Open a PR that updates `flake.lock` (with an optional auto-merge).
- [`dependabot-auto-merge.yml`](.github/workflows/dependabot-auto-merge.yml) — Enable auto-merge on Dependabot PRs.

## Prerequisites

`update-pr-branches` and `update-flake-lock` require the gawakawa-bot GitHub App to be installed on the caller repository, with `BOT_APP_ID` and `BOT_PRIVATE_KEY` secrets configured.
