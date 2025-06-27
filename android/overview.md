# Android Client Overview

The [[android/overview|Android client]] is built with Kotlin and follows MVVM architecture.

Main features:
- User authentication via [[backend/api#Auth|Backend Auth API]]
- Game list and details from [[backend/api#Games|Games API]]
- Review submission via [[backend/api#Reviews|Reviews API]]
- Profile management

## Architecture

- **Activities**: [[android/key-classes#MainActivity|MainActivity]], [[android/key-classes#LoginActivity|LoginActivity]], [[android/key-classes#SignUpActivity|SignUpActivity]]
- **Fragments**: [[android/key-classes#HomeFragment|HomeFragment]], [[android/key-classes#GameDetailFragment|GameDetailFragment]]
- **Network**: [[android/key-classes#ApiClient|ApiClient]] for [[android/api|API communication]]
- **Data**: [[android/key-classes#SessionManager|SessionManager]] for auth state

## Integration

Communicates with [[backend/overview|Backend Server]] via [[android/api|REST API]].
Shares data models with [[web/overview|Web Frontend]] through [[backend/api|Backend API]]. 