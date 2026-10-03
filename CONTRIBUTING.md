# Contributing to Melo and its plugins

Thank you for your interest in contributing to the Melo ecosystem.

Contributions can include bug reports, feature requests, documentation updates, tests, code improvements, new plugins and review feedback. Every contribution helps make Melo more useful, reliable and accessible.

Before contributing, please read this guide and the README of the repository you want to modify.

## Code of conduct

Be respectful and constructive in issues, discussions, code reviews and Pull Requests.

Harassment, discrimination, personal attacks and disruptive behavior are not tolerated. Focus on the technical topic, explain disagreements clearly and assume good intent.

## Legal use

Melo and its plugins are intended for legal and personal use.

Do not contribute features intended to bypass DRM, copy protection, access controls or copyright law. Do not use issues or Pull Requests to share copyrighted music, CD images, keys or other unauthorized material.

## Before opening an issue

Before creating an issue:

1. Search existing issues to avoid duplicates.
2. Make sure the issue belongs to the correct repository.
3. Use the issue template, if one is available.
4. For bugs, include enough information for someone else to reproduce the problem.
5. For feature requests, explain the user need and expected behavior, not only a possible technical solution.

A useful bug report should include:

- Melo and/or plugin version
- Operating system and version
- Rust version, if relevant
- Steps to reproduce the issue
- Expected behavior
- Actual behavior
- Logs, error messages or screenshots when safe to share

Never include passwords, API keys, private music files, personal paths or other sensitive data in an issue.

## Finding a contribution

If you are new to the project, look for issues labelled:

- `good first issue` for small and accessible tasks
- `help wanted` for tasks where contributors are welcome
- `documentation` for documentation improvements
- `bug` for reproducible problems
- `plugin` for plugin-related work

For larger features or architectural changes, open an issue first. This prevents duplicated work and lets maintainers discuss the direction before implementation starts.

## Development workflow

Use the following workflow for code and documentation changes.

1. Fork the repository you want to contribute to.
2. Clone your fork locally.
3. Create a branch from the default branch.
4. Make one focused change.
5. Run the relevant formatting, linting and tests.
6. Commit your work with a clear message.
7. Push your branch to your fork.
8. Open a Pull Request against the original repository.

Example:

```bash
git clone [https://github.com/YOUR-USERNAME/Melo.git](https://github.com/YOUR-USERNAME/Melo.git)
cd Melo

git checkout -b feat/improve-library-search

# Make your changes

git add .
git commit -m "feat: improve library search"
git push origin feat/improve-library-search
```

Use a clear branch name:

```text
feat/add-playlist-import
fix/handle-invalid-metadata
docs/update-installation-guide
test/add-plugin-loading-tests
refactor/simplify-library-service
```

Do not work directly on the `main` branch of your fork.

## Commit conventions

Use short, descriptive commit messages following this format:

```text
type: short description
```

Recommended types:

| Type | Use for |
|---|---|
| `feat` | A new user-visible feature |
| `fix` | A bug fix |
| `docs` | Documentation changes |
| `test` | Adding or updating tests |
| `refactor` | Code restructuring without behavior changes |
| `perf` | Performance improvements |
| `build` | Build system, Cargo or Docker changes |
| `ci` | GitHub Actions or CI changes |
| `chore` | Maintenance work, dependencies or tooling |

Examples:

```text
feat: add audio CD detection
fix: prevent duplicate track imports
docs: clarify Docker setup
test: add metadata parser coverage
ci: run Clippy on pull requests
```

## Rust code standards

For Rust repositories, run these commands before opening a Pull Request:

```bash
cargo fmt --all -- --check
cargo clippy --all-targets --all-features -- -D warnings
cargo test --all-features
```

If formatting is needed, apply it with:

```bash
cargo fmt --all
```

Your Pull Request should compile, pass tests and avoid new Clippy warnings. If a command cannot be run locally, explain why in the Pull Request description.

## Documentation standards

Documentation changes should:

- Use clear and understandable English
- Keep commands tested and copy-pasteable
- Mention platform-specific requirements when necessary
- Avoid claiming that unfinished or experimental features are stable
- Update the README when installation, configuration or behavior changes
- Include examples when they make usage clearer

## Pull Request guidelines

A good Pull Request should:

- Address one problem or one feature at a time
- Reference the related issue when applicable
- Explain what changed and why
- Include tests for changed behavior when practical
- Update relevant documentation
- Pass all automated checks
- Avoid unrelated formatting changes or large generated files

Use this structure in your Pull Request description:

```md
## What changed

Briefly explain the change.

## Why

Explain the issue or need addressed.

## Testing

Describe the commands and manual tests you performed.

## Checklist

- [ ] I tested my changes locally
- [ ] I ran formatting checks
- [ ] I ran Clippy
- [ ] I ran relevant tests
- [ ] I updated documentation when needed
- [ ] I did not include secrets or copyrighted files
```

Maintainers may request changes before merging. This is a normal part of collaboration and code review.

## Creating a Melo plugin

Before creating a plugin, open an issue in the [Melo repository](https://github.com/Melo-and-its-plugins/Melo/issues) to discuss the idea, the target use case and the required integration points.

A plugin repository should contain at least:

```text
your-melo-plugin/
├── README.md
├── LICENSE
├── Cargo.toml
├── src/
├── tests/                 # when relevant
└── .github/
    └── workflows/
        └── ci.yml
```

Your plugin README should include:

- The plugin’s purpose
- Installation instructions
- Required Melo version
- Supported operating systems
- Configuration instructions
- Usage examples
- Known limitations
- License information

Do not use undocumented Melo internals as a public plugin API. The plugin API can change before the first stable Melo release, so clearly state the version or commit range your plugin supports.

## Security issues

Do not open a public issue for a potential security vulnerability.

Check the repository’s `SECURITY.md` file for its private reporting process. If no security policy is available, contact a maintainer privately through GitHub.

## License and ownership

By submitting a contribution, you confirm that:

- You have the right to submit the code, documentation or assets.
- Your contribution does not contain proprietary, confidential or copyrighted material that you are not allowed to share.
- Your contribution may be distributed under the license of the repository to which you contribute.

Melo and its official plugins use the **GNU Affero General Public License v3.0 (AGPL-3.0)** unless a repository explicitly states another license.

## Thank you

Thank you for helping build a free, local and extensible music ecosystem.