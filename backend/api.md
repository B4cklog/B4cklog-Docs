# API (Backend)

The [[backend/overview|Backend Server]] provides REST API endpoints consumed by [[android/overview|Android]] and [[web/overview|Web]] clients.

## Auth
- `POST /auth/login` - used by [[android/key-classes#LoginActivity|LoginActivity]] and [[web/key-components#LoginPage|LoginPage]]
- `POST /auth/register` - used by [[android/key-classes#SignUpActivity|SignUpActivity]] and [[web/key-components#RegisterPage|RegisterPage]]
- `POST /auth/refresh` - token refresh for [[android/key-classes#SessionManager|SessionManager]]

## Games
- `GET /games` - consumed by [[android/key-classes#HomeFragment|HomeFragment]] and [[web/key-components#GameList|GameList]]
- `POST /games` - game creation
- `GET /games/{id}` - used by [[android/key-classes#GameDetailFragment|GameDetailFragment]] and [[web/key-components#GameDetailPage|GameDetailPage]]
- `PUT /games/{id}` - game updates
- `DELETE /games/{id}` - game deletion
- `GET /games/search` - search functionality for [[web/key-components#SearchBar|SearchBar]]

## Platforms
- `GET /platforms` - platform listing for filters
- `GET /platforms/{id}` - platform details

## Reviews
- `GET /reviews` - review listing
- `POST /reviews` - review submission via [[android/key-classes#GameDetailFragment|GameDetailFragment]] and [[web/key-components#GameDetailPage|GameDetailPage]]
- `GET /reviews/{id}` - individual review details

## Implementation

All endpoints are handled by [[backend/key-classes#Controllers|Controllers]] with business logic in [[backend/key-classes#Services|Services]].
Data is persisted in [[backend/database|MySQL database]]. 