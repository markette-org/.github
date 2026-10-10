# Security policy

Markette stores credentials for social networks, email providers and payment systems, so we take
security reports seriously.

## Reporting a vulnerability

Please **do not open a public issue**. Use GitHub's private reporting instead: go to the
**Security** tab of the affected repository and choose **Report a vulnerability**. Include what you
found, how to reproduce it, and the impact you expect.

We aim to acknowledge reports within a few days and will keep you informed while we work on a fix.
We credit reporters in the release notes unless you prefer otherwise.

## Supported versions

Security fixes go into the latest release and the `main` branch. Self-hosters should keep their
deployment up to date (`docker compose pull && docker compose up -d`).
