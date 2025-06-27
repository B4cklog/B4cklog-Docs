# Android Client Overview

The [Android client](android/overview.md) is built with Kotlin and follows MVVM architecture.

Main features:
- User authentication via [Backend Auth API](backend/api.md#Auth)
- Game list and details from [Games API](backend/api.md#Games)
- Review submission via [Reviews API](backend/api.md#Reviews)
- Profile management

## Architecture

- **Activities**: [MainActivity](android/key-classes.md#MainActivity), [LoginActivity](android/key-classes.md#LoginActivity), [SignUpActivity](android/key-classes.md#SignUpActivity)
- **Fragments**: [HomeFragment](android/key-classes.md#HomeFragment), [GameDetailFragment](android/key-classes.md#GameDetailFragment)
- **Network**: [ApiClient](android/key-classes.md#ApiClient) for [API communication](android/api.md)
- **Data**: [SessionManager](android/key-classes.md#SessionManager) for auth state

## Integration

Communicates with [Backend Server](backend/overview.md) via [REST API](android/api.md).
Shares data models with [Web Frontend](web/overview.md) through [Backend API](backend/api.md). 