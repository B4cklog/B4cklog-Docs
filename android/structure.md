# Android Client Structure

- **[activities/](android/key-classes.md#Activities)**: Main screens ([Login](android/key-classes.md#LoginActivity), [Main](android/key-classes.md#MainActivity), [SignUp](android/key-classes.md#SignUpActivity), Welcome)
- **[fragments/](android/key-classes.md#Fragments)**: UI fragments ([Home](android/key-classes.md#HomeFragment), Profile, [Game Detail](android/key-classes.md#GameDetailFragment), etc.)
- **adapters/**: RecyclerView adapters for [GameAdapter](android/key-classes.md#GameAdapter), [ScreenshotAdapter](android/key-classes.md#ScreenshotAdapter)
- **models/**: Data models (Game, Platform, Review, User) shared with [Backend](backend/overview.md)
- **network/**: [API clients](android/key-classes.md#ApiClient) for [REST communication](android/api.md)
- **util/**: Utilities ([AuthPrefs](android/key-classes.md#AuthPrefs), [SessionManager](android/key-classes.md#SessionManager))

## Data Flow

1. [ApiClient](android/key-classes.md#ApiClient) → [Backend API](backend/api.md)
2. [SessionManager](android/key-classes.md#SessionManager) → [Auth API](backend/api.md#Auth)
3. [GameAdapter](android/key-classes.md#GameAdapter) → [Games API](backend/api.md#Games) 