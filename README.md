# Booking.com (booking-com)
Booking.com is a leading online travel platform that connects travelers with accommodations, car rentals, and other travel services worldwide. Their developer platform offers Demand APIs for affiliate partners to search and book travel inventory, as well as Connectivity APIs for property management systems and channel managers to manage listings, rates, availability, reservations, and promotions at scale.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/apis.yml)

## Scope

- **Type:** Contract
- **Position:** Consuming
- **Access:** 3rd-Party

## Tags:

 - Travel, Hotels, Accommodations, Car Rentals, Booking, Connectivity

## Timestamps

- **Created:** 2026-03-20
- **Modified:** 2026-03-20

## APIs

### Booking.com Demand API
The Booking.com Demand API is a RESTful API that enables Affiliate Partners to access Booking.com's extensive travel inventory. It provides endpoints for searching accommodations such as hotels and apartments, checking availability, retrieving reviews, and getting detailed property information. The API uses JSON responses and requires HTTPS POST requests with Affiliate ID and token authentication. The latest version (V3.1) offers improved functionality and additional endpoints for building travel booking experiences.

**Human URL:** [https://developers.booking.com/demand/docs/getting-started/overview](https://developers.booking.com/demand/docs/getting-started/overview)


#### Tags:

 - Travel, Hotels, Accommodations, Search, Booking, Affiliates

#### Properties

- [Documentation](https://developers.booking.com/demand/docs/getting-started/overview)
- [OpenAPI](openapi/booking-com-demand-api-openapi.yml)

### Booking.com Car Rentals API
The Booking.com Car Rentals API is part of the Demand API and provides endpoints specific to the car rental segment of the connected trip experience. Developers can use it to search for available car rentals, retrieve car details, and look up depots and suppliers. The API enables affiliate partners to integrate Booking.com's car rental inventory into their own platforms, offering users the ability to find and book vehicles as part of their travel planning workflow.

**Human URL:** [https://developers.booking.com/demand/docs/open-api/demand-api/cars](https://developers.booking.com/demand/docs/open-api/demand-api/cars)


#### Tags:

 - Car Rentals, Travel, Transportation, Vehicles

#### Properties

- [Documentation](https://developers.booking.com/demand/docs/open-api/demand-api/cars)
- [OpenAPI](openapi/booking-com-car-rentals-api-openapi.yml)

### Booking.com Connectivity Content API
The Booking.com Connectivity Content API enables Connectivity Partners to register properties and modify their content directly without using the Booking.com extranet. Partners can manage facilities, rates, rooms, photos, and other property details programmatically. This API is designed for property management systems, channel managers, and other connectivity solutions that need to create and maintain property listings on Booking.com at scale.

**Human URL:** [https://developers.booking.com/connectivity/docs/content](https://developers.booking.com/connectivity/docs/content)


#### Tags:

 - Properties, Hotels, Content Management, Connectivity

#### Properties

- [Documentation](https://developers.booking.com/connectivity/docs/content)
- [OpenAPI](openapi/booking-com-connectivity-content-api-openapi.yml)

### Booking.com Connectivity Reservations API
The Booking.com Connectivity Reservations API allows Connectivity Partners to retrieve and update reservation information for properties listed on Booking.com. It operates over a PCI-compliant secure endpoint and supports reservation retrieval, confirmation, and modification. This API is essential for property management systems and channel managers that need to synchronize booking data between Booking.com and their own systems in real time.

**Human URL:** [https://developers.booking.com/connectivity/docs](https://developers.booking.com/connectivity/docs)


#### Tags:

 - Reservations, Hotels, Booking, Connectivity

#### Properties

- [Documentation](https://connect.booking.com/user_guide/site/en-US/res/)
- [OpenAPI](openapi/booking-com-connectivity-reservations-api-openapi.yml)

### Booking.com Connectivity Rates and Availability API
The Booking.com Connectivity Rates and Availability API allows Connectivity Partners to set room availability, pricing, and restrictions for properties on Booking.com. Partners can manage advance booking windows, length of stay requirements, and rate plans programmatically. This API is a core component of the Connectivity suite, enabling channel managers and property management systems to keep inventory and pricing synchronized between their platforms and Booking.com without manual extranet updates.

**Human URL:** [https://developers.booking.com/connectivity/docs/ari](https://developers.booking.com/connectivity/docs/ari)


#### Tags:

 - Rates, Availability, Pricing, Inventory, Connectivity

#### Properties

- [Documentation](https://developers.booking.com/connectivity/docs/ari)
- [OpenAPI](openapi/booking-com-connectivity-rates-availability-api-openapi.yml)

### Booking.com Connectivity Promotions API
The Booking.com Connectivity Promotions API enables Connectivity Partners to create and manage promotional offers for properties listed on Booking.com. Partners can programmatically set up deals, discounts, and special rates to attract travelers and increase bookings. This API integrates with the broader Connectivity suite, allowing property management systems and channel managers to coordinate promotional campaigns across distribution channels without requiring manual configuration through the Booking.com extranet.

**Human URL:** [https://developers.booking.com/connectivity/docs](https://developers.booking.com/connectivity/docs)


#### Tags:

 - Promotions, Deals, Discounts, Marketing, Connectivity

#### Properties

- [Documentation](https://developers.booking.com/connectivity/docs)
- [OpenAPI](openapi/booking-com-connectivity-promotions-api-openapi.yml)

## Common Properties

- [Developer Portal](https://developers.booking.com/)
- [Demand API Documentation](https://developers.booking.com/demand/docs/getting-started/overview)
- [Connectivity Documentation](https://developers.booking.com/connectivity/docs)
- [Website](https://www.booking.com/)
- [PrivacyPolicy](https://www.booking.com/content/privacy.html)
- [TermsOfService](https://www.booking.com/content/terms.html)

## Maintainers

**FN:** API Evangelist

**Email:** info@apievangelist.com
