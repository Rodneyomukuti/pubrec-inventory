# PUBReC Lab Inventory — phone app

Installable app for the PUBReC Lab Inventory (Pwani University Biosciences Research Centre).
It opens the live inventory full-screen with the PUBReC icon. All data stays in the Google Sheet behind the web app.

## Install on a phone
- **Android (Chrome):** open the app link, then tap **Install app** (or ⋮ → *Add to Home screen*).
- **iPhone (Safari):** open the app link, tap **Share → Add to Home Screen**.

## Publish (GitHub Pages)
1. Put these files at the root of a GitHub repository (for example `pubrec-inventory`).
2. In the repository: **Settings → Pages → Build and deployment → Deploy from a branch → `main` / `(root)` → Save**.
3. After a minute the app is live at `https://<your-username>.github.io/pubrec-inventory/`.

## If the web app URL changes
Edit `APP_URL` in `index.html` (one line) and commit.

## Files
- `index.html` — app shell (splash, offline screen, full-screen frame)
- `manifest.webmanifest` — name, colours and icons for installation
- `sw.js` — caches the shell so the app opens offline and shows a clear "you're offline" screen
- `icons/` — app icons made from the PUBReC logo

© 2026 Rodney Omukuti · PUBReC Lab Inventory System
