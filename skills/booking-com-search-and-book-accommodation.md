---
name: booking-com-search-and-book-accommodation
description: Search Booking.com accommodation inventory, price a stay, preview the order and create the booking, using the Demand API 3.2.
api: Booking.com Demand API
version: '3.2'
base_url: https://demandapi.booking.com/3.2
sandbox_url: https://demandapi-sandbox.booking.com/3.2
operations:
  - /accommodations/search
  - /accommodations/details
  - /accommodations/availability
  - /orders/preview
  - /orders/create
  - /orders/details
generated: '2026-09-17'
method: generated
source: openapi/booking-com-demand-api-3-2-openapi.yml
---

# Search and book a Booking.com stay

Every operation below is a **POST**, reads included. Parameters go in the JSON body, never the query
string — a query string on a Demand API request returns `invalid_request` ("Query string provided but
none expected").

## Before you start

Send both headers on every request:

- `Authorization: Bearer <key>` — the API key generated in the Affiliate Partner Centre.
- `X-Affiliate-Id: <aid>` — the affiliate ID of the API user.

Missing or wrong either one returns **401**. A wrong affiliate ID returns **403**.

Use `https://demandapi-sandbox.booking.com/3.2` with the same credentials while building. Sandbox is
capped at 50 requests per minute and its accommodation IDs (10507360, 12337, 42709, 3427703, 4462291,
5476508, 2098153) return an error or empty results if used against production.

## Steps

1. **Find candidates — `/accommodations/search`.**
   Send a location (`city`, `country`, or `coordinates` with a `radius`), `checkin`, `checkout`,
   `guests` and `currency`, plus a `booker` object with `platform` and `country`. The response is the
   cheapest available product per accommodation. Narrow with distance, price and
   `cancellation_type_filter` rather than pulling the whole set — this is the documented way to stay
   inside the rate limit. Note that the `non_refundable` value of `cancellation_type_filter` is marked
   deprecated in the contract.

2. **Fill in what you need — `/accommodations/details`.**
   Pass the accommodation IDs and an `extras` array naming only the blocks you want: `description`,
   `facilities`, `payment`, `photos`, `policies`, `rooms`. Every extra you do not ask for is payload you
   do not pay for.

3. **Price the stay — `/accommodations/availability`.**
   Returns priced products for the dates, each carrying the cancellation policy schedule. **Read that
   schedule before you book.** Each entry has a `from` (an ISO 8601 date-time, or the literal `now`) and
   the fee that applies from that moment — this is the only place the cancellation window is stated,
   and it is per product, not per property.

4. **Rehearse — `/orders/preview`.**
   Confirm the final price and terms before committing. This is the only dry-run Booking.com offers.

5. **Commit — `/orders/create`.**
   **There is no idempotency key on this endpoint.** If the call times out, do *not* blind-retry: call
   `/orders/details` first to see whether the order exists, or you will create a second booking.
   A `422` means the payment was refused; branch on `errors[].id` — the `payment_refused_*` family is
   catalogued in `errors/booking-com-decline-codes.yml`. `payment_refused_sca_required` means the 3-D
   Secure data was missing, invalid or expired, not necessarily absent.

6. **Confirm — `/orders/details`.**
   Read back the created order. Every error response carries a `request_id`; log it — Booking.com
   support works from it.

## Error handling

Errors arrive as `{ "request_id": "...", "errors": [ { "id": "...", "message": "..." } ] }`.
Branch on `id`, never on `message`. See `errors/booking-com-problem-types.yml`.

On **429**, back off exponentially (1s, 2s, 4s, 8s) with a retry cap; the counter resets after roughly
one minute. No rate-limit headers are returned, so you cannot see your remaining budget — only the 429.
