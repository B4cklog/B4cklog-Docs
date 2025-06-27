# API (Web)

The [Web Frontend](web/overview.md) communicates with the [Backend Server](backend/overview.md) via REST API endpoints:

## Authentication
- `POST /auth/login` - used by [LoginPage](web/key-components.md#LoginPage)
- `POST /auth/register` - used by [RegisterPage](web/key-components.md#RegisterPage)

## Game Management
- `GET /games` - consumed by [GameList](web/key-components.md#GameList) and [HomePage](web/key-components.md#HomePage)
- `GET /games/{id}` - used by [GameDetailPage](web/key-components.md#GameDetailPage)
- `POST /games` - game creation
- `PUT /games/{id}` - game updates
- `DELETE /games/{id}` - game deletion
- `GET /games/search` - used by [SearchBar](web/key-components.md#SearchBar) and [SearchResultsPage](web/key-components.md#SearchResultsPage)

## Reviews
- `GET /reviews` - review listing
- `POST /reviews` - review submission via [GameDetailPage](web/key-components.md#GameDetailPage)

## Platforms
- `GET /platforms` - platform listing for filters
- `GET /platforms/{id}` - platform details

## Implementation

All API calls are handled by [API service layer](web/api.md) with authentication managed through [Backend Auth API](backend/api.md#Auth).

Authentication is handled via JWT tokens from [Backend Auth endpoints](backend/api.md#Auth). 