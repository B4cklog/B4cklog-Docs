# Architecture

B4cklog is a modular monorepo with three main components:

- **[[android/overview|Android Client]]**: Kotlin, MVVM, Retrofit
- **[[backend/overview|Backend Server]]**: Spring Boot (Kotlin), REST API, MySQL
- **[[web/overview|Web Frontend]]**: React, TypeScript, Tailwind CSS

All modules communicate via REST API. [[devops/docker-compose|Docker Compose]] is used for local development and deployment.

## Component Interactions

### Authentication Flow
1. [[android/overview|Android]] and [[web/overview|Web]] clients authenticate via [[backend/api#Auth|Auth API]]
2. [[backend/overview|Backend]] validates credentials and returns JWT tokens
3. Clients use tokens for subsequent API calls

### Data Flow
1. [[backend/overview|Backend]] serves game data via [[backend/api#Games|Games API]]
2. [[android/overview|Android]] and [[web/overview|Web]] consume data via [[android/api|Android API]] and [[web/api|Web API]]
3. [[backend/database|Database]] stores all persistent data

## Infrastructure

- [[devops/docker-compose|Docker Compose]] orchestrates all services
- [[devops/environments|Environment]] configuration via environment variables
- [[devops/deployment|Deployment]] process for production 