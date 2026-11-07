# Contributing to LLCForge projects

Thanks for taking the time to contribute! This document applies to every repository under
[github.com/LLCForge](https://github.com/LLCForge) unless the repository has its own `CONTRIBUTING.md`.

## Before you start

- **Search first.** Check open and closed issues and the Discussions tab — your idea or bug may already be tracked.
- **Open an issue for anything non-trivial.** Bug fixes and docs can go straight to a pull request; new features,
  behaviour changes and refactors should start as an issue so we can agree on scope and approach.
- **One change per pull request.** Small, focused PRs get reviewed and merged much faster.

## Development workflow

1. Fork the repository and create a branch from `main`:
   `git checkout -b feat/short-description` (or `fix/…`, `docs/…`, `chore/…`).
2. Follow the toolchain versions pinned in the repository (`go.mod`, `rust-toolchain.toml`, `.nvmrc`, …).
3. Run the formatter, linter and the full test suite locally before pushing — the commands are in the repository README.
4. Write tests for new behaviour and for every bug you fix.
5. Update documentation (README, `docs/`, CLI help) when behaviour or configuration changes.

## Commit messages

We use [Conventional Commits](https://www.conventionalcommits.org/):

```
feat(api): add rate-limit headers to /v1/solve
fix(agent): do not retry on 4xx responses
docs: clarify docker compose quick start
```

Types: `feat`, `fix`, `docs`, `refactor`, `perf`, `test`, `build`, `ci`, `chore`. Add `!` after the type
(or a `BREAKING CHANGE:` footer) for breaking changes. Reference issues in the footer: `Closes #123`.

## Pull requests

- Fill in the PR template: what changed, why, how it was tested, screenshots for UI changes.
- CI must be green. Flaky tests should be fixed or reported, not re-run until they pass.
- A maintainer will review within a few days. Please respond to review comments; stale PRs are closed after 30 days of silence.
- Squash-merge is the default; keep the PR title in conventional-commit form, it becomes the commit message.

## Code style

- Go: `gofmt` + `golangci-lint`; Rust: `cargo fmt` + `cargo clippy -D warnings`; TypeScript: Prettier + ESLint.
- Prefer clarity over cleverness. Comments explain *why*, the code explains *what*.
- No new dependencies without a short justification in the PR description.

## Reporting bugs

A good bug report includes: the version or commit, your OS/architecture, exact steps to reproduce,
what you expected, what happened instead, and relevant logs (redact secrets!).

## Security issues

Never open a public issue for a security problem. See [SECURITY.md](SECURITY.md).

## License

By contributing you agree that your contributions are licensed under the license of the repository
you contribute to (MIT or Apache-2.0 unless stated otherwise).
