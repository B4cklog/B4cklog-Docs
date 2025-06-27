# Key Components (Web)

## Pages
- **[[LoginPage.tsx]]** / **[[RegisterPage.tsx]]**: Auth pages using [[backend/api#Auth|Auth API]]
- **[[GameList.tsx]]**: Game list display consuming [[backend/api#Games|Games API]]
- **[[GameDetailPage.tsx]]**: Game details and reviews via [[backend/api#Reviews|Reviews API]]
- **[[SearchBar.tsx]]**: Search input for [[backend/api#Games|Games search endpoint]]
- **[[Settings.tsx]]**: User settings and profile management
- **[[Navbar.tsx]]**: Main navigation between pages

## Components
- **[[HomePage.tsx]]**: Main dashboard with [[web/key-components#GameList|GameList]] and [[web/key-components#SearchBar|SearchBar]]
- **[[ProfilePage.tsx]]**: User profile management
- **[[SearchResultsPage.tsx]]**: Search results display
- **[[WelcomePage.tsx]]**: Landing page for new users

## API Integration

All components communicate with [[backend/overview|Backend Server]] through [[web/api|API service layer]].
Authentication state is managed across [[web/key-components#LoginPage|LoginPage]], [[web/key-components#RegisterPage|RegisterPage]], and [[web/key-components#ProfilePage|ProfilePage]]. 