# Backend Structure

- **[[backend/key-classes#Controllers|controller/]]**: REST controllers handling requests from [[android/overview|Android]] and [[web/overview|Web]] clients
- **[[backend/key-classes#Services|service/]]**: Business logic for authentication, game management, and data processing
- **[[backend/key-classes#Models|model/]]**: Data models (game, platform, review, user, token) shared with [[android/overview|Android]] and [[web/overview|Web]]
- **dto/**: Data transfer objects for [[backend/api|API communication]]
- **util/**: Utilities ([[backend/key-classes#HashUtils|HashUtils]], [[backend/key-classes#JwtUtils|JwtUtils]]) for authentication and data processing

## Data Flow

1. **Controllers** receive requests from [[android/api|Android API]] and [[web/api|Web API]]
2. **Services** process business logic and interact with [[backend/database|Database]]
3. **Models** represent data entities stored in [[backend/database|MySQL]]
4. **DTOs** format data for [[backend/api|API responses]] 