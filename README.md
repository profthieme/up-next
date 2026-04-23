# Up Next — Family Watchlist

A personal watchlist app for keeping track of shows, movies, and documentaries,
including where to stream each one. Family members each get their own profile,
and lists sync across everyone's devices through Firebase.

## What's in this folder

- `index.html` — the entire app (React + styles + logic + Firebase, in one file)
- `manifest.json` — makes the app installable to a phone home screen
- `icon-192.png`, `icon-512.png`, `icon-512-maskable.png`, `favicon.png` — app icons
- `README.md` — this file

## Updating the app on Netlify

1. In your Netlify dashboard, click your site (`tfamily-watchlists`).
2. Click the **Deploys** tab at the top.
3. Scroll down to the drag-and-drop zone: *"Need to update your site?..."*
4. Drag this entire folder onto it.
5. Wait a few seconds. Your live URL stays the same.

## Installing to phone home screens

**iPhone (Safari):** open the URL → Share button → "Add to Home Screen."
**Android (Chrome):** open the URL → three-dot menu → "Add to Home Screen" or "Install app."
**Samsung TV / Fire Stick:** open the URL in the built-in browser and bookmark it.

## How data is stored

Everyone's profiles, lists, and items live in a shared Firestore database at the
Firebase project `tfamily-watchlists`. Any change on one device shows up on all
other devices within a second or two.

## Tech stack (for the curious)

- Plain HTML + React via CDN (no build step).
- TMDB API for movie/TV info and JustWatch streaming availability.
- Firebase Firestore for real-time family sync.
- Fonts: Fraunces (display) and DM Sans (body), via Google Fonts.
