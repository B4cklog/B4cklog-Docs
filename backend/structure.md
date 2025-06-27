# Backend Structure

- **[controller/](backend/key-classes.md#Controllers)**: REST controllers handling requests from [Android](android/overview.md) and [Web](web/overview.md) clients
- **[service/](backend/key-classes.md#Services)**: Business logic for authentication, game management, and data processing
- **[model/](backend/key-classes.md#Models)**: Data models (game, platform, review, user, token) shared with [Android](android/overview.md) and [Web](web/overview.md)
- **dto/**: Data transfer objects for [API communication](backend/api.md)
- **util/**: Utilities ([HashUtils](backend/key-classes.md#HashUtils), [JwtUtils](backend/key-classes.md#JwtUtils)) for authentication and data processing

## Data Flow

1. **Controllers** receive requests from [Android API](android/api.md) and [Web API](web/api.md)
2. **Services** process business logic and interact with [Database](backend/database.md)
3. **Models** represent data entities stored in [MySQL](backend/database.md)
4. **DTOs** format data for [API responses](backend/api.md) 