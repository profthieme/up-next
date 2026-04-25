# Coming Soon… — Family Watchlist

A personal watchlist app for keeping track of shows, movies, and documentaries,
including where to stream each one. Family members each get their own profile,
and lists sync across everyone's devices through Firebase.

## What's in this folder

- `index.html` — the entire app (React + styles + logic + Firebase, in one file)
- `manifest.json` — makes the app installable to a phone home screen
- `icon-192.png`, `icon-512.png`, `icon-512-maskable.png`, `favicon.png` — app icons
- `README.md` — this file

## Updating the app on GitHub Pages

1. In your GitHub repository (`up-next` or whatever you named it), click **Add file → Upload files**.
2. Drag this entire folder onto the upload zone.
3. Scroll down. Add a commit message (or leave the default), and click **Commit changes**.
4. GitHub Pages rebuilds in 1–2 minutes. Your live URL stays the same.

For small changes to a single file, you can also click the file in the repo,
click the pencil icon to edit, paste new contents, and commit.

## Installing to phone home screens

**iPhone (Safari):** open the URL → Share button → "Add to Home Screen."
**Android (Chrome):** open the URL → three-dot menu → "Add to Home Screen" or "Install app."
**Samsung TV / Fire Stick:** open the URL in the built-in browser and bookmark it.

After updating to a new icon or name, you may need to remove the old home-screen
icon and re-add it, since phones cache the icon.

## How data is stored

Everyone's profiles, lists, and items live in a shared Firestore database at the
Firebase project `tfamily-watchlists`. Any change on one device shows up on all
other devices within a second or two.

## Tech stack (for the curious)

- Plain HTML + React via CDN (no build step).
- TMDB API for movie/TV info and JustWatch streaming availability.
- OMDb API for IMDb ratings.
- Firebase Firestore for real-time family sync.
- Fonts: Fraunces (display) and DM Sans (body), via Google Fonts.
