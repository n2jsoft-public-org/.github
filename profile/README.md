<div align="center">

# N2JSoft

**Open-source tools from the engineering team behind [N2F](https://www.n2f.com/), the expense management platform.**

We build them for our own platform and CI, then publish them. They are free to use under open-source licenses.

</div>

## 🔐 Infrastructure access

| Project | What it does |
|---|---|
| [**airlock**](https://github.com/n2jsoft-public-org/airlock) | One access point to private databases, EKS clusters, caches and AWS data, from localhost and as guarded MCP servers for AI assistants. |
| [traefik-maintenance-plugin](https://github.com/n2jsoft-public-org/traefik-maintenance-plugin) | Traefik middleware that restricts access to allowed IPs and redirects everyone else, for maintenance windows or private environments. |

## 🧱 Architecture guardrails for .NET

| Project | What it does |
|---|---|
| [**ModularGuard**](https://github.com/n2jsoft-public-org/ModularGuard) | CLI that enforces module boundaries in modular monolith C# projects by validating project references. |
| [ModularGuard-action](https://github.com/n2jsoft-public-org/ModularGuard-action) | GitHub Action that runs ModularGuard on pull requests, with inline annotations and a summary comment. |
| [slnxsync](https://github.com/n2jsoft-public-org/slnxsync) | Generates filtered `.slnx` solution files from one source solution, for faster CI builds. |

## 🗄️ Database migrations

| Project | What it does |
|---|---|
| [**liquibase-linter**](https://github.com/n2jsoft-public-org/liquibase-linter) | Fast linter for Liquibase changelogs: catches security risks, performance issues and bad practices before they reach production. |
| [liquibase-linter-action](https://github.com/n2jsoft-public-org/liquibase-linter-action) | GitHub Action that runs liquibase-linter and annotates pull requests. |

## 📦 Install

Our CLIs ship for macOS, Linux and Windows:

```sh
brew install --cask n2jsoft-public-org/tap/airlock      # Homebrew
scoop bucket add n2jsoft https://github.com/n2jsoft-public-org/scoop-bucket   # Scoop
```

Each project's README lists every install option.

## 🤝 Contributing

Issues and pull requests are welcome. Read the [contributing guide](https://github.com/n2jsoft-public-org/.github/blob/main/CONTRIBUTING.md) first, and report vulnerabilities privately as described in our [security policy](https://github.com/n2jsoft-public-org/.github/blob/main/SECURITY.md).
