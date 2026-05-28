# agents.md -- Marketplace Issues

## Repository Overview

Issue-only repository for tracking bugs and feature requests related to the ownCloud Marketplace. Contains no code. Archived/legacy status.

- **Product family:** Community / Meta
- **Primary language(s):** Markdown

## Architecture & Key Paths

- No code paths -- this is an issue tracker only.
- Issues are categorized using GitHub labels for priority and component area.

## Development Conventions

- Issue-only repository -- no code contributions expected.
- Follow the existing label taxonomy when triaging new issues.

## Build & Test Commands

N/A -- no code to build.

## Important Constraints

- No license detected. The OSPO is reviewing licensing for all repositories, with a goal of migrating to Apache 2.0 where possible. Repos with copyleft dependencies require auditing first.
- Do not introduce new **copyleft-licensed dependencies** (GPL, AGPL, LGPL, MPL) without explicit discussion in an issue first. This is especially important for repos that are migrating to or already under Apache 2.0, as copyleft dependencies would block or complicate that migration.
- Archived/legacy repository.
- All contributions require a DCO sign-off.


## OSPO Policy Constraints

### GitHub Actions
- **Only** use actions owned by `owncloud`, created by GitHub (`actions/*`), verified on the GitHub Marketplace, or verified by the ownCloud Maintainers.
- Pin all actions to their full commit SHA (not tags): `uses: actions/checkout@<SHA> # vX.Y.Z`
- Never introduce actions from unverified third parties.

### Dependency Management
- Dependabot is configured for automated dependency updates.
- Review and merge Dependabot PRs as part of regular maintenance.
- Do not introduce new dependencies without discussion in an issue first.

### Git Workflow
- **Rebase policy**: Always rebase; never create merge commits. Use `git pull --rebase` and `git rebase` before pushing.
- **Signed commits**: All commits **must** be PGP/GPG signed (`git commit -S -s`).
- **DCO sign-off**: Every commit needs a `Signed-off-by` line (`git commit -s`).
- **Conventional Commits & Squash Merge**: Use the [Conventional Commits](https://www.conventionalcommits.org/) format where the repository enforces it. Many repos use squash merge, where the PR title becomes the commit message on the default branch — apply Conventional Commits format to PR titles as well. A reusable GitHub Actions workflow enforces this.

## Context for AI Agents

This repository exists solely for issue tracking. There is no code to modify.
