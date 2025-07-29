\# Airbnb Clone - Backend Requirements



\## 1. User Authentication



\### Functional Description

Allows users (hosts/guests) to register, log in, and manage sessions securely using JWT.



\### API Endpoints

\- `POST /api/register`  

\- `POST /api/login`  

\- `GET /api/logout`



\### Input/Output

\*\*Register\*\*  

Request:

```json

{

&nbsp; "email": "user@example.com",

&nbsp; "password": "securePassword123"

}



{

&nbsp; "message": "Registration successful",

&nbsp; "token": "JWT\_TOKEN"

}



{

&nbsp; "title": "Cozy Cabin",

&nbsp; "description": "A quiet getaway in the woods",

&nbsp; "price": 120,

&nbsp; "location": "Cape Town"

}



{

&nbsp; "message": "Property listed",

&nbsp; "property\_id": 102

}



{

&nbsp; "property\_id": 102,

&nbsp; "check\_in": "2025-08-01",

&nbsp; "check\_out": "2025-08-05",

&nbsp; "guests": 2

}



{

&nbsp; "message": "Booking confirmed",

&nbsp; "booking\_id": 304

}

