---
name: Pull Skimlinks performance and commissions
description: Retrieve a Skimlinks publisher's commissions, aggregated performance and payment status for reporting and reconciliation.
api: openapi/skimbit-reporting-openapi.yml
operations: [searchCommissions, getAggregatedReports, getPaymentStatus, getDeactivatedMerchants]
---

# Pull Skimlinks performance and commissions

Use the Skimlinks Reporting API (`https://reporting.skimapis.com`) to reconcile revenue and analyse performance.

## Authenticate
Mint an `access_token` at `https://authentication.skimapis.com/access_token` (client_credentials) and pass it as the `access_token` query parameter on every call.

## Steps
1. **Raw commissions** — `searchCommissions` (GET `/publisher/{publisher_id}/commission-report`). Use `start_date`/`end_date` (datetime, e.g. `2021-01-01T00:00:00`) for a window, or `updated_since` to catch refunds/cancellations. Filter by `status` (`active`/`cancelled`), `merchant_id`, `custom_id` (your `xcust`). Page with `limit` (max 5000) + `offset` until `pagination.has_next` is false.
2. **Aggregated performance** — `getAggregatedReports` (GET `/publisher/{publisher_id}/reports`). Required: `report_by` (e.g. `date`, `merchant`, `page`), `start_date`, `end_date`. Read `reports[]` and `totals`.
3. **Payment status** — `getPaymentStatus` (GET `/publisher/{publisher_id}/payment-status`) to tie commissions to invoices; filter by `payment_status` (`paid`/`unpaid`).
4. **(Optional) Deactivated merchants** — `getDeactivatedMerchants` to spot programs that went away and cost revenue.

## Rules
- `searchCommissions` is limited to 40/min and 300/hour per API key (and per-IP ceilings). Aggregated reports 40/min, 500/hour. Handle HTTP `429` with back-off.
- Some networks post reversals as separate negative commissions, so sale counts can differ from the Hub; for exact Hub-matching totals use the multi-aggregated link/page report endpoints.
- If you routinely hit rate limits and are a managed publisher, prefer the batch Data Pipe for event-level data.
