# Key Classes (Android)

## Activities
- **[MainActivity.kt]**: Main navigation and fragment host, integrates with [fragments](android/structure.md#Fragments)
- **[LoginActivity.kt]** / **[SignUpActivity.kt]**: Auth screens, communicate with [Auth API](backend/api.md#Auth)

## Fragments
- **[HomeFragment.kt]**: Main game list, uses [GameAdapter.kt] and [Games API](backend/api.md#Games)
- **[GameDetailFragment.kt]**: Game details and reviews, integrates with [Reviews API](backend/api.md#Reviews)

## Network Layer
- **[ApiClient.kt]**: Network layer for all [API communication](android/api.md) with [Backend](backend/overview.md)
- **[SessionManager.kt]**: Auth/session management, handles [JWT tokens](backend/api.md#Auth)

## Adapters
- **[GameAdapter.kt]**: Displays game list from [Games API](backend/api.md#Games)
- **[ScreenshotAdapter.kt]**: Shows game screenshots

## Utilities
- **[AuthPrefs.kt]**: Local auth preferences storage
- **[SessionManager.kt]**: Manages user sessions and [authentication state](backend/api.md#Auth) 