# Contributing

Thank you for your interest in contributing! This guide will walk you through the process.

## Code of Conduct

Please read our [Code of Conduct](CODE_OF_CONDUCT.md) before contributing.

## Getting Started

### Prerequisites

- [Go](https://golang.org/dl/) (see `go.mod` for version)
- [Git](https://git-scm.com/)

### Fork and Clone

1. **Fork the repository** — Click the "Fork" button on GitHub

2. **Clone your fork**
   ```bash
   git clone https://github.com/YOUR_USERNAME/go-serves.git
   cd go-serves
   ```

3. **Add the upstream remote**
   ```bash
   git remote add upstream https://github.com/ORIGINAL_OWNER/go-serves.git
   ```

## Making Changes

### Create a Branch

Always create a new branch for your changes:

```bash
git checkout -b feature/your-feature-name
```

Use descriptive branch names:
- `feature/add-middleware` — for new features
- `fix/connection-timeout` — for fixing unexpected behavior
- `docs/update-readme` — for documentation

### Make Your Changes

1. Write your code
2. Add or update tests as needed
3. Run tests locally:
   ```bash
   go test ./...
   ```
4. Run linting:
   ```bash
   go vet ./...
   ```

### Commit Your Changes

Write clear, concise commit messages:

```bash
git add .
git commit -m "Add middleware for request logging"
```

Follow these commit message guidelines:
- Use present tense ("Add feature" not "Added feature")
- Keep the first line under 72 characters
- Reference issues when applicable ("Fix #123")

## Submitting a Pull Request

### Sync with Upstream

Before submitting (and before a PR will be merged), sync your fork with the latest changes:

```bash
git fetch upstream
git rebase upstream/main
```

Resolve any conflicts if they arise.

### Push Your Branch

```bash
git push origin feature/your-feature-name
```

### Open a Pull Request

1. Go to your fork on GitHub
2. Click "Compare & pull request"
3. Fill out the [pull request template](PULL_REQUEST_TEMPLATE.md)
4. Click "Create pull request"

### Code Review

- Respond to feedback promptly
- Make requested changes in new commits
- Once approved, a maintainer will merge your PR

## Additional Guidelines

### Testing

- All new features should include tests
- All fixes for unexpected behavior should include a test that reproduces the unexpected behavior
- Aim for meaningful coverage, not 100% coverage

### Documentation

- Update README.md if adding new features
- Add inline comments for complex logic
- Update examples if applicable

## Questions?

Open an issue if you have questions or need help getting started.

---

Thank you for contributing! 🎉
