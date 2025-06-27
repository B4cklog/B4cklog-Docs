# API (Android)

The [[android/overview|Android client]] communicates with the [[backend/overview|Backend Server]] via REST API endpoints:

## Authentication
- `POST /auth/login` - handled by [[android/key-classes#LoginActivity|LoginActivity]]
- `POST /auth/register` - handled by [[android/key-classes#SignUpActivity|SignUpActivity]]

## Game Management
- `GET /games` - used by [[android/key-classes#HomeFragment|HomeFragment]] and [[android/key-classes#GameAdapter|GameAdapter]]
- `GET /games/{id}` - used by [[android/key-classes#GameDetailFragment|GameDetailFragment]]
- `POST /games` - game creation
- `PUT /games/{id}` - game updates
- `DELETE /games/{id}` - game deletion

## Reviews
- `GET /reviews` - review listing
- `POST /reviews` - review submission via [[android/key-classes#GameDetailFragment|GameDetailFragment]]

## Platforms
- `GET /platforms` - platform listing
- `GET /platforms/{id}` - platform details

## Implementation

All API calls are handled by [[android/key-classes#ApiClient|ApiClient]] with authentication managed by [[android/key-classes#SessionManager|SessionManager]].

Authentication is handled via JWT tokens from [[backend/api#Auth|Backend Auth API]]. 