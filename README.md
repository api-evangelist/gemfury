# Gemfury

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
