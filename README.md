# Movie Discovery Hub

Responsive international movie and TV discovery app built with React, TypeScript, Vite, Tailwind CSS and Capacitor.

## Current capabilities
- TMDB discovery shelves: trending today and this week, popular and now-playing movies, top-rated movies, upcoming releases, popular and top-rated series, and TV airing today (requires your own API Read Access Token).
- Search movies, TV shows and people; filter by genre, year and minimum rating.
- Movie/TV detail view, synopsis, rating, release date, runtime, genres, cast and YouTube trailer link when available.
- Actor profiles with biography, birthday, birthplace and known credits.
- Local favourites, watchlist, watched and recently viewed lists stored in this browser (up to 30 recent titles).
- Create custom collections and add/remove titles to organize a personal cinema library.
- Export and import a JSON backup of favourites, watchlist, watched titles, recently viewed titles and custom collections.
- Share movie and series details using native device sharing or a copied deep link.
- Random title discovery with the Surprise me action; filter and sort results by popularity, rating, release year and genre.
- Responsive desktop/mobile layout and online/offline indicator.
- Capacitor Android configuration and scripts.

## Run on Windows (Git Bash)
~~~bash
npm install
npm run dev
~~~

## TMDB setup
1. Create a TMDB account and request an API key at https://www.themoviedb.org/settings/api
2. Copy the API Read Access Token (Bearer token).
3. Open Settings in the app, paste the token and save.

The token is stored in this browser and is not committed to GitHub. For public production use, avoid shipping private secrets in frontend code; use a secure server-side proxy or an appropriate public-key approach and follow TMDB terms, attribution and rate limits. Free/non-commercial eligibility depends on TMDB current terms.

## Android
Install Android Studio and Android SDK first, then run:
~~~bash
npm install
npx cap add android
npm run android:sync
npm run android:open
~~~
In Android Studio choose Build → Build Bundle(s) / APK(s) → Build APK(s). iOS requires macOS and Xcode.

## Hosting
Deploy to Vercel or Netlify with build command `npm run build` and output directory `dist`. Users add their own TMDB token in app Settings; do not commit it.

## Data and privacy
This version does not yet include Supabase/Firebase accounts or cloud sync. Favourites, watchlist, watched state and custom collections are local to the current browser/device. Use the library export/import controls to move a JSON backup between browsers. Shared title links identify a TMDB title but do not transfer private library data. Live TMDB data requires internet; do not assume the full catalogue works offline.

## Implementation status and roadmap
The current implementation includes the features listed above. `FEATURE_ROADMAP.md` is a planned capability backlog (700+ entries), not a list of completed work. The long-term 5,000-feature ambition is not complete and is not represented as implemented. Items requiring accounts, shared/cloud data, realtime services, provider licensing or a secure backend remain future phases.

## Attribution
This product uses the TMDB API but is not endorsed or certified by TMDB. Add TMDB-required branding and notice before public release, following current branding guidelines.
