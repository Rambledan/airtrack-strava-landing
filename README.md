# AirTrack for Strava — Landing Page

A single static landing page (`index.html`) promoting the AirTrack Strava integration.
Styling (colors, fonts, spacing tokens) was pulled from the live brand site at
[airawarelabs.com/airtrack](https://www.airawarelabs.com/airtrack) as of 2026-07-06:

- Font: **Inter** (Google Fonts)
- CTA orange: `#ff610a`
- Electric blue (headings / Pro accent): `#1a0e9a`
- Clean-air green: `#5b8e3e`
- Body copy gray: `#4a5e72`

## Assets

All placeholders have been replaced with real assets:

| Location | Asset |
|---|---|
| Header logo | `assets/airtrack-logo.svg` |
| Footer logo | `assets/airtrack-logo.svg` (same orange mark, reads fine on the dark footer) |
| Hero (Strava route mockup) | `assets/StraveMockUp.png` |
| "See it in the app" section | `assets/newdashboard.png` |
| App Store / Google Play badges | `assets/app-store-badge.svg`, `assets/play-store-badge.png` |

The footer currently reuses the same orange logo mark rather than a dedicated
white/light variant — swap in a light version in `assets/` and update the
`.brand-logo-footer` reference in `index.html` if one becomes available.

## Run locally

Any static file server works, e.g.:

```bash
python3 -m http.server 4173
```

Then open http://localhost:4173.

## Deploy

Deployed via Vercel as a static site (no build step). Pushing to `main` on GitHub
is connected to auto-deploy on Vercel.
