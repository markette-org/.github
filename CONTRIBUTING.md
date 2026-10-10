# Contributing to Markette

Thank you for helping. Markette is built in the open and every kind of contribution counts:
bug reports, fixes, new network integrations, documentation, translations and design.

## Where things live

| Change | Repository |
|---|---|
| API, scheduling, providers, metrics, MCP server | [markette-server](https://github.com/markette-org/markette-server) |
| Web interface | [markette-web](https://github.com/markette-org/markette-web) |
| Android and iOS apps | [markette-mobile](https://github.com/markette-org/markette-mobile) |
| Docker setup, documentation for operators | [markette-deploy](https://github.com/markette-org/markette-deploy) |

Not sure? Open an issue in markette-deploy and we'll move it.

## Before you start

- For anything bigger than a small fix, open an issue first to agree on the approach.
- New network integrations: check the platform's **current** API terms and limits, and write them
  down in the provider's docstring. Never automate around a platform's rules: scraping, private
  APIs, or anything that breaks a site's terms will not be merged.
- Personal data deserves care. Ask for the minimum, encrypt credentials, and never log tokens.

## Pull requests

- Keep each PR focused. Explain the *why* in its description.
- Add or update tests. Server PRs must pass `ruff`, `pytest` and the OpenAPI validation. Web PRs
  must build without warnings.
- Match the style of the surrounding code; formatters and linters are configured in each repository.
- By contributing you agree that your work is licensed under the
  [AGPL-3.0](https://www.gnu.org/licenses/agpl-3.0.html), like the rest of Markette.

## Getting help

Use GitHub Discussions or issues. Be patient and kind: Markette is maintained by volunteers.
