# API (Backend)

The [Backend Server](backend/overview.md) provides REST API endpoints consumed by [Android](android/overview.md) and [Web](web/overview.md) clients.

## Auth
- `POST /auth/login` - used by [LoginActivity](android/key-classes.md#LoginActivity) and [LoginPage](web/key-components.md#LoginPage)
- `POST /auth/register` - used by [SignUpActivity](android/key-classes.md#SignUpActivity) and [RegisterPage](web/key-components.md#RegisterPage)
- `POST /auth/refresh` - token refresh for [SessionManager](android/key-classes.md#SessionManager)

## Games
- `GET /games` - consumed by [HomeFragment](android/key-classes.md#HomeFragment) and [GameList](web/key-components.md#GameList)
- `POST /games` - game creation
- `GET /games/{id}` - used by [GameDetailFragment](android/key-classes.md#GameDetailFragment) and [GameDetailPage](web/key-components.md#GameDetailPage)
- `PUT /games/{id}` - game updates
- `DELETE /games/{id}` - game deletion
- `GET /games/search` - search functionality for [SearchBar](web/key-components.md#SearchBar)

## Platforms
- `GET /platforms` - platform listing for filters
- `GET /platforms/{id}` - platform details

## Reviews
- `GET /reviews` - review listing
- `POST /reviews` - review submission via [GameDetailFragment](android/key-classes.md#GameDetailFragment) and [GameDetailPage](web/key-components.md#GameDetailPage)
- `GET /reviews/{id}` - individual review details

## Implementation

All endpoints are handled by [Controllers](backend/key-classes.md#Controllers) with business logic in [Services](backend/key-classes.md#Services).
Data is persisted in [MySQL database](backend/database.md). 