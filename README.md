<p align="center">
  <img src="icons/logo.png" alt="PUBReC — Pwani University Biosciences Research Centre" width="360">
</p>

<h1 align="center">PUBReC Lab Inventory</h1>

<p align="center">
  The lab inventory for every research group at the Pwani University Biosciences Research Centre.<br>
  <b><a href="https://rodneyomukuti.github.io/pubrec-inventory/">Open the app →</a></b>
</p>

---

## What it does

- **Stock:** store and pick supplies for your group or from PUBReC's shared stock. When you pick, the lot that expires soonest is used first.
- **Alerts:** shows items that are running low or close to expiry.
- **Research projects:** link each pick to a grant or sub-project so use can be reported per project.
- **Cold chain:** a daily temperature log for the fridges (4–8 °C), the −20 °C freezers and the −80 °C freezers.
- **Reports:** monthly, quarterly and yearly reports for each group, plus the PUBReC Lab Analytical Plan (PLAP).

All data lives in PUBReC's Google Sheet. This repository holds only the installable app wrapper: it opens the live system full-screen, with the PUBReC icon.

## Install it

Install from this link on every device: **https://rodneyomukuti.github.io/pubrec-inventory/**

| Device | Steps |
|---|---|
| **Windows or Mac: Chrome** | Open the link → click the **install icon** at the right of the address bar (or **⋮ → Cast, save and share → Install page as app**) → **Install**. |
| **Windows or Mac: Edge** | Open the link → **⋯ → Apps → Install this site as an app** → **Install**. |
| **Mac: Safari** (macOS Sonoma or newer) | Open the link → **File → Add to Dock** → **Add**. |
| **Android** | Open the link in **Chrome** → tap **Install app** (or **⋮ → Add to Home screen**). |
| **iPhone or iPad** | Open the link in **Safari** → **Share** → **Add to Home Screen** → **Add**. |

To pin it: on Windows, right-click the app's taskbar icon → **Pin to taskbar**. On a Mac, right-click its Dock icon → **Options → Keep in Dock**.

## Sign in

1. Enter the email you use with the lab and choose **Email me a code**.
2. Enter the 6-digit code sent from **pubrec@pu.ac.ke**.
3. Under **My account**, set a password. Next time, sign in with your email and password.

New to the lab? Choose **Request access** on the sign-in screen. Your PI or the lab admin approves you.

## Good to know

- **Updates are automatic.** Installed apps always open the latest version. Nobody needs to reinstall.
- **Internet is needed.** Without a connection, the app shows a "you're offline" screen and a **Try again** button.
- **"Sorry, unable to open the file":** this comes from Google when a browser is signed in to several Google accounts. The app already uses the address that avoids it. If you still see it, open the app in a browser profile with only one Google account, or in Edge.

## For maintainers

| File | Purpose |
|---|---|
| `index.html` | App shell: splash screen, offline screen and a full-screen frame for the web app. `APP_URL` holds the live Apps Script address. |
| `manifest.webmanifest` | App name, colours and icons used when installing. |
| `sw.js` | Caches the shell only. Stock data always comes live from the web app. |
| `icons/` | Icons made from the PUBReC logo. |

**If the web app address changes:** edit the single `APP_URL` line in `index.html` and commit. Keep the `/a/macros/pu.ac.ke/` form of the address.

GitHub Pages publishes from `main` / root (**Settings → Pages**).

---

<p align="center"><sub>© 2026 Rodney Omukuti · PUBReC Lab Inventory System</sub></p>
