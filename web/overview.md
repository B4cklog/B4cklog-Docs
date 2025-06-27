# Web Frontend Overview

The [Web Frontend](web/overview.md) is built with React and TypeScript.
It provides a modern UI for managing your game backlog.

## Backend Integration

Communicates with [Backend Server](backend/overview.md) via [REST API](web/api.md) endpoints.
Shares authentication flow with [Android Client](android/overview.md) through [Backend Auth API](backend/api.md#Auth).

## Key Features

- **Authentication**: [Login](web/key-components.md#LoginPage) and [Registration](web/key-components.md#RegisterPage) via [Auth API](backend/api.md#Auth)
- **Game Management**: [Game listing](web/key-components.md#GameList) and [Game details](web/key-components.md#GameDetailPage) via [Games API](backend/api.md#Games)
- **Search**: [Search functionality](web/key-components.md#SearchBar) with [Games search endpoint](backend/api.md#Games)
- **Reviews**: Review system via [Reviews API](backend/api.md#Reviews)

## Architecture

- **Components**: Reusable UI components in [components/](web/structure.md#Components)
- **Pages**: Main application pages in [pages/](web/structure.md#Pages)
- **API Layer**: [API service](web/api.md) for [Backend communication](backend/overview.md) 