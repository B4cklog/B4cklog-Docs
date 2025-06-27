# Web Frontend Overview

The [[web/overview|Web Frontend]] is built with React and TypeScript.
It provides a modern UI for managing your game backlog.

## Backend Integration

Communicates with [[backend/overview|Backend Server]] via [[web/api|REST API]] endpoints.
Shares authentication flow with [[android/overview|Android Client]] through [[backend/api#Auth|Backend Auth API]].

## Key Features

- **Authentication**: [[web/key-components#LoginPage|Login]] and [[web/key-components#RegisterPage|Registration]] via [[backend/api#Auth|Auth API]]
- **Game Management**: [[web/key-components#GameList|Game listing]] and [[web/key-components#GameDetailPage|Game details]] via [[backend/api#Games|Games API]]
- **Search**: [[web/key-components#SearchBar|Search functionality]] with [[backend/api#Games|Games search endpoint]]
- **Reviews**: Review system via [[backend/api#Reviews|Reviews API]]

## Architecture

- **Components**: Reusable UI components in [[web/structure#Components|components/]]
- **Pages**: Main application pages in [[web/structure#Pages|pages/]]
- **API Layer**: [[web/api|API service]] for [[backend/overview|Backend communication]] 