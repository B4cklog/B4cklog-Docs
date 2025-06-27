# Key Classes (Android)

## Activities
- **[[MainActivity.kt]]**: Main navigation and fragment host, integrates with [[android/structure#Fragments|fragments]]
- **[[LoginActivity.kt]]** / **[[SignUpActivity.kt]]**: Auth screens, communicate with [[backend/api#Auth|Auth API]]

## Fragments
- **[[HomeFragment.kt]]**: Main game list, uses [[GameAdapter.kt]] and [[backend/api#Games|Games API]]
- **[[GameDetailFragment.kt]]**: Game details and reviews, integrates with [[backend/api#Reviews|Reviews API]]

## Network Layer
- **[[ApiClient.kt]]**: Network layer for all [[android/api|API communication]] with [[backend/overview|Backend]]
- **[[SessionManager.kt]]**: Auth/session management, handles [[backend/api#Auth|JWT tokens]]

## Adapters
- **[[GameAdapter.kt]]**: Displays game list from [[backend/api#Games|Games API]]
- **[[ScreenshotAdapter.kt]]**: Shows game screenshots

## Utilities
- **[[AuthPrefs.kt]]**: Local auth preferences storage
- **[[SessionManager.kt]]**: Manages user sessions and [[backend/api#Auth|authentication state]] 