# Geomacro Testnet Dashboard

Public, read-only operational dashboard for the Geomacro wallet-first Developer API Testnet program.

## Purpose

The dashboard presents redacted aggregate evidence from the canonical Geomacro backend. It is designed for testers, partners, grant reviewers and technical stakeholders who want to see how the Testnet program is performing without exposing tester identity or privileged operational data.

The live data source is:

`https://blocknine0.github.io/geomacro-testnet-dashboard/`

The frontend supports rolling 7-day, 30-day and 90-day windows.

## What it shows

- verified and active tester counts
- Testnet API request volume, success/failure and average latency
- credits consumed and capability coverage
- signed Risk Object and Risk Gate delivery counts
- direct pay-per-call Testnet USDC settlement by supported chain
- idempotent replay evidence
- reconciliation and execution-boundary counters
- privacy-safe recent API and payment activity

## Permanent privacy boundaries

The public feed and dashboard do **not** expose tester identity, wallet addresses, transaction hashes, request IDs, subject/query text, raw API credentials, raw request bodies, or upstream news-source identity.

Testnet payments are technical proof only and are always classified as non-revenue. `execution_authorized` remains false.

## Deployment

This repository is intentionally static and can be hosted with GitHub Pages. Set Pages to deploy from the `main` branch root.

No GitHub Actions secrets, Supabase service role, wallet key or private API credential belongs in this repository.

## Canonical sources

- Product/backend: `blocknine0/geomacro`
- Testnet access: `https://geomacro.live/testnet-access`
- Public dashboard feed: `https://geomacro.live/api/testnet/dashboard`

