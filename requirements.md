# Airbnb Clone - Backend Requirements

This document defines the technical and functional requirements for the core backend features of the Airbnb Clone project, including User Authentication, Property Management, and Booking System.

## User Authentication

Enables both guests and hosts to register, log in, and manage sessions securely using JSON Web Tokens (JWT).

**API Endpoints:**
- `POST /api/register`
- `POST /api/login`
- `GET /api/logout`

## Property Management

Allows hosts to create and manage property listings.

**API Endpoints:**
- `POST /api/properties`

## Booking System

Allows users to book listed properties.

**API Endpoints:**
- `POST /api/bookings`

## Example Combined Flow

### 🔐 Registration Request
```json
{
  "email": "user@example.com",
  "password": "securePassword123"
}
```

### ✅ Registration Response
```json
{
  "message": "Registration successful",
  "token": "JWT_TOKEN"
}
```

### 🔐 Login Request
```json
{
  "email": "user@example.com",
  "password": "securePassword123"
}
```

### ✅ Login Response
```json
{
  "message": "Login successful",
  "token": "JWT_TOKEN"
}
```

### 🚪 Logout Response
```json
{
  "message": "Logout successful"
}
```

### 🏡 Property Listing Request
```json
{
  "title": "Cozy Cabin",
  "description": "A quiet getaway in the woods",
  "price": 120,
  "location": "Cape Town"
}
```

### ✅ Property Listing Response
```json
{
  "message": "Property listed",
  "property_id": 102
}
```

### 📆 Booking Request
```json
{
  "property_id": 102,
  "check_in": "2025-08-01",
  "check_out": "2025-08-05",
  "guests": 2
}
```

### ✅ Booking Response
```json
{
  "message": "Booking confirmed",
  "booking_id": 304
}
```
