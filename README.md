# ZiYan416 · Open Source Maintenance

This is the public account-level `.github` repository for shared open-source community standards and reusable CI workflows.

## What is inherited?

GitHub automatically uses the default issue forms, pull-request template, contribution guidelines, code of conduct, support guide, and security policy **only when the destination repository does not define its own version**.

Repository-specific files, dependency updates, branch rulesets, license selection, and CI triggers are **not** globally inherited.

The original maintenance configuration is licensed under MIT. This license **does not grant licenses to code in other repositories**.

## Reusable workflows

- `.github/workflows/reusable-repository-check.yml`: general repository documentation check
- `.github/workflows/reusable-node-ci.yml`: npm lockfile, lint, typecheck, tests, build
- `.github/workflows/reusable-python-ci.yml`: uv lockfile and pytest

Use `ZiYan416/.github/.github/workflows/<filename>@main` from a caller repository. For long-term stability, pin the caller to a reviewed release tag or commit SHA rather than `main`.

Existing projects must keep their project-specific CI until the replacement is verified.

## Deployment

Run the root `bootstrap.ps1` from the distributed maintenance package using an authenticated GitHub CLI. The script creates only two **new public repositories**: `ZiYan416/.github` and `ZiYan416/open-source-starter`; it does not modify existing projects or their visibility.
