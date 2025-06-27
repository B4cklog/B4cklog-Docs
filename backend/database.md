# Database (Backend)

- **MySQL database** for persistent storage
- **JPA/Hibernate** for ORM mapping
- **Main entities**: User, Game, Platform, Review, RefreshToken

## Entity Relationships

- **User**: Authentication and profile data for [Android](android/overview.md) and [Web](web/overview.md) clients
- **Game**: Game information shared across [GameAdapter](android/key-classes.md#GameAdapter) and [GameList](web/key-components.md#GameList)
- **Platform**: Gaming platforms for filtering
- **Review**: User reviews and ratings from [GameDetailFragment](android/key-classes.md#GameDetailFragment) and [GameDetailPage](web/key-components.md#GameDetailPage)
- **RefreshToken**: Token refresh mechanism for [SessionManager](android/key-classes.md#SessionManager)

## Data Access

- **Repositories**: Data access layer for [Services](backend/key-classes.md#Services)
- **DAOs**: Direct database operations
- **JPA Entities**: Mapped to [Models](backend/key-classes.md#Models) used by [API endpoints](backend/api.md) 