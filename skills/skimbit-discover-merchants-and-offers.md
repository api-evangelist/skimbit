---
name: Discover Skimlinks merchants and offers
description: Find the merchant programs, monetizable domains, verticals and current offers available to a Skimlinks publisher.
api: openapi/skimbit-merchant-openapi.yml
operations: [listDomains, listVerticals, listMerchants, listOffers]
---

# Discover Skimlinks merchants and offers

Use the Skimlinks Merchant API (`https://merchants.skimapis.com`) to find which merchant programs a publisher can monetize and what offers are live.

## Authenticate
1. Get a `Client ID` and `Client Secret` from the Publisher Hub (Toolbox > APIs > API Authentication credentials).
2. Mint an `access_token`: `POST https://authentication.skimapis.com/access_token` with JSON `{client_id, client_secret, grant_type: "client_credentials"}`. Keep the `access_token`; it expires (see `expiry_timestamp`).
3. Pass `access_token` as a query parameter on every request.

## Steps
1. **List the publisher's domains** — `listDomains` (GET `/v4/publisher/{publisher_id}/domains`). Pick the `publisher_domain_id` you want to query merchants for.
2. **(Optional) List verticals** — `listVerticals` (GET `/v4/verticals`, no auth needed) to get a `vertical` id for filtering.
3. **List / search merchants** — `listMerchants` (GET `/v4/publisher/{publisher_id}/merchants`). Required: `publisher_domain_id`. Filter with `search`, `vertical`, `country`, `a_id`; sort with `sort_by` + `sort_dir`; page with `limit`/`offset`. Rates and stats returned depend on the domain queried.
4. **List offers** — `listOffers` (GET `/v4/publisher/{publisher_id}/offers`) to surface coupons/deals; filter by `merchant_id`, `period` (e.g. `ongoing`), `country`.

## Rules
- Merchant and offer list responses use HTTP `201`; paginate with `has_more` + `offset`.
- Respect the rate limit: 40 requests/min and 1000/hour per API key; back off on HTTP `429`.
- Prefer `advertiser_id` over the deprecated `merchant_id` field.
