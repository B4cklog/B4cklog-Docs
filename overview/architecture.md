# Architecture

B4cklog is a modular monorepo with three main components:

- **[Android Client](android/overview.md)**: Kotlin, MVVM, Retrofit
- **[Backend Server](backend/overview.md)**: Spring Boot (Kotlin), REST API, MySQL
- **[Web Frontend](web/overview.md)**: React, TypeScript, Tailwind CSS

All modules communicate via REST API. [Docker Compose](devops/docker-compose.md) is used for local development and deployment.

## Component Interactions

### Authentication Flow
1. [Android](android/overview.md) and [Web](web/overview.md) clients authenticate via [Auth API](backend/api.md#Auth)
2. [Backend](backend/overview.md) validates credentials and returns JWT tokens
3. Clients use tokens for subsequent API calls

### Data Flow
1. [Backend](backend/overview.md) serves game data via [Games API](backend/api.md#Games)
2. [Android](android/overview.md) and [Web](web/overview.md) consume data via [Android API](android/api.md) and [Web API](web/api.md)
3. [Database](backend/database.md) stores all persistent data

## Infrastructure

- [Docker Compose](devops/docker-compose.md) orchestrates all services
- [Environment](devops/environments.md) configuration via environment variables
- [Deployment](devops/deployment.md) process for production 