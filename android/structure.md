# Android Client Structure

- **[[android/key-classes#Activities|activities/]]**: Main screens ([[android/key-classes#LoginActivity|Login]], [[android/key-classes#MainActivity|Main]], [[android/key-classes#SignUpActivity|SignUp]], Welcome)
- **[[android/key-classes#Fragments|fragments/]]**: UI fragments ([[android/key-classes#HomeFragment|Home]], Profile, [[android/key-classes#GameDetailFragment|Game Detail]], etc.)
- **adapters/**: RecyclerView adapters for [[android/key-classes#GameAdapter|GameAdapter]], [[android/key-classes#ScreenshotAdapter|ScreenshotAdapter]]
- **models/**: Data models (Game, Platform, Review, User) shared with [[backend/overview|Backend]]
- **network/**: [[android/key-classes#ApiClient|API clients]] for [[android/api|REST communication]]
- **util/**: Utilities ([[android/key-classes#AuthPrefs|AuthPrefs]], [[android/key-classes#SessionManager|SessionManager]])

## Data Flow

1. [[android/key-classes#ApiClient|ApiClient]] → [[backend/api|Backend API]]
2. [[android/key-classes#SessionManager|SessionManager]] → [[backend/api#Auth|Auth API]]
3. [[android/key-classes#GameAdapter|GameAdapter]] → [[backend/api#Games|Games API]] 