# Contributing to This Project

First off, thank you for considering contributing! We welcome issues, bugfixes, improvements, and new features. This document outlines the standards and process we follow to keep the codebase clean, stable, and maintainable.

---

## Branching and Commit Standards

- Branch names must be descriptive and start with either `fix/` or `feature/`.
  - Example: `fix/login-redirect`, `feature/signup-form`
  - Follow the [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) standard for determining branch prefixes

- Commits must follow the [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) specification:

- Squash your commits into one logical unit before submitting a pull request.

---

## Pull Request Guidelines

Before opening a pull request:

1. Make sure your branch is targeting `main`
2. Your PR title must be descriptive and **must not include emojis**.
3. Your PR title must follow the [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) specification:

  ```plaintext
  <type>[optional scope]: <description>

  [optional body]

  [optional footer(s)]
  ```

  Examples:
      - `fix(auth)!: correct OAuth2 redirect`
      - `feat(cli): add generate-config subcommand`

4. Your PR description must explain:
   - **What** you changed.
   - **Why** you made the change.
   - Which issue it closes (use `closes #xxxx` syntax).
5. Make sure all checks pass:
   - `npm run build` (for docs-related changes)
   - `go build ./...` and `golangci-lint run` (for Go code)
   - All unit tests pass.
   - Unit test coverage **does not decrease**.

---

## Contact

If you’re unsure about anything, feel free to file an issue.

Thanks for helping improve this project!
