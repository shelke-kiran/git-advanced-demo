# Advanced Git Workflow Demo

This repository is configured with enterprise-grade **Pull Request Gates** to enforce quality control, formatting standards, and audit checkpoints prior to code integration.

## Implemented PR Gates
This repository utilizes a custom GitHub Actions workflow (`pr-gate.yml`) that validates:
1. **Conventional Commits**: PR titles must conform to standardized prefixes (e.g., `feat:`, `fix:`, `chore:`, `docs:`).
2. **Branch Protection Enforcements**: Ensures the incoming code merges cleanly and passes formatting rules.

## Recommended Branch Strategy
We recommend following the **GitHub Flow** branches structure:
* `main`: Stable production branch. Fully locked and only updatable via approved PRs.
* `feat/*`: Feature development branches.
* `fix/*`: Bugfix branches.
* `chore/*`: Maintenance tasks.
