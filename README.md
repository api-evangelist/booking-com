# Booking.com

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

Booking.com is the world's largest online travel agency, part of Booking Holdings, listing more than 28 million accommodation options plus car rentals, flights, attractions and airport transfers in over 60,000 destinations. It runs two distinct API programmes. The Demand API serves affiliate partners who want to search, price and book Booking.com inventory inside their own product; the Connectivity platform serves the supply side - channel managers, property management systems and hotel groups keeping rooms, rates, availability, content, reservations and payouts in sync. Twenty OpenAPI descriptions covering 210 operations are published through the developer portal, and the Connectivity estate additionally speaks OpenTravel Alliance (OTA) and Booking.com's own B.XML message formats. Both programmes are credentialed: keys come from the Affiliate Partner Centre or from a machine account in the Connectivity Portal, and no API host answers an anonymous request.

**Areas:** Travel · Hospitality · Accommodation · Booking · Car Rental · Payments · Connectivity · Marketplace · OTA · Attractions · A2A · Hotels

## Booking.com on APIs.io

Everything profiled for Booking.com is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/booking-com/](https://apis.io/providers/booking-com/)** — or go straight to one of the APIs or properties below.

### APIs (49)

- [Booking.com Status API](https://apis.io/apis/booking-com/booking-com-status-api/) — The Status API reports the current operational status of monitored Demand API endpoints, grouped by endpoint group, so partners can detect degradation and…
- [Booking.com Contacts API](https://apis.io/apis/booking-com/booking-com-contacts-api/) — The Connectivity Contacts endpoint manages the contact records attached to a property on Booking.com, letting connectivity providers read and maintain…
- [Booking.com Historical Reservations API](https://apis.io/apis/booking-com/booking-com-historical-reservations-api/) — Retrieve a property's historical reservation details to initialise or reconcile reservation data for revenue management. Room reservations are selected by…
- [Booking.com Property Health API](https://apis.io/apis/booking-com/booking-com-property-health-api/) — A read-only JSON API for connectivity providers that returns property health and status data, explaining why properties are unbookable or at risk so…
- [Booking.com Accommodations API](https://apis.io/apis/booking-com/booking-com-accommodations-api/) — This API collection is specific for the stay part of the connected trip. </br></br>Use these endpoints to search for stays such as hotels and apartments,…
- [Booking.com Attachments API](https://apis.io/apis/booking-com/booking-com-attachments-api/) — Provides endpoints for handling message attachments. </br></br>Use these endpoints to upload and download images shared within conversations.
- [Booking.com Attractions API](https://apis.io/apis/booking-com/booking-com-attractions-api/) — The Attractions API from Booking.com — 5 operation(s) for attractions.
- [Booking.com Bank transfer payout API](https://apis.io/apis/booking-com/booking-com-bank-transfer-payout-api/) — Retrieve Bank Transfer payout details for accommodation reservations.
- [Booking.com Cars API](https://apis.io/apis/booking-com/booking-com-cars-api/) — This API collection is specific to the car rentals part of the connected trip.</br></br> Use these endpoints to search for car rentals, check car details…
- [Booking.com Charges endpoint API](https://apis.io/apis/booking-com/booking-com-charges-endpoint-api/) — Lists the details of the Charges endpoints to set and retrieve taxes and fees at the property and room level.
- [Booking.com Charges meta endpoint API](https://apis.io/apis/booking-com/booking-com-charges-meta-endpoint-api/) — Lists the details of the Charges meta endpoint to retrieve a full list of charge types supported by the Charges API.
- [Booking.com Check legal details API](https://apis.io/apis/booking-com/booking-com-check-legal-details-api/) — Check legal details of Partner using email or entity ID.
- [Booking.com Common/autocomplete API](https://apis.io/apis/booking-com/booking-com-common-autocomplete-api/) — Use this endpoint to retrieve ranked suggestions based on a free-text query. Designed for real-time "as-you-type" autocomplete experiences.
- [Booking.com Common/languages API](https://apis.io/apis/booking-com/booking-com-common-languages-api/) — Provides a list of supported language codes for use in API requests.
- [Booking.com Common/locations API](https://apis.io/apis/booking-com/booking-com-common-locations-api/) — Provides identifiers for a wide range of geographical locations, including airports, countries, cities, and regions. </br></br>Use these identifiers to…
- [Booking.com Common/payments API](https://apis.io/apis/booking-com/booking-com-common-payments-api/) — Provides generic payment-related endpoints, including supported currencies and payment types.
- [Booking.com Conversations API](https://apis.io/apis/booking-com/booking-com-conversations-api/) — Provides endpoints to retrieve and manage messaging conversations. </br></br>Use these endpoints to list conversations, fetch conversation details, and…
- [Booking.com Demand API V2 Compatible API](https://apis.io/apis/booking-com/booking-com-demand-api-v2-compatible-api/) — The demand-api-v2-compatible API from Booking.com — 8 operation(s) for demand-api-v2-compatible.
- [Booking.com Inventory API](https://apis.io/apis/booking-com/booking-com-inventory-api/) — The Inventory API from Booking.com — 1 operation(s) for inventory.
- [Booking.com Manage bathrooms API](https://apis.io/apis/booking-com/booking-com-manage-bathrooms-api/) — Use the GET and the PUT endpoints to: <ul><li>Retrieve room bathroom configuration</li> <li>Add, modify or delete room-level bathroom information</li></ul>
- [Booking.com Manage contracts API](https://apis.io/apis/booking-com/booking-com-manage-contracts-api/) — Create, update or resend contract details.
- [Booking.com Manage property facilities API](https://apis.io/apis/booking-com/booking-com-manage-property-facilities-api/) — Use the GET and the PUT endpoints to: <ul><li>Retrieve property-level facilities details</li> <li>Add, modify or delete property-level facilities…
- [Booking.com Manage room facilities API](https://apis.io/apis/booking-com/booking-com-manage-room-facilities-api/) — Use the GET and the PUT endpoints to: <ul><li>Retrieve room facilities set for a property.</li><li>Add, modify or delete room facilities.</li></ul>
- [Booking.com Messages API](https://apis.io/apis/booking-com/booking-com-messages-api/) — Provides endpoints for two-way post-booking communication between guests and properties. </br></br>Use these endpoints to send and retrieve messages,…
- [Booking.com Meta API](https://apis.io/apis/booking-com/booking-com-meta-api/) — Retrieve units meta data and translations
- [Booking.com Meta data endpoint API](https://apis.io/apis/booking-com/booking-com-meta-data-endpoint-api/) — <p>Retrieve the latest facility definitions.</p> <ul> <li>Get the list of all supported facilities<ul> <li>To get the details of a property-level facility:…
- [Booking.com Orders API](https://apis.io/apis/booking-com/booking-com-orders-api/) — Enables management of booking orders within the Demand API. </br></br>Use these endpoints to preview and create new orders, check order details, cancel or…
- [Booking.com Payments by Booking configurations API](https://apis.io/apis/booking-com/booking-com-payments-by-booking-configurations-api/) — Update Payments by Booking payout configurations for properties.
- [Booking.com Payments by Booking configurations status API](https://apis.io/apis/booking-com/booking-com-payments-by-booking-configurations-status-api/) — Check the processing status of Payments by Booking configuration update requests.
- [Booking.com Payments eligibility details for partners API](https://apis.io/apis/booking-com/booking-com-payments-eligibility-details-for-partners-api/) — Retrieve payments eligibility details for partners.
- [Booking.com Property Description API](https://apis.io/apis/booking-com/booking-com-property-description-api-api/) — Create, update and retrieve property description
- [Booking.com Property Details API](https://apis.io/apis/booking-com/booking-com-property-details-api-api/) — Create, update and retrieve property details
- [Booking.com Property Settings API](https://apis.io/apis/booking-com/booking-com-property-settings-api-api/) — Add, update or retrieve property settings
- [Booking.com Property Status API](https://apis.io/apis/booking-com/booking-com-property-status-api-api/) — Check if a property is ready to open; open or close a property
- [Booking.com Reconciliation reports API](https://apis.io/apis/booking-com/booking-com-reconciliation-reports-api/) — Generate financial reconciliation reports for one or more properties.
- [Booking.com Refundable VCCs API](https://apis.io/apis/booking-com/booking-com-refundable-vccs-api/) — Provides information of the refundable VCCs.
- [Booking.com Report filters API](https://apis.io/apis/booking-com/booking-com-report-filters-api/) — Retrieve the available filter and configuration options for reconciliation report generation.
- [Booking.com Report status API](https://apis.io/apis/booking-com/booking-com-report-status-api/) — Check the processing status of a reconciliation report generation request and retrieve the download URL when the report is ready.
- [Booking.com Reports API](https://apis.io/apis/booking-com/booking-com-reports-api/) — The Reports API from Booking.com — 1 operation(s) for reports.
- [Booking.com Request access API](https://apis.io/apis/booking-com/booking-com-request-access-api/) — Request access to existing partner.
- [Booking.com Reservation breakdown API](https://apis.io/apis/booking-com/booking-com-reservation-breakdown-api/) — Retrieve detailed breakdown for accommodation reservations with respect to partner payout.
- [Booking.com Reservation payout details API](https://apis.io/apis/booking-com/booking-com-reservation-payout-details-api/) — Retrieve detailed partner payout information for accommodation reservations.
- [Booking.com Reservation Status API](https://apis.io/apis/booking-com/booking-com-reservation-status-api-api/) — Provides reservation status information with respect to a reservation ID.
- [Booking.com Rooms API](https://apis.io/apis/booking-com/booking-com-rooms-api-api/) — Create, update, retrieve and delete property units
- [Booking.com Rooms API Bulk API](https://apis.io/apis/booking-com/booking-com-rooms-api-bulk-api/) — Create, update and delete multiple units
- [Booking.com Transfers API](https://apis.io/apis/booking-com/booking-com-transfers-api/) — This collection includes endpoints related to **transfer** services within the connected trip experience.<br/>Use these endpoints to:<br/>- Search for…
- [Booking.com Value Adds API](https://apis.io/apis/booking-com/booking-com-value-adds-api/) — Retrieve catalog of value adds available for properties with dynamic attributes
- [Booking.com VCC payout details, per accommodation reservation API](https://apis.io/apis/booking-com/booking-com-vcc-payout-details-per-accommodation-reservation-api/) — Provides VCC payout details for an accommodation reservation
- [Booking.com VCCs to be charged API](https://apis.io/apis/booking-com/booking-com-vccs-to-be-charged-api/) — Provides information of the VCCs to be charged.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Booking Com Webhooks](https://apis.io/asyncapis/booking-com/booking-com-webhooks/)

#### GraphQL (1)

GraphQL schemas.

- [Moved to /providers/booking-com/](https://apis.io/graphqls/booking-com/booking-com-graphql/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [Booking.com Docs MCP server](https://apis.io/servers/booking-com/booking-com-docs-mcp-server/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Booking Com Agentic Access](https://apis.io/agentic-access/booking-com/booking-com-agentic-access/)

#### JSON Schema (3)

The data models the API reads and writes.

- [Booking.com Accommodation](https://apis.io/schemas/booking-com/booking-com-accommodation/)
- [Booking.com Order](https://apis.io/schemas/booking-com/booking-com-order/)
- [Booking.com Promotion](https://apis.io/schemas/booking-com/booking-com-promotion/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Booking Com Context](https://apis.io/jsonld/booking-com/booking-com-context/)

#### Collections (30)

Postman and Open Collection request collections.

- [Booking.com Car Rentals Accommodations API](https://apis.io/collections/booking-com/open-booking-com-accommodations-api/)
- [Booking.com Car Rentals Accommodations Availability API](https://apis.io/collections/booking-com/open-booking-com-availability-api/)
- [Booking.com Car Rentals API](https://apis.io/collections/booking-com/open-booking-com-car-rentals-api/)
- [Booking.com Car Rentals Accommodations Cars API](https://apis.io/collections/booking-com/open-booking-com-cars-api/)
- [Booking.com Connectivity Content API](https://apis.io/collections/booking-com/open-booking-com-connectivity-content-api/)
- [Booking.com Connectivity Promotions API](https://apis.io/collections/booking-com/open-booking-com-connectivity-promotions-api/)
- [Booking.com Connectivity Rates and Availability API](https://apis.io/collections/booking-com/open-booking-com-connectivity-rates-availability-api/)
- [Booking.com Connectivity Reservations API](https://apis.io/collections/booking-com/open-booking-com-connectivity-reservations-api/)
- [Booking.com Car Rentals Accommodations Constants API](https://apis.io/collections/booking-com/open-booking-com-constants-api/)
- [Booking.com Car Rentals Accommodations Conversations API](https://apis.io/collections/booking-com/open-booking-com-conversations-api/)
- [Booking.com Demand API](https://apis.io/collections/booking-com/open-booking-com-demand-api/)
- [Booking.com Car Rentals Accommodations Depots API](https://apis.io/collections/booking-com/open-booking-com-depots-api/)
- [Booking.com Car Rentals Accommodations Derived Pricing API](https://apis.io/collections/booking-com/open-booking-com-derived-pricing-api/)
- [Booking.com Car Rentals Accommodations Facilities API](https://apis.io/collections/booking-com/open-booking-com-facilities-api/)
- [Booking.com Car Rentals Accommodations Inventory API](https://apis.io/collections/booking-com/open-booking-com-inventory-api/)
- [Booking.com Car Rentals Accommodations Locations API](https://apis.io/collections/booking-com/open-booking-com-locations-api/)
- [Booking.com Car Rentals Accommodations Messages API](https://apis.io/collections/booking-com/open-booking-com-messages-api/)
- [Booking.com Car Rentals Accommodations Orders API](https://apis.io/collections/booking-com/open-booking-com-orders-api/)
- [Booking.com Car Rentals Accommodations OTA Availability API](https://apis.io/collections/booking-com/open-booking-com-ota-availability-api/)
- [Booking.com Car Rentals Accommodations OTA Legacy API](https://apis.io/collections/booking-com/open-booking-com-ota-legacy-api/)
- [Booking.com Car Rentals Accommodations OTA Reservations API](https://apis.io/collections/booking-com/open-booking-com-ota-reservations-api/)
- [Booking.com Car Rentals Accommodations Payments API](https://apis.io/collections/booking-com/open-booking-com-payments-api/)
- [Booking.com Car Rentals Accommodations Photos API](https://apis.io/collections/booking-com/open-booking-com-photos-api/)
- [Booking.com Car Rentals Accommodations Promotions API](https://apis.io/collections/booking-com/open-booking-com-promotions-api/)
- [Booking.com Car Rentals Accommodations Property Management API](https://apis.io/collections/booking-com/open-booking-com-property-management-api/)
- …and 5 more published on APIs.io

#### Overlays (20)

OpenAPI overlays, including conversational phrasing for each operation.

- [Booking Com Charges Api Overlay](https://apis.io/overlays/booking-com/booking-com-charges-api-overlay/)
- [Booking Com Connect Api Overlay](https://apis.io/overlays/booking-com/booking-com-connect-api-overlay/)
- [Booking Com Contacts Api Overlay](https://apis.io/overlays/booking-com/booking-com-contacts-api-overlay/)
- [Booking Com Contracting Api Overlay](https://apis.io/overlays/booking-com/booking-com-contracting-api-overlay/)
- [Booking Com Demand Api 3 1 Overlay](https://apis.io/overlays/booking-com/booking-com-demand-api-3-1-overlay/)
- [Booking Com Demand Api 3 2 Beta Overlay](https://apis.io/overlays/booking-com/booking-com-demand-api-3-2-beta-overlay/)
- [Booking Com Demand Api 3 2 Overlay](https://apis.io/overlays/booking-com/booking-com-demand-api-3-2-overlay/)
- [Booking Com Facilities Api Overlay](https://apis.io/overlays/booking-com/booking-com-facilities-api-overlay/)
- [Booking Com Facilities Api Remote Sync Overlay](https://apis.io/overlays/booking-com/booking-com-facilities-api-remote-sync-overlay/)
- [Booking Com Historical Reservations Api Overlay](https://apis.io/overlays/booking-com/booking-com-historical-reservations-api-overlay/)
- [Booking Com Payments Api Overlay](https://apis.io/overlays/booking-com/booking-com-payments-api-overlay/)
- [Booking Com Payments By Booking Onboarding Api Overlay](https://apis.io/overlays/booking-com/booking-com-payments-by-booking-onboarding-api-overlay/)
- [Booking Com Property Api Overlay](https://apis.io/overlays/booking-com/booking-com-property-api-overlay/)
- [Booking Com Property Health Api Overlay](https://apis.io/overlays/booking-com/booking-com-property-health-api-overlay/)
- [Booking Com Reconciliation Api Overlay](https://apis.io/overlays/booking-com/booking-com-reconciliation-api-overlay/)
- [Booking Com Rooms Api Bulk Overlay](https://apis.io/overlays/booking-com/booking-com-rooms-api-bulk-overlay/)
- [Booking Com Rooms Api Generated Names Overlay](https://apis.io/overlays/booking-com/booking-com-rooms-api-generated-names-overlay/)
- [Booking Com Rooms Api Overlay](https://apis.io/overlays/booking-com/booking-com-rooms-api-overlay/)
- [Booking Com Status Api Overlay](https://apis.io/overlays/booking-com/booking-com-status-api-overlay/)
- [Booking Com Valueadds Api Overlay](https://apis.io/overlays/booking-com/booking-com-valueadds-api-overlay/)

#### Governance rules (1)

Spectral rulesets for the provider's contracts.

- [Booking.com — jsonschema rules](https://apis.io/rules/booking-com/booking-com-jsonschema-spectral-rules/)

#### Security (4)

Authentication, trust centre, and vulnerability disclosure.

- [Booking Com Authentication](https://apis.io/security/booking-com/booking-com-authentication/)
- [Booking Com Domain Security](https://apis.io/security/booking-com/booking-com-domain-security/)
- [Booking Com Trust Center](https://apis.io/security/booking-com/booking-com-trust-center/)
- [Booking Com Vulnerability Disclosure](https://apis.io/security/booking-com/booking-com-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Booking Com Plans Pricing](https://apis.io/plans/booking-com/booking-com-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Booking Com Rate Limits](https://apis.io/rate-limits/booking-com/booking-com-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Booking Com Finops](https://apis.io/finops/booking-com/booking-com-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.booking.com)
- [Documentation](https://developers.booking.com/demand/docs/getting-started/overview)
- [Getting started](https://developers.booking.com/demand/docs/getting-started/overview)
- [API reference](https://developers.booking.com/demand/docs/open-api/3.2/demand-api)
- [Sign up](https://www.booking.com/affiliate-program/v2/index.html)
- [Support](https://connectivity.booking.com/s/article/Contact-Us)
- [Blog](https://news.booking.com/feed/)
- [Terms of service](https://www.booking.com/content/terms.html)
- [Privacy policy](https://www.booking.com/content/privacy.html)
- [GitHub](https://github.com/bookingcom)
- [Status](https://developers.booking.com/demand/docs/additional-services/status-api/about)

## API Evangelist rating

**Kin Score 64.8** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 80.0 |
| Contract quality | 64.5 |
| Contract governance | 14.4 |
| Operational transparency | 92.1 |
| Developer ergonomics | 63.7 |
| Access clarity | 50.0 |

**Agent readiness 43.6** — agent-ready (gated down from agent-native)

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | verified |
| MCP Server | documented (partial credit) |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | verified |
| Rate Limit Signal | verified |
| Event Surface Described | yes |
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
| Operation Distinctiveness | — |

**Regulatory alignment 37.5** — Payments

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/booking-com/](https://apis.io/providers/booking-com/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Booking.com: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/booking-com/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
