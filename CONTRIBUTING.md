# Contributing

Thank you for helping. This guide applies to every N2JSoft repository that does not have its own
`CONTRIBUTING.md`; when a repository has one, it wins. Everyone taking part follows the
[Code of Conduct](CODE_OF_CONDUCT.md).

## Before you start

- **Bugs**: open an issue with the version you run, your OS and the steps to reproduce.
- **Features and larger changes**: open an issue first, so that we agree on the design before you
  write the code. Small fixes and docs can go straight to a pull request.
- **Vulnerabilities**: never in a public issue. See [SECURITY.md](SECURITY.md).

## Build and check your change

Each repository's README explains how to build and test it; most have a `Makefile`. Run the tests
and linters before you open a pull request: CI runs them on every pull request too. Do not commit
built binaries.

## Pull requests and releases

Our CLIs release automatically from `main` with
[semantic-release](https://semantic-release.gitbook.io/). Pull requests are squash-merged into one
commit named after the pull request, so **the pull request title decides the version**. It must be a
[conventional commit](https://www.conventionalcommits.org/):

| Title | Release |
|---|---|
| `feat!: …`, or `BREAKING CHANGE:` in the body | major |
| `feat: …` | minor |
| `fix: …` and other types | patch |

Do not create version tags by hand. Dependency updates come from Renovate.

A pull request needs green checks and a maintainer's approval before it is merged.
