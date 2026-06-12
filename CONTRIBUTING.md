# Contributing to Pixium

Welcome! Pixium is a community-built project and contributions of all kinds are welcome — smart contracts, backend, frontend, indexer, documentation, and testing.

---

## How It Works

1. Browse open issues across the repos
2. Comment on an issue to claim it — wait for a maintainer to assign it to you
3. Fork the repo and create a branch
4. Submit a pull request referencing the issue
5. Address review feedback and get merged

**Good first issues** are labeled for contributors new to the project.

---

## Repositories

| Repo | Stack | Description |
|---|---|---|
| [`onchain`](https://github.com/Pixium-Org/onchain) | Rust / Soroban | Smart contracts |
| [`backend`](https://github.com/Pixium-Org/backend) | Node.js / TypeScript / NestJS | API and WebSocket services |
| [`frontend`](https://github.com/Pixium-Org/frontend) | Next.js / React / Tailwind | Player interface |
| [`indexer`](https://github.com/Pixium-Org/indexer) | Node.js / TypeScript | Stellar event indexer |

---

## Branch Strategy

- `main` — stable, always deployable
- `dev` — integration branch; all PRs target this branch
- Feature branches: `feature/<issue-number>-short-description`

---

## Commit Format

Use [Conventional Commits](https://www.conventionalcommits.org):

```
feat: add faction leaderboard endpoint
fix: correct cooldown calculation in canvas contract
chore: update dependencies
docs: improve indexer setup guide
test: add unit tests for place_pixel
```

---

## Code Style

**Rust (onchain)**
```bash
cargo fmt
cargo clippy -- -D warnings
```

**TypeScript (backend, frontend, indexer)**
```bash
npm run lint
npm run format
```

---

## Pull Request Checklist

Before submitting a PR, make sure:

- [ ] Linked to an issue (`Closes #123`)
- [ ] Branch targets `dev`, not `main`
- [ ] Code is formatted and lints pass
- [ ] Tests added or updated where relevant
- [ ] No breaking changes without prior discussion

---

## Issue Labels

| Label | Description |
|---|---|
| `feat` | New feature |
| `bug` | Something is broken |
| `dev` | Tooling, CI, documentation, refactor |
| `good first issue` | Suitable for new contributors |
| `help wanted` | Extra attention needed |

---

## Code of Conduct

All contributors are expected to follow the [Code of Conduct](./CODE_OF_CONDUCT.md). Be respectful, constructive, and collaborative.
