# Movie Discovery Hub

An offline-first movie discovery application built with React, TypeScript and Vite.

## Features
- Works offline with a bundled starter movie catalogue.
- Search movies by title, genre or overview.
- Filter by genre and sort by rating or release year.
- Save and remove favourites.
- Keep a personal watchlist.
- Favourites and watchlist are stored in this browser using localStorage.

## Run locally
```bash
npm install
npm run dev
```

Open the local URL printed by Vite.

## Offline notes
The bundled catalogue and saved lists work offline after the app has been loaded once. Remote posters are illustrative and require internet; the app shows a local fallback when they cannot load. No account or backend is required.

## Android
Android packaging with Capacitor will be added in a later project step.
