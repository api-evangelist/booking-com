---
name: booking-com-cancel-or-modify-order
description: Reverse or change an existing Booking.com order, reading the cancellation fee schedule first so the cost of the reversal is known before it is taken.
api: Booking.com Demand API
version: '3.2'
base_url: https://demandapi.booking.com/3.2
operations:
  - /orders/details
  - /orders/details/accommodations
  - /orders/details/cars
  - /orders/modify
  - /orders/cancel
generated: '2026-09-17'
method: generated
source: openapi/booking-com-demand-api-3-2-openapi.yml
---

# Cancel or modify a Booking.com order

## Read before you act

Call `/orders/details` (or `/orders/details/accommodations`, `/orders/details/cars`) and read the
cancellation policy schedule on the travel service. Each entry carries `from` — an ISO 8601 date-time,
or the literal `now` — and the fee that applies from that moment. Comparing the current time against
that schedule tells you what the cancellation will cost *before* you make it. Do not assume free
cancellation because the search result said `free_cancellation`; the deadline is in the schedule.

## Cancel — `/orders/cancel`

- POST with the reservation or insurance policy you want to cancel.
- **One travel service per request.** Cancelling three services takes three calls.
- A **200** means the request was accepted. Accommodation cancellations complete immediately; car
  rental and car insurance cancellations continue **asynchronously** after the 200 — re-read
  `/orders/details/cars` to confirm, do not treat the 200 as final for cars.
- A **409** means the service is not eligible in its current state — already cancelled, or no longer
  cancellable. This is terminal for that service; retrying will not change it.
- A **403** with `sandbox_blocked` means you called the car path in sandbox. Use production.

## Modify — `/orders/modify`

Use `/orders/modify` to change an existing order. On the 3.2-Beta track, `/orders/modify/preview`
prices the change first; on 3.2 there is no preview for modifications, so read the fee schedule
yourself before committing.

## The retry trap

None of these operations accepts an idempotency key. If a cancel or modify times out, re-read
`/orders/details` to establish the true state before sending anything again.
