# Station REST API

This demonstration reference shows the documentation structure for a booking API. The endpoints and examples are portfolio samples and do not represent a public production service.

## Base URL

```text
https://api.example.com/api/v1
```

## Authentication

Protected operations use a bearer token:

```http
Authorization: Bearer <access_token>
```

## Documented operation

| Method | Path | Description |
|---|---|---|
| `POST` | `/bookings` | Create a booking |

This version documents one operation, matching the scope of the OpenAPI file.

## Create a booking

`POST /bookings`

Creates a booking for an available seat on a trip.

### Request

```json
{
  "tripId": 152,
  "seatId": 38,
  "passenger": {
    "firstName": "Ivan",
    "lastName": "Petrov"
  }
}
```

### Successful response

Status: `201 Created`

```json
{
  "id": 8432,
  "status": "confirmed",
  "tripId": 152,
  "seatId": 38
}
```

### Errors

| Status | Code | Meaning |
|---|---|---|
| `400` | `INVALID_REQUEST` | A required field is missing or invalid |
| `401` | `UNAUTHORIZED` | The token is missing or invalid |
| `404` | `RESOURCE_NOT_FOUND` | The trip or seat does not exist |
| `409` | `SEAT_UNAVAILABLE` | The seat is no longer available |

Example error:

```json
{
  "error": {
    "code": "SEAT_UNAVAILABLE",
    "message": "The selected seat is no longer available."
  }
}
```

## OpenAPI

See the [OpenAPI specification](openapi.yaml) for a machine-readable version of the sample.
