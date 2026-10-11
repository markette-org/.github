<h1 align="center">Markette</h1>

<p align="center">
  <b>Open-source publishing for the social web.</b><br>
  Write once, tailor per network, schedule at the right moment, and see what worked.<br>
  Self-hosted, multi-tenant, AGPL-3.0.<br>
  <a href="https://markette.org">markette.org</a> · <a href="https://app.markette.org">app.markette.org</a>
</p>

---

Social media tools decide what you may publish, when, and with which AI, and they change those rules
whenever it suits their business. Markette is a publishing system you run yourself. Your accounts,
content, audience data and choice of AI stay under your control, and the code is open for anyone to
read, audit, improve and fork.

## What it does

- **Publish everywhere from one place.** 22 destinations:
  - **Social:** X, Threads, Bluesky, Mastodon, LinkedIn, Facebook, Instagram, YouTube, Reddit.
  - **Messaging:** Telegram, WhatsApp, WeChat, QQ, Discord, Slack.
  - **Sites and blogs:** WordPress, Drupal, Ghost, Medium, Hugo (git).
  - **Newsletters:** Brevo, Listmonk.
  - **Integrations:** a signed webhook for n8n, Make or your own code.
- **Real scheduling.**
  - Times per channel: exact time, weekly queue slots, or the best time learned from each channel's own engagement.
  - Retries with backoff, and an approval workflow for teams.
- **Measure what worked.** Metrics per post and channel, audience growth, and a best-time heatmap.
- **Built for organizations.** Organizations, workspaces per brand or client, teams with channel access
  and reviewers, SSO with OpenID Connect, plans with Stripe, and a superadmin console.
- **AI on your terms.** Optional help to pick times, plan campaigns and adapt copy, through OpenRouter
  or any OpenAI-compatible endpoint, including a local model. No AI is required.
- **Everywhere you work.**
  - A REST API documented with OpenAPI.
  - An MCP server for AI assistants.
  - Android and iOS apps with "Share with Markette".

## Repositories

| Repository | What it contains |
|---|---|
| [markette-deploy](https://github.com/markette-org/markette-deploy) | **Start here.** docker-compose for self-hosting, configuration and network setup guides |
| [markette-server](https://github.com/markette-org/markette-server) | Django API, Celery scheduler and workers, network providers, MCP server |
| [markette-web](https://github.com/markette-org/markette-web) | Angular web app |
| [markette-mobile](https://github.com/markette-org/markette-mobile) | Android and iOS apps (Capacitor) with the share extension |
| [markette-extension](https://github.com/markette-org/markette-extension) | Chrome extension: share pages, selections, links and images ([download](https://github.com/markette-org/markette-extension/releases/latest)) |

## Quick start

```bash
git clone https://github.com/markette-org/markette-deploy.git && cd markette-deploy
cp .env.example .env && docker compose up -d
```

## Contributing

Bug reports, network integrations, translations and documentation are all welcome. Read
[CONTRIBUTING](https://github.com/markette-org/.github/blob/main/CONTRIBUTING.md) and our
[Code of Conduct](https://github.com/markette-org/.github/blob/main/CODE_OF_CONDUCT.md). Report security
issues privately as described in [SECURITY](https://github.com/markette-org/.github/blob/main/SECURITY.md).

Markette is young software: expect rough edges, and tell us about them.

<sub>Markette is free software, licensed under the GNU Affero General Public License v3.0. Running a
modified version as a service means sharing your changes with its users.</sub>
