---
name: booking-com-search-car-rentals
description: Search Booking.com car rental inventory and resolve the depot, supplier and terms behind an offer.
api: Booking.com Demand API
version: '3.2'
base_url: https://demandapi.booking.com/3.2
operations:
  - /cars/search
  - /cars/details
  - /cars/depots
  - /cars/depots/reviews/scores
  - /cars/suppliers
  - /cars/constants
generated: '2026-09-17'
method: generated
source: openapi/booking-com-demand-api-3-2-openapi.yml
---

# Search Booking.com car rentals

## Limits that bite first

- `/cars/search` has its own published limit: **3000 requests per minute**. It is the only
  per-endpoint number Booking.com publishes.
- **Cars are not available in the sandbox.** The whole collection must be exercised against
  production, and `/orders/cancel` for cars returns 403 `sandbox_blocked` in sandbox.

## Steps

1. **`/cars/constants`** — pull the enumerated values (vehicle categories, fuel policies, transmission
   types) once and cache them. They change rarely and re-fetching them burns rate limit.
2. **`/cars/search`** — POST pick-up and drop-off location and times. Returns available vehicles.
3. **`/cars/details`** — resolve a specific offer, its inclusions and its price breakdown.
4. **`/cars/depots`** — resolve the pick-up/drop-off location behind the offer.
5. **`/cars/depots/reviews/scores`** — depot review scores, for surfacing pick-up quality.
6. **`/cars/suppliers`** — the rental company behind the offer.

On the 3.2-Beta track, `/cars/availability` additionally returns an `estimated_commission` object for
eligible partners (a search-time predictive estimate, omitted when no reliable estimate exists) and
insurance details carry a `documents` array. Beta also adds `/cars/terms-and-conditions`.

## Booking a car

Car rentals are booked through the same order flow as accommodation — `/orders/preview` then
`/orders/create`, read back with `/orders/details/cars`. On 3.2-Beta, eligible `pay_at_pickup` car
orders can be created without credit card details.
