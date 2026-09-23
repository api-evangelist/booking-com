---
name: booking-com-reconcile-connectivity-payouts
description: Retrieve payout, VCC and reconciliation data for Booking.com Connectivity properties, and stay current through the notification service.
api: Booking.com Payments API / Reconciliation API
base_url: https://payments-api.booking.com
operations:
  - getPayoutDetails
  - getPriceBreakdown
  - getBTDetails
  - getVCCDetailsPerReservation
  - getVCCtoChargeForProperty
  - getVCCRefundablesForProperty
  - getReservationStatusResponse
  - generateReconReport
  - getReconReportStatus
  - getReconReportFilters
generated: '2026-09-17'
method: generated
source: openapi/booking-com-payments-api-openapi.yml, openapi/booking-com-reconciliation-api-openapi.yml
---

# Reconcile Booking.com Connectivity payouts

This is the **supply** side. Authentication is a JWT minted hourly from a machine account created in the
Connectivity Portal — not the Demand API bearer-token-plus-affiliate-ID pair. The credential-based
scheme these APIs used to accept was sunset on 31 December 2025.

## Per-reservation

- `getPayoutDetails` — `GET /connectivity-payments/reservations/{reservation-id}` — total payout,
  commission and charges.
- `getPriceBreakdown` — `GET /connectivity-payments/reservations/{reservation-id}/breakdown`.
- `getBTDetails` — `GET .../payout/bt` — bank transfer payout details.
- `getVCCDetailsPerReservation` — `GET .../payout/vcc` — virtual credit card payout details.
- `getReservationStatusResponse` — `GET .../status`.

## Per-property

- `getVCCtoChargeForProperty` — `GET /connectivity-payments/properties/{property-id}/chargeable-vccs`.
- `getVCCRefundablesForProperty` — `GET .../refundable-vccs`.

## Reports (asynchronous)

1. `getReconReportFilters` — `GET /connectivity-payments/recon-reports/filters` — discover the valid
   filters and configuration options first; do not guess them.
2. `generateReconReport` — `POST /connectivity-payments/recon-reports` — request a payout report for a
   date range and property set. Returns a request id.
3. `getReconReportStatus` — `GET /connectivity-payments/recon-reports/{request-id}` — poll until the
   report is ready.

The Reconciliation API is the only Booking.com contract that declares a rate-limit signal: a **429**
with a `Retry-After` header carrying an integer number of seconds. Honour it.

## Do not poll blindly

Subscribe to the Connectivity Notifications Service instead. `PAYOUT_UPDATE`, `PAYOUT_METHOD_UPDATE`,
`VIRTUAL_CREDIT_CARD_UPDATE`, `BANK_TRANSFER_UPDATE`, `VCC_BALANCE` and `VCC_FEES_PAYOUT` are pushed on
a Reservations connection and carry the property and reservation identifiers to re-query. See
`asyncapi/booking-com-webhooks.yml`. Note that no signature verification is documented for inbound
notifications — treat the payload as a trigger to re-query, never as the source of truth.
