# booking-com (booking-com)

Seamlessly incorporate Booking.com inventory into your travel application.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/apis.yml)

## Timestamps

- **Modified:** 2026-05-19

## APIs

### Booking.com Demand API

The Booking.com Demand API is a RESTful API that enables Affiliate Partners to access Booking.com's extensive travel inventory. It provides endpoints for searching accommodations such as hotels and apartments, checking availability, retrieving reviews, and getting detailed property information. The API uses JSON responses and requires HTTPS POST requests with Affiliate ID and token authentication.

- **Human URL:** [https://developers.booking.com/demand/docs/getting-started/overview](https://developers.booking.com/demand/docs/getting-started/overview)
- **Base URL:** `https://demandapi.booking.com`

#### Tags

- Accommodations
- Affiliates
- Booking
- Hotels
- Search
- Travel

#### Properties

- [Documentation](https://developers.booking.com/demand/docs/getting-started/overview)
- [OpenAPI](openapi/booking-com-demand-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/booking-com-demand-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/booking-com-demand-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Booking.com Car Rentals API

The Booking.com Car Rentals API is part of the Demand API and provides endpoints specific to the car rental segment of the connected trip experience. Developers can use it to search for available car rentals, retrieve car details, and look up depots and suppliers. The API enables affiliate partners to integrate Booking.com's car rental inventory into their own platforms, offering users the ability to find and book vehicles as part of their travel planning workflow.

- **Human URL:** [https://developers.booking.com/demand/docs/open-api/demand-api/cars](https://developers.booking.com/demand/docs/open-api/demand-api/cars)
- **Base URL:** `https://demandapi.booking.com`

#### Tags

- Car Rentals
- Transportation
- Travel
- Vehicles

#### Properties

- [Documentation](https://developers.booking.com/demand/docs/open-api/demand-api/cars)
- [OpenAPI](openapi/booking-com-car-rentals-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/booking-com-car-rentals-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/booking-com-car-rentals-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Booking.com Connectivity Content API

The Booking.com Connectivity Content API enables Connectivity Partners to register properties and modify their content directly without using the Booking.com extranet. Partners can manage facilities, rates, rooms, photos, and other property details programmatically. This API is designed for property management systems, channel managers, and other connectivity solutions that need to create and maintain property listings on Booking.com at scale.

- **Human URL:** [https://developers.booking.com/connectivity/docs/content](https://developers.booking.com/connectivity/docs/content)
- **Base URL:** `https://supply-xml.booking.com`

#### Tags

- Connectivity
- Content Management
- Hotels
- Properties

#### Properties

- [Documentation](https://developers.booking.com/connectivity/docs/content)
- [OpenAPI](openapi/booking-com-connectivity-content-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/booking-com-connectivity-content-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/booking-com-connectivity-content-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Booking.com Connectivity Reservations API

The Booking.com Connectivity Reservations API allows Connectivity Partners to retrieve and update reservation information for properties listed on Booking.com. It operates over a PCI-compliant secure endpoint and supports reservation retrieval, confirmation, and modification. This API is essential for property management systems and channel managers that need to synchronize booking data between Booking.com and their own systems in real time.

- **Human URL:** [https://developers.booking.com/connectivity/docs](https://developers.booking.com/connectivity/docs)
- **Base URL:** `https://secure-supply-xml.booking.com`

#### Tags

- Booking
- Connectivity
- Hotels
- Reservations

#### Properties

- [Documentation](https://connect.booking.com/user_guide/site/en-US/res/)
- [OpenAPI](openapi/booking-com-connectivity-reservations-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/booking-com-connectivity-reservations-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/booking-com-connectivity-reservations-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Booking.com Connectivity Rates and Availability API

The Booking.com Connectivity Rates and Availability API allows Connectivity Partners to set room availability, pricing, and restrictions for properties on Booking.com. Partners can manage advance booking windows, length of stay requirements, and rate plans programmatically.

- **Human URL:** [https://developers.booking.com/connectivity/docs/ari](https://developers.booking.com/connectivity/docs/ari)
- **Base URL:** `https://supply-xml.booking.com`

#### Tags

- Availability
- Connectivity
- Inventory
- Pricing
- Rates

#### Properties

- [Documentation](https://developers.booking.com/connectivity/docs/ari)
- [OpenAPI](openapi/booking-com-connectivity-rates-availability-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/booking-com-connectivity-rates-availability-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/booking-com-connectivity-rates-availability-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Booking.com Connectivity Promotions API

The Booking.com Connectivity Promotions API enables Connectivity Partners to create and manage promotional offers for properties listed on Booking.com. Partners can programmatically set up deals, discounts, and special rates to attract travelers and increase bookings.

- **Human URL:** [https://developers.booking.com/connectivity/docs](https://developers.booking.com/connectivity/docs)
- **Base URL:** `https://supply-xml.booking.com`

#### Tags

- Connectivity
- Deals
- Discounts
- Marketing
- Promotions

#### Properties

- [Documentation](https://developers.booking.com/connectivity/docs)
- [OpenAPI](openapi/booking-com-connectivity-promotions-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/booking-com-connectivity-promotions-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/booking-com-connectivity-promotions-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/bookingcom)
- [JSON-LD](json-ld/booking-com-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON Schema](json-schema/booking-com-accommodation-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/booking-com-order-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/booking-com-promotion-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Features](undefined)
- [L L Ms Txt](https://developers.booking.com/llms.txt)
