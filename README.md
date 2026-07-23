# python-ci-template

Template repository with GitHub Actions CI for Python projects.

## What's included

A CI workflow (`.github/workflows/ci.yml`) that runs on every push and PR to main:

| Job | Tool | What it checks |
|-----|------|---------------|
| **Lint** | ruff | Code style, formatting, import sorting |
| **Type Check** | mypy | Static type errors |
| **Security Scan** | pip-audit | Known CVEs in dependencies |

All three jobs run in parallel.

## Usage

### New repos
Click **"Use this template"** on GitHub to create a new repo with this CI setup.

### Existing repos
Copy these into your repo:
- `.github/workflows/ci.yml`
- The `[tool.ruff]` and `[tool.mypy]` sections from `pyproject.toml`
