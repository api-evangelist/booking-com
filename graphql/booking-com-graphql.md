# Booking.com GraphQL Schema

## Overview

This is a conceptual GraphQL schema for the Booking.com platform, covering accommodation search, availability, booking, reviews, and property management. It is derived from the public REST/XML APIs available through the Booking.com Demand API and Connectivity APIs.

- Provider: Booking.com
- Category: Accommodations, Travel, Booking
- REST API: https://developers.booking.com/demand/docs/getting-started/overview
- Connectivity API: https://developers.booking.com/connectivity/docs
- GitHub: https://github.com/bookingcom

## Schema Source

Conceptual schema derived from the Booking.com Demand API (REST/JSON) and Connectivity APIs (XML/REST). Booking.com does not currently publish a public GraphQL endpoint. This schema models the domain objects and operations documented in their public developer portal.

## Types

- Property, Hotel, Accommodation, Room, Apartment, Villa, Hostel
- Availability, RoomAvailability, RateInfo, Price, PriceBreakdown
- Tax, Fee, CancellationPolicy, PaymentPolicy
- Reservation, Booking, BookingGuest, GuestInfo
- Payment, PaymentMethod
- Review, ReviewScore, ReviewCategory, ReviewBreakdown, ReviewText, GuestReview
- AmenityList, Facility, PetPolicy, BabyBed, ChildPolicy, ExtraBeds
- PropertyHighlight, PropertyLocation, GeoCoordinate, NearbyPlace
- SearchResult, HotelSearch, AvailabilitySearch, Filter, SortOrder, PageResult
- DiscountedRate, PromoCampaign, AffiliatePartner, Commission
- RoomType, BedType, BedConfig
- Image, Language

## Queries

- property(id: ID!): Property
- searchHotels(input: HotelSearch!): SearchResult
- availability(input: AvailabilitySearch!): [RoomAvailability]
- review(id: ID!): Review
- reviews(propertyId: ID!, page: Int): PageResult

## Mutations

- createReservation(input: ReservationInput!): Reservation
- cancelReservation(id: ID!): Reservation
- updateReservation(id: ID!, input: ReservationInput!): Reservation
