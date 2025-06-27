# Key Components (Web)

## Pages
- **[LoginPage.tsx]**: Auth pages using [Auth API](backend/api.md#Auth)
- **[RegisterPage.tsx]**: Auth pages using [Auth API](backend/api.md#Auth)
- **[GameList.tsx]**: Game list display consuming [Games API](backend/api.md#Games)
- **[GameDetailPage.tsx]**: Game details and reviews via [Reviews API](backend/api.md#Reviews)
- **[SearchBar.tsx]**: Search input for [Games search endpoint](backend/api.md#Games)
- **[Settings.tsx]**: User settings and profile management
- **[Navbar.tsx]**: Main navigation between pages

## Components
- **[HomePage.tsx]**: Main dashboard with [GameList](web/key-components.md#GameList) and [SearchBar](web/key-components.md#SearchBar)
- **[ProfilePage.tsx]**: User profile management
- **[SearchResultsPage.tsx]**: Search results display
- **[WelcomePage.tsx]**: Landing page for new users

## API Integration

All components communicate with [Backend Server](backend/overview.md) through [API service layer](web/api.md).
Authentication state is managed across [LoginPage](web/key-components.md#LoginPage), [RegisterPage](web/key-components.md#RegisterPage), and [ProfilePage](web/key-components.md#ProfilePage). 