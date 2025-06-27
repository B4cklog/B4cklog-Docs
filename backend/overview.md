# Backend Server Overview

The [Backend Server](backend/overview.md) is a REST API built with Spring Boot (Kotlin).
It handles authentication, game data, reviews, and user management.

## Client Integration

- **[Android Client](android/overview.md)**: Consumes [API endpoints](backend/api.md) via [Android API layer](android/api.md)
- **[Web Frontend](web/overview.md)**: Consumes [API endpoints](backend/api.md) via [Web API layer](web/api.md)

## Core Components

- **[Controllers](backend/key-classes.md#Controllers)**: Handle HTTP requests from [Android](android/overview.md) and [Web](web/overview.md) clients
- **[Services](backend/key-classes.md#Services)**: Business logic for game management and authentication
- **[Database](backend/database.md)**: MySQL storage for all persistent data
- **[Models](backend/key-classes.md#Models)**: Data entities shared across the system

## External Integrations

- **IGDB API**: Game data enrichment via [IGDBService](backend/key-classes.md#IGDBService)
- **JWT Authentication**: Token-based auth for [Android](android/overview.md) and [Web](web/overview.md) clients 