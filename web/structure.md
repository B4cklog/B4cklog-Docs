# Web Frontend Structure

- **[[web/key-components#Components|components/]]**: Reusable UI components ([[web/key-components#GameList|GameList]], [[web/key-components#SearchBar|SearchBar]], [[web/key-components#Navbar|Navbar]])
- **[[web/key-components#Pages|pages/]]**: Main pages ([[web/key-components#HomePage|Home]], [[web/key-components#LoginPage|Login]], [[web/key-components#RegisterPage|Register]], [[web/key-components#ProfilePage|Profile]], [[web/key-components#GameDetailPage|Game Detail]], [[web/key-components#SearchResultsPage|Search Results]], [[web/key-components#WelcomePage|Welcome]])
- **[[web/api|api/]]**: API service layer for [[backend/overview|Backend communication]]
- **styles/**: CSS and theme files

## Component Hierarchy

1. **Pages** contain multiple **Components**
2. **Components** use **API layer** for [[backend/api|Backend communication]]
3. **API layer** handles [[web/api|REST requests]] to [[backend/overview|Backend Server]] 