---
name: Enrich content with Skimlinks Product Key
description: Look up product details, pricing, availability and monetizable merchant alternatives to power commerce content and widgets.
api: openapi/skimbit-product-key-openapi.yml
operations: [getProduct, getMultiProducts, getTrendingProducts]
---

# Enrich content with Skimlinks Product Key

Use the Skimlinks Product Key API (`https://products.skimapis.com`) to fetch product data and affiliated merchant alternatives for commerce content. Product Key is available on request and uses a dedicated Client ID / Client Secret.

## Authenticate
Mint an `access_token` at `https://authentication.skimapis.com/access_token` (client_credentials, Product-Key-specific credentials) and pass it as the `access_token` query parameter. `publisher_domain_id` is required on product calls.

## Steps
1. **Single product** — `getProduct` (GET `/publisher/{publisher_id}/product`). Identify the product by `product_url`, `upc`, or `product_id` (+`product_id_type`). Returns `product_details` plus `product_alternatives[]` (other merchants selling the same item), each with `price`, `is_available`, images and an `urls.affiliated_url` ready to link.
2. **Multiple products** — `getMultiProducts` (POST `/v1/publisher/{publisher_id}/products`) with a JSON body `{product_urls: [...]}` or `{product_ids: [...]}` to resolve many at once. Results are keyed by the input URL.
3. **(Optional) Trending inspiration** — `getTrendingProducts` (GET `/publisher/{publisher_id}/trending-products` on the Reporting API) with `period` = `today`/`7_days`/`30_days` to find products trending across the network you have not yet featured.

## Rules
- `getProduct` default limit 80/min and 5000/hour; `getMultiProducts` 20/min and 1000/hour. Back off on HTTP `429`; ask your account manager to raise limits.
- Use `domains`/`exclude_domains` and `merchant_type=featured` to steer which alternatives are returned.
- Always link via the returned `urls.affiliated_url` so clicks are monetized and attributed.
