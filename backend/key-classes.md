# Key Classes (Backend)

## Controllers
- **[AuthController.kt]**: Authentication endpoints for [Android](android/api.md) and [Web](web/api.md) clients
- **[GameController.kt]**: Game management endpoints consumed by [HomeFragment](android/key-classes.md#HomeFragment) and [GameList](web/key-components.md#GameList)
- **[ReviewController.kt]**: Review endpoints used by [GameDetailFragment](android/key-classes.md#GameDetailFragment) and [GameDetailPage](web/key-components.md#GameDetailPage)
- **[UserController.kt]**: User management for profile features

## Services
- **[AuthService.kt]**: Auth logic for [JWT token](backend/api.md#Auth) generation and validation
- **[IGDBService.kt]**: IGDB API integration for game data enrichment
- **[JwtUtils.kt]**: JWT token utilities for [SessionManager](android/key-classes.md#SessionManager) and web auth

## Models
- **User**: Authentication and profile data
- **Game**: Game information shared with [Android](android/overview.md) and [Web](web/overview.md)
- **Review**: User reviews and ratings
- **Platform**: Gaming platforms
- **RefreshToken**: Token refresh mechanism

## Utilities
- **[HashUtils.kt]**: Password hashing for secure authentication
- **[JwtUtils.kt]**: JWT token management for [Android](android/api.md) and [Web](web/api.md) clients 