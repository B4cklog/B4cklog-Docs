# Backend Server Overview

The [[backend/overview|Backend Server]] is a REST API built with Spring Boot (Kotlin).
It handles authentication, game data, reviews, and user management.

## Client Integration

- **[[android/overview|Android Client]]**: Consumes [[backend/api|API endpoints]] via [[android/api|Android API layer]]
- **[[web/overview|Web Frontend]]**: Consumes [[backend/api|API endpoints]] via [[web/api|Web API layer]]

## Core Components

- **[[backend/key-classes#Controllers|Controllers]]**: Handle HTTP requests from [[android/overview|Android]] and [[web/overview|Web]] clients
- **[[backend/key-classes#Services|Services]]**: Business logic for game management and authentication
- **[[backend/database|Database]]**: MySQL storage for all persistent data
- **[[backend/key-classes#Models|Models]]**: Data entities shared across the system

## External Integrations

- **IGDB API**: Game data enrichment via [[backend/key-classes#IGDBService|IGDBService]]
- **JWT Authentication**: Token-based auth for [[android/overview|Android]] and [[web/overview|Web]] clients 