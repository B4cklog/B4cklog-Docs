# Web Frontend Structure

- **[components/](web/key-components.md#Components)**: Reusable UI components ([GameList](web/key-components.md#GameList), [SearchBar](web/key-components.md#SearchBar), [Navbar](web/key-components.md#Navbar))
- **[pages/](web/key-components.md#Pages)**: Main pages ([Home](web/key-components.md#HomePage), [Login](web/key-components.md#LoginPage), [Register](web/key-components.md#RegisterPage), [Profile](web/key-components.md#ProfilePage), [Game Detail](web/key-components.md#GameDetailPage), [Search Results](web/key-components.md#SearchResultsPage), [Welcome](web/key-components.md#WelcomePage))
- **[api/](web/api.md)**: API service layer for [Backend communication](backend/overview.md)
- **styles/**: CSS and theme files

## Component Hierarchy

1. **Pages** contain multiple **Components**
2. **Components** use **API layer** for [Backend communication](backend/api.md)
3. **API layer** handles [REST requests](web/api.md) to [Backend Server](backend/overview.md) 