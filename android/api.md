# API (Android)

The [Android client](android/overview.md) communicates with the [Backend Server](backend/overview.md) via REST API endpoints:

## Authentication
- `POST /auth/login` - handled by [LoginActivity](android/key-classes.md#LoginActivity)
- `POST /auth/register` - handled by [SignUpActivity](android/key-classes.md#SignUpActivity)

## Game Management
- `GET /games` - used by [HomeFragment](android/key-classes.md#HomeFragment) and [GameAdapter](android/key-classes.md#GameAdapter)
- `GET /games/{id}` - used by [GameDetailFragment](android/key-classes.md#GameDetailFragment)
- `POST /games` - game creation
- `PUT /games/{id}` - game updates
- `DELETE /games/{id}` - game deletion

## Reviews
- `GET /reviews` - review listing
- `POST /reviews` - review submission via [GameDetailFragment](android/key-classes.md#GameDetailFragment)

## Platforms
- `GET /platforms` - platform listing
- `GET /platforms/{id}` - platform details

## Implementation

All API calls are handled by [ApiClient](android/key-classes.md#ApiClient) with authentication managed by [SessionManager](android/key-classes.md#SessionManager).

Authentication is handled via JWT tokens from [Backend Auth API](backend/api.md#Auth). 