# CLAUDE.md

This file provides guidance to Claude (and other AI assistants) when working with this repository.

## Repository Overview

This is a new repository for **cynthiacampos/cynthiacampos**. As the project evolves, update this file to reflect the actual stack, structure, and conventions in use.

## Project Structure

_To be updated once source files are added. Document top-level directories and their purpose here._

```
cynthiacampos/
├── CLAUDE.md          # This file
└── ...                # Add project files and update this tree
```

## Tech Stack

_Document the languages, frameworks, and major dependencies once they are chosen._

- **Language:** TBD
- **Framework:** TBD
- **Package manager:** TBD
- **Database:** TBD

## Development Setup

_Update these steps once the project is initialized._

### Prerequisites

List required tools and versions here (e.g., Node.js >= 20, Python >= 3.11, Go >= 1.22).

### Installation

```bash
# Clone the repo
git clone <repo-url>
cd cynthiacampos

# Install dependencies (update command for your stack)
# npm install     # Node.js
# pip install -e . # Python
# go mod download  # Go
```

### Environment Variables

Copy `.env.example` to `.env` and fill in values (create `.env.example` once secrets are identified):

```bash
cp .env.example .env
```

## Common Commands

_Update these once the project is set up._

| Task | Command |
|------|---------|
| Install deps | `TBD` |
| Run dev server | `TBD` |
| Run tests | `TBD` |
| Lint code | `TBD` |
| Format code | `TBD` |
| Build | `TBD` |

## Git Workflow

- **Main branch:** `main` (or `master`)
- **Feature branches:** `<username>/<short-description>`
- **Claude branches:** `claude/<description>-<session-id>`

### Commit Style

Use clear, imperative commit messages:

```
Add user authentication middleware
Fix off-by-one error in pagination logic
Update README with setup instructions
```

Avoid vague messages like "fix bug" or "update stuff".

### Pull Requests

- Keep PRs focused and small when possible
- Include a description of what changed and why
- Reference any related issues

## Code Conventions

_Update this section to match the conventions adopted by the project._

### General

- Prefer clarity over cleverness
- Keep functions small and single-purpose
- Avoid unnecessary abstractions — add them when patterns repeat 3+ times
- Do not add dead code, unused imports, or commented-out blocks

### Error Handling

- Handle errors explicitly; do not silently swallow them
- Validate inputs at system boundaries (user input, external APIs), not internally

### Testing

- Write tests for new functionality and bug fixes
- Tests should cover the happy path and key edge cases
- Keep test setup minimal and focused

### Security

- Never commit secrets, credentials, or API keys — use environment variables
- Validate and sanitize all external input
- Follow OWASP top 10 guidelines when building web-facing features

## AI Assistant Guidelines

When working in this repository, AI assistants (including Claude) should:

### Do

- Read existing code before proposing changes
- Make the minimum change necessary to accomplish the task
- Follow the conventions already established in the codebase
- Run tests (when available) after making changes
- Commit work with descriptive messages
- Update this CLAUDE.md if the project structure or conventions change significantly

### Do Not

- Add unnecessary abstractions, helpers, or utilities for one-off operations
- Add docstrings, comments, or type annotations to code that wasn't changed
- Introduce backwards-compatibility shims for internal code
- Over-engineer solutions — simplest working approach is preferred
- Push to branches other than the designated development branch without permission
- Make risky or destructive git operations (force push, hard reset) without explicit user approval

### Working with This Repository

1. **Check the current branch** before making changes
2. **Read relevant files** before editing them
3. **Run tests** if a test suite exists and commands are documented above
4. **Commit incrementally** with clear messages as tasks are completed
5. **Push** to the designated feature branch when work is done

## CI/CD

_Document the CI/CD pipeline once it is set up (e.g., GitHub Actions workflows, linting gates, deployment targets)._

## Deployment

_Document deployment process and environments once they are established._

---

_Last updated: 2026-02-26. Keep this file current as the project grows._
