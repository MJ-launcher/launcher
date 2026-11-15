# MJLauncher

A Progressive Web App (PWA): the MJ launcher with 15 game versions, fully
offline-capable once installed. Install it from any static host and it behaves
like a native app with its own icon and window.

## What's inside

| File | Purpose |
| --- | --- |
| `index.html` | The MJ launcher (Mojolauncher edition) — self-contained |
| `manifest.webmanifest` | PWA manifest — name "MJLauncher", icons, standalone display |
| `sw.js` | Service worker — caches the launcher + all games for offline play |
| `apple-touch-icon.png` | Home-screen icon for iOS (auto-discovered at the root) |
| `icons/` | App icons: 192/512 px, maskable variants, Apple touch icon |
| `*.html` | The 15 game versions (Latest release 26.3 … release 1) |

## Run it locally

Needs a local web server (service workers do not work from `file://`):

    python3 -m http.server 8000

then open http://localhost:8000

## Host it

Upload the contents of this folder to any static host:

- GitHub Pages
- Netlify Drop (drag & drop)
- Cloudflare Pages
- Vercel

## Install as an app

- **iOS (Safari):** Share → *Add to Home Screen* — the MJ monogram icon
  appears on the home screen and the app opens full-screen.
- **Android (Chrome):** menu → *Add to Home screen* / *Install app*.
- **Chrome / Edge (desktop):** click the install icon in the address bar, or
  menu → *Install MJLauncher*.

After the first load, the launcher and all games work completely offline.

## The launcher

Dark teal MJ launcher with an instances home screen: create, duplicate and
edit instances, pick any of the 15 versions, change your username and
renderer, and press PLAY — the game opens in a new window. Everything
(instances, username, settings) is saved in the browser.
