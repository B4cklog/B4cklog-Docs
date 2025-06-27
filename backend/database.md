# Database (Backend)

- **MySQL database** for persistent storage
- **JPA/Hibernate** for ORM mapping
- **Main entities**: User, Game, Platform, Review, RefreshToken

## Entity Relationships

- **User**: Authentication and profile data for [[android/overview|Android]] and [[web/overview|Web]] clients
- **Game**: Game information shared across [[android/key-classes#GameAdapter|GameAdapter]] and [[web/key-components#GameList|GameList]]
- **Platform**: Gaming platforms for filtering
- **Review**: User reviews and ratings from [[android/key-classes#GameDetailFragment|GameDetailFragment]] and [[web/key-components#GameDetailPage|GameDetailPage]]
- **RefreshToken**: Token refresh mechanism for [[android/key-classes#SessionManager|SessionManager]]

## Data Access

- **Repositories**: Data access layer for [[backend/key-classes#Services|Services]]
- **DAOs**: Direct database operations
- **JPA Entities**: Mapped to [[backend/key-classes#Models|Models]] used by [[backend/api|API endpoints]] 