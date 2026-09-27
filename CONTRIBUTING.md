# Contributing

Thank you for taking the time to contribute to an open source project.

Before contributing, please read the [Code of Conduct](https://github.com/demartini/.github/blob/main/CODE_OF_CONDUCT.md). By participating, you agree to follow it.

## Before you start

Before opening an issue or pull request:

1. Search existing issues and pull requests to avoid duplicates.
2. Check the project's documentation and contribution guidelines.
3. For significant changes, open or comment on an issue first to discuss the proposed approach.

## Reporting bugs

Use the **Bug Report** issue template for reproducible problems.

A useful bug report should include:

- A clear description of the problem.
- The expected behavior.
- The actual behavior.
- Steps to reproduce the problem.
- Relevant environment and version information.
- Logs, screenshots, or other supporting information when useful.

## Suggesting features

Use the **Feature Request** issue template for proposed improvements or new functionality.

Describe:

- The problem or use case.
- The proposed solution.
- Alternatives you considered.
- Any relevant context, examples, or screenshots.

Feature requests are subject to the project's scope, technical constraints, and maintainer review.

## Pull requests

Keep pull requests focused on a single purpose and avoid unrelated changes.

Before starting significant work, discuss the change with the maintainers unless the project explicitly says otherwise.

A typical workflow is:

1. Fork the repository.
2. Create a focused branch from the default branch.
3. Make your changes.
4. Run the project's required checks.
5. Commit your changes using the Conventional Commits format.
6. Push your branch to your fork.
7. Open a pull request using the provided template.

### Pull request expectations

A pull request should:

- Clearly explain what changed and why.
- Include tests or other validation when appropriate.
- Update relevant documentation when behavior or public APIs change.
- Avoid unrelated formatting or refactoring.
- Identify breaking changes and include migration guidance when necessary.

## Commit messages

Commit messages follow [Conventional Commits](https://www.conventionalcommits.org/).

The basic format is:

```
<type>(<scope>): <description>
```

The scope is optional.

### Types

| Type | Purpose |
| --- | --- |
| `build` | Changes to the build system or external dependencies. |
| `chore` | Maintenance or repository changes that do not affect application behavior. |
| `ci` | Changes to continuous integration and automation. |
| `docs` | Documentation-only changes. |
| `feat` | A new feature. |
| `fix` | A bug fix. |
| `perf` | A performance improvement. |
| `refactor` | A code change that neither fixes a bug nor adds a feature. |
| `revert` | Reverts a previous commit. |
| `style` | Changes that affect formatting or code style without changing behavior. |
| `test` | Adding or updating tests. |

### Subject

The subject should:

- Use the imperative, present tense.
- Start with a lowercase letter.
- Be concise.
- Not end with a period.

For example:

```
fix(auth): handle expired sessions
```

### Body

Use the body when additional context is useful. Explain the motivation for the change and describe relevant behavior or implementation details.

### Breaking changes

Breaking changes must be clearly identified with `BREAKING CHANGE:` in the footer or with a `!` after the type or scope.

For example:

```
feat(api)!: remove deprecated endpoint
```

or:

```
feat(api): remove deprecated endpoint

BREAKING CHANGE: The deprecated endpoint is no longer available.
```

### Reverts

A revert should use the `revert` type and reference the commit being reverted.

For example:

```
revert: feat(auth): add social login
```

## Code style

Follow the project's existing tooling and conventions. Do not introduce unrelated formatting changes.

When a project has a repository-specific style guide, that guide takes precedence over these general guidelines.

## Questions

If you are unsure whether a change is appropriate, open an issue or discuss it with the project maintainers before investing significant time in implementation.
