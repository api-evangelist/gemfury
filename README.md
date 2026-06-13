# Gemfury

Gemfury is a private package repository service with a REST API for pushing and managing gems, npm, pip, composer, and other language packages for teams and organizations. It supports a wide range of package ecosystems including Gem, npm, PyPI, Go Modules, Composer, Maven, DEB, RPM, Bower, NuGet, and Rust Crates.

## Links

- **Website:** https://gemfury.com
- **Developer Documentation:** https://gemfury.com/help/
- **API Reference:** https://gemfury.com/guide/api/
- **API Quickstart:** https://gemfury.com/guide/api/quickstart/
- **CLI Documentation:** https://gemfury.com/guide/cli/
- **Pricing:** https://fury.co/pricing/
- **Status Page:** https://status.fury.co/
- **Blog / Changelog:** https://fury.blog/changelog
- **GitHub Org:** https://github.com/gemfury
- **X (Twitter):** https://x.com/Gemfury

## API

The Gemfury Developer API is a REST API over HTTPS with JSON payloads. Base URL: `https://api.fury.io`. The current API version is 1, specified via `/1/` path prefix or `X-Fury-Api-Version: 1` header.

Authentication uses Bearer tokens: `Authorization: Bearer YOUR_API_TOKEN`. Tokens are managed at `https://manage.fury.io`.

Resources covered by the API:
- Packages
- Versions
- Accounts
- Members
- Tokens

## Plans

See [plans/gemfury-plans-pricing.yml](plans/gemfury-plans-pricing.yml) for full pricing details.

| Plan | Collaborators | Private Packages | Price/mo |
|------|---------------|------------------|----------|
| Public | Unlimited | 0 | Free |
| Personal 1C | 1 | Unlimited | $9 |
| Personal 5C | 5 | Unlimited | $14 |
| Personal 10C | 10 | Unlimited | $23 |
| Personal 25C | 25 | Unlimited | $50 |
| Personal 50C | 50 | Unlimited | $100 |
| Team 10P | Unlimited | 10 | $25 |
| Team 20P | Unlimited | 20 | $50 |
| Team 50P | Unlimited | 50 | $100 |
| Team 125P | Unlimited | 125 | $200 |
| Team 200P | Unlimited | 200 | $300 |
| Team 300P | Unlimited | 300 | $450 |
| Team 450P | Unlimited | 450 | $650 |
| Enterprise | Custom | Custom | Custom |

## Rate Limits

See [rate-limits/gemfury-rate-limits.yml](rate-limits/gemfury-rate-limits.yml). Specific thresholds are not publicly documented. Implement exponential backoff when receiving 429 responses.

## FinOps

See [finops/gemfury-finops.yml](finops/gemfury-finops.yml) for cost optimization and governance guidance.

## APIs.json

This repository is indexed via [apis.yml](apis.yml) following the APIs.json 0.19 specification.
