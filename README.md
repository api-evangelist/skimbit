# SkimBit

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

SkimBit Ltd, operating as Skimlinks, is a London-founded content-monetization and affiliate-marketing platform (now part of Taboola) that helps publishers and content creators earn commerce revenue from the products and merchants they mention in editorial content. Skimlinks automatically affiliates outbound merchant links, tracks the resulting clicks and commissions across thousands of affiliate networks and merchant programs, and pays publishers a share of the revenue. For developers, Skimlinks exposes a suite of publisher-facing REST APIs — the Merchant API (merchant programs, domains, verticals and offers), the Reporting API (raw commissions, aggregated performance, trending/purchased products, payment status and deactivated merchants) and the Product Key API (product details, pricing, availability and merchant alternatives across a billion+ product offers) — plus the Skimlinks JavaScript on-page monetization script and a batch Data Pipe delivering event-level clicks, impressions, commissions and product-purchase data to cloud storage.

**Areas:** Company · Affiliate Marketing · Content Monetization · Commerce · Publishers · Advertising · Retail · Reporting · Product · E-Commerce

## SkimBit on APIs.io

Everything profiled for SkimBit is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/skimbit/](https://apis.io/providers/skimbit/)** — or go straight to one of the APIs or properties below.

### APIs (8)

- [SkimBit Commissions API](https://apis.io/apis/skimbit/skimbit-commissions-api/) — The Commissions API from SkimBit — 1 operation(s) for commissions.
- [SkimBit Domains API](https://apis.io/apis/skimbit/skimbit-domains-api/) — The Domains API from SkimBit — 1 operation(s) for domains.
- [SkimBit Merchants API](https://apis.io/apis/skimbit/skimbit-merchants-api/) — The Merchants API from SkimBit — 1 operation(s) for merchants.
- [SkimBit Offers API](https://apis.io/apis/skimbit/skimbit-offers-api/) — The Offers API from SkimBit — 1 operation(s) for offers.
- [SkimBit Payments API](https://apis.io/apis/skimbit/skimbit-payments-api/) — The Payments API from SkimBit — 1 operation(s) for payments.
- [SkimBit Products API](https://apis.io/apis/skimbit/skimbit-products-api/) — The Products API from SkimBit — 4 operation(s) for products.
- [SkimBit Reports API](https://apis.io/apis/skimbit/skimbit-reports-api/) — The Reports API from SkimBit — 8 operation(s) for reports.
- [SkimBit Verticals API](https://apis.io/apis/skimbit/skimbit-verticals-api/) — The Verticals API from SkimBit — 2 operation(s) for verticals.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Skimlinks Data Pipe](https://apis.io/asyncapis/skimbit/skimbit-data-pipe-asyncapi/)

#### Event channels (4)

Individual events and webhooks the provider emits.

- [{bucket}/clicks/date={date}/version=0/](https://apis.io/channels/skimbit/bucket-clicks-date-date-version-0/)
- [{bucket}/commissions/snapshot_date={snapshot_date}/version=0/](https://apis.io/channels/skimbit/bucket-commissions-snapshot-date-snapshot-date-version-0/)
- [{bucket}/pages/date={date}/version=0/](https://apis.io/channels/skimbit/bucket-pages-date-date-version-0/)
- [{bucket}/products/snapshot_date={snapshot_date}/version=0/](https://apis.io/channels/skimbit/bucket-products-snapshot-date-snapshot-date-version-0/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [skimlinks](https://apis.io/servers/skimbit/skimlinks/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Skimbit Agentic Access](https://apis.io/agentic-access/skimbit/skimbit-agentic-access/)

#### Collections (8)

Postman and Open Collection request collections.

- [Skimlinks Merchant Commissions API](https://apis.io/collections/skimbit/open-skimbit-commissions-api/)
- [Skimlinks Merchant Commissions Domains API](https://apis.io/collections/skimbit/open-skimbit-domains-api/)
- [Skimlinks Merchant Commissions Merchants API](https://apis.io/collections/skimbit/open-skimbit-merchants-api/)
- [Skimlinks Merchant Commissions Offers API](https://apis.io/collections/skimbit/open-skimbit-offers-api/)
- [Skimlinks Merchant Commissions Payments API](https://apis.io/collections/skimbit/open-skimbit-payments-api/)
- [Skimlinks Merchant Commissions Products API](https://apis.io/collections/skimbit/open-skimbit-products-api/)
- [Skimlinks Merchant Commissions Reports API](https://apis.io/collections/skimbit/open-skimbit-reports-api/)
- [Skimlinks Merchant Commissions Verticals API](https://apis.io/collections/skimbit/open-skimbit-verticals-api/)

#### Overlays (3)

OpenAPI overlays, including conversational phrasing for each operation.

- [Skimbit Merchant Overlay](https://apis.io/overlays/skimbit/skimbit-merchant-overlay/)
- [Skimbit Product Key Overlay](https://apis.io/overlays/skimbit/skimbit-product-key-overlay/)
- [Skimbit Reporting Overlay](https://apis.io/overlays/skimbit/skimbit-reporting-overlay/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Skimbit Authentication](https://apis.io/security/skimbit/skimbit-authentication/)
- [Skimbit Domain Security](https://apis.io/security/skimbit/skimbit-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Skimbit Plans Pricing](https://apis.io/plans/skimbit/skimbit-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Skimbit Rate Limits](https://apis.io/rate-limits/skimbit/skimbit-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://skimlinks.com)
- [Documentation](https://developers.skimlinks.com)
- [API reference](https://developers.skimlinks.com/merchant.html)
- [Sign up](https://signup.skimlinks.com/)
- [Support](https://support.skimlinks.com/hc/en-us)
- [Blog](https://www.skimlinks.com/insights/)
- [Terms of service](https://www.skimlinks.com/terms-of-service/)
- [Privacy policy](https://www.skimlinks.com/privacy-policy/)

## API Evangelist rating

**Kin Score 44.3** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 78.6 |
| Contract quality | 55.2 |
| Contract governance | 4.5 |
| Operational transparency | 39.5 |
| Developer ergonomics | 47.0 |
| Access clarity | 34.2 |

**Agent readiness 25.7** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | partial |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | derived (partial credit) |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | distinct |

**Regulatory alignment 24.5** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/skimbit/](https://apis.io/providers/skimbit/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for SkimBit: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/skimbit/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
