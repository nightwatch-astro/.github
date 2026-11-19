# Contributing to Nightwatch Astro

Thanks for your interest in contributing! This guide applies to all repositories in the [nightwatch-astro](https://github.com/nightwatch-astro) organization.

## Contributor License Agreement (CLA)

These repositories require a CLA for all contributions. When you open your first pull
request, the CLA Assistant bot will comment with a link to review and sign the
agreement. You only need to sign once — it covers all future contributions to
the nightwatch-astro repositories. The agreement text is in [`CLA.md`](CLA.md) and in a
[public gist](https://gist.github.com/srobroek/33b6a2146c71597c2309d6ad0f93b304) that CLA Assistant reads. A change to `CLA.md`
must update the gist in the same change.

**Why?** The CLA ensures the project maintainer retains the ability to offer the
code under alternative licensing terms (e.g., a commercial license) without
needing to track down every contributor individually. Your contribution remains
publicly available under each project's open-source license regardless.

## Getting Started

1. Fork the repository
2. Clone your fork
3. Create a feature branch (`feat/description` or `fix/description`)
4. Make your changes
5. Push and open a Pull Request

## Commit Convention

All repositories use [conventional commits](https://www.conventionalcommits.org/):

```
feat(scope): add new feature
fix(scope): fix a bug
docs: update documentation
test: add or update tests
refactor(scope): restructure code without behavior change
perf(scope): improve performance
chore: maintenance tasks
```

## Code Quality

### Rust projects

```bash
cargo test          # run tests
cargo clippy        # lint
cargo fmt --check   # format check
```

### Web projects

```bash
pnpm install
pnpm test
pnpm lint
```

## Pull Request Process

1. Ensure all tests pass and linters are clean
2. Use conventional commit messages
3. Reference related issues in the PR description (`Fixes #123`)
4. Keep PRs focused — one logical change per PR

## Releases

Releases are automated via [release-plz](https://release-plz.ieni.dev/). When a PR is merged to `main`, release-plz creates a release PR with version bump and changelog. Merging the release PR publishes to crates.io and creates a GitHub release.

Do NOT manually bump versions or create releases.

## Questions?

Open an issue in the relevant repository. For general questions, use the [Discussions](https://github.com/orgs/nightwatch-astro/discussions) tab (if enabled) or file an issue.
