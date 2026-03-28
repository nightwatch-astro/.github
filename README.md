# nightwatch-astro/.github

Organization-wide defaults for [nightwatch-astro](https://github.com/nightwatch-astro) repositories.

## What's here

| Path | Purpose |
|------|---------|
| `.github/workflows/` | Reusable CI/CD workflows (Rust release, etc.) |
| `.github/ISSUE_TEMPLATE/` | Default issue templates for repos without their own |
| `.github/PULL_REQUEST_TEMPLATE.md` | Default PR template |
| `profile/README.md` | Organization profile (shown on github.com/nightwatch-astro) |
| `CONTRIBUTING.md` | Default contributing guide |
| `CODE_OF_CONDUCT.md` | Contributor Covenant Code of Conduct |
| `SECURITY.md` | Security vulnerability reporting policy |
| `.github/FUNDING.yml` | Organization-wide sponsor links |

## Reusable workflows

### `rust-release.yml`

Automated Rust crate release via [release-plz](https://release-plz.ieni.dev/). Creates release PRs with changelogs and publishes to crates.io on merge.

```yaml
# In your repo's .github/workflows/release.yml:
name: Release
on:
  push:
    branches: [main]
jobs:
  release:
    uses: nightwatch-astro/.github/.github/workflows/rust-release.yml@main
    secrets: inherit
```

**Required org secrets:** `NIGHTWATCH_APP_ID`, `NIGHTWATCH_APP_PRIVATE_KEY`, `CARGO_REGISTRY_TOKEN`

## How defaults work

GitHub automatically uses files from this repo as defaults for all repositories in the organization. Repos can override any default by adding their own version of the file. For example:

- A repo with its own `.github/ISSUE_TEMPLATE/` will use those templates instead of the defaults here
- A repo with its own `CONTRIBUTING.md` will display that instead of this one
- Reusable workflows must be explicitly referenced with `uses:` — they don't auto-apply
