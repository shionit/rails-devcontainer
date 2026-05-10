# Security Policy

## Supported Versions

This repository is a DevContainer template for Ruby on Rails development.
Security fixes are applied to the `main` branch only.

| Branch | Supported |
|--------|-----------|
| `main` | ✅ Yes    |
| Others | ❌ No     |

## Reporting a Vulnerability

If you discover a security vulnerability in this repository, please **do not
open a public GitHub issue**.

Instead, report it privately via
[GitHub Private Vulnerability Reporting](https://github.com/shionit/rails-devcontainer/security/advisories/new).

You can expect an acknowledgement within **7 days** and a resolution or
status update within **30 days**.

## Supply Chain Security

This repository applies the following controls to reduce supply chain risk:

- **SHA-pinned GitHub Actions**: all workflow steps reference actions by
  full commit SHA, not mutable version tags.
- **Pinned Docker image digests**: base images in workflows are pinned to
  specific digests.
- **Renovate**: automated PRs keep SHA pins and dependency versions
  current on a weekly schedule.
- **StepSecurity Harden Runner**: outbound network activity from CI jobs
  is monitored (audit mode).
- **Minimal GITHUB_TOKEN permissions**: workflows are scoped to
  `contents: read` by default.
- **CODEOWNERS**: changes to CI pipelines and security configuration
  require explicit owner approval.

## Recommended GitHub Repository Settings

Enable the following features in **Settings → Security** for this repository:

- [ ] Dependabot alerts
- [ ] Dependabot security updates
- [ ] Secret scanning
- [ ] Push protection (prevent secrets from being pushed)
- [ ] Branch protection on `main` (require PR review before merge)
