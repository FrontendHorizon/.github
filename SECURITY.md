# Security policy

If you find a vulnerability in any Frontend Horizon repository, **don't open a public issue**. Email **john@frontendhorizon.com** instead.

We'll acknowledge within 48 hours and aim to ship a fix or mitigation within 14 days for high-severity findings. Lower-severity stuff lands on a normal cadence.

## Scope

- Apps and services in `github.com/FrontendHorizon/*`
- The infrastructure they run on (Coolify, Supabase, Stripe, Twilio, Resend integrations)
- Customer data flowing through any of the above

## Out of scope

- Findings on third-party SaaS we use (report to the vendor — Supabase, Stripe, etc.)
- Issues that require physical access to a customer's device or account
- Best-practice notes that don't translate to a real attack path

## What helps

- A clear repro on the latest deployed version
- Evidence the vulnerability is exploitable, not theoretical
- Suggested fix or mitigation if you've thought about it
