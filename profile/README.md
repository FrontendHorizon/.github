# Frontend Horizon

We build SEO-grade websites and the systems behind them for service businesses that need leads that close.

This org hosts the apps, products, and shared infrastructure that power FH's customer funnel and the [Elevi](https://github.com/FrontendHorizon/elevi-core) operations platform.

## Reusable workflows

Every repo here can call shared CI from `.github`:

- **`check.yml`** — typecheck + lint + build
- **`security.yml`** — CodeQL, dependency review, secret scanning
- **`audit.yml`** — nightly `npm audit` with auto-issue creation
- **`lighthouse.yml`** — performance audits on push + daily
- **`uptime.yml`** — scheduled URL probes with auto-issue on failure

Reference from a repo's workflow:

```yaml
jobs:
  check:
    uses: FrontendHorizon/.github/.github/workflows/check.yml@main
    with:
      working-directory: site
```

## Issue / PR templates

Bug, feature, and incident templates live in `.github/ISSUE_TEMPLATE/`. PRs use the standard PR template.

## Reporting security issues

See [SECURITY.md](SECURITY.md). Email john@frontendhorizon.com — don't open a public issue.
