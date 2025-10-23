# Contributor Guide


## Branching & Contribution Guidelines

- All contributions should be made in a **feature branch** off of `develop`
- Open a **pull request into `develop`**, not `main`
- The `main` branch is reserved for releases and deploys
- Releases are automatically generated from `develop` using [`release-please`](https://github.com/googleapis/release-please)

## Commit Conventions

We use [Conventional Commits](https://www.conventionalcommits.org/) to ensure consistent history and changelog generation via `release-please`.

Use one of the following prefixes in your commit messages:

- `feat:` — new user-facing feature
- `fix:` — bug fix
- `docs:` — documentation-only change
- `style:` — formatting, whitespace, etc.
- `refactor:` — code change that neither fixes a bug nor adds a feature
- `perf:` — performance improvements
- `test:` — add or fix tests
- `build:` — changes to build tools, dependencies, CI/CD
- `chore:` — other changes that don’t modify app logic

### Examples

```bash
git commit -m "feat: add agency merge strategy"
git commit -m "fix: resolve CLI argument conflict"
git commit -m "docs: clarify Graphviz usage in README"
```
## Optional: Releasing

> Releases are automatically generated from `develop` by `release-please`.

To build locally:

```bash
uv run python -m build
```
