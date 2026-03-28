# Contributing to Nightwatch Astro

Thanks for your interest in contributing! This guide applies to all repositories in the [nightwatch-astro](https://github.com/nightwatch-astro) organization.

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
