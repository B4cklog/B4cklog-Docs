# Key Classes (Backend)

## Controllers
- **[[AuthController.kt]]**: Authentication endpoints for [[android/api|Android]] and [[web/api|Web]] clients
- **[[GameController.kt]]**: Game management endpoints consumed by [[android/key-classes#HomeFragment|HomeFragment]] and [[web/key-components#GameList|GameList]]
- **[[ReviewController.kt]]**: Review endpoints used by [[android/key-classes#GameDetailFragment|GameDetailFragment]] and [[web/key-components#GameDetailPage|GameDetailPage]]
- **[[UserController.kt]]**: User management for profile features

## Services
- **[[AuthService.kt]]**: Auth logic for [[backend/api#Auth|JWT token]] generation and validation
- **[[IGDBService.kt]]**: IGDB API integration for game data enrichment
- **[[JwtUtils.kt]]**: JWT token utilities for [[android/key-classes#SessionManager|SessionManager]] and web auth

## Models
- **User**: Authentication and profile data
- **Game**: Game information shared with [[android/overview|Android]] and [[web/overview|Web]]
- **Review**: User reviews and ratings
- **Platform**: Gaming platforms
- **RefreshToken**: Token refresh mechanism

## Utilities
- **[[HashUtils.kt]]**: Password hashing for secure authentication
- **[[JwtUtils.kt]]**: JWT token management for [[android/api|Android]] and [[web/api|Web]] clients 