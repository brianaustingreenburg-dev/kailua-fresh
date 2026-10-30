# Kailúa Fresh Coffee Kitchen — Menu

Bilingual (ES/EN) QR menu for Kailúa Fresh. A single static page: `index.html`.

- Edit prices or items in the `MENU` list inside `index.html`.
- Every push to `main` redeploys on Vercel automatically, so printed QR codes keep working.
- `print/` holds the 5×7 table card (front: welcome, back: menu + Wi‑Fi QR).

## Offline app
The menu installs as an app (Add to Home Screen) and works with no Wi‑Fi or data after the first visit.
- `manifest.webmanifest` and `icons/`: app name and home-screen icon.
- `sw.js`: keeps the menu on the phone. When you change prices, bump `CACHE` (e.g. `kailua-fresh-v2`) so phones pick up the update next time they're online.
- `fonts/`: fonts are self-hosted so they also work offline.
