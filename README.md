# AirTrack for Strava — Landing Page

A single static landing page (`index.html`) promoting the AirTrack Strava integration.
Styling (colors, fonts, spacing tokens) was pulled from the live brand site at
[airawarelabs.com/airtrack](https://www.airawarelabs.com/airtrack) as of 2026-07-06:

- Font: **Inter** (Google Fonts)
- CTA orange: `#ff610a`
- Electric blue (headings / Pro accent): `#1a0e9a`
- Clean-air green: `#5b8e3e`
- Body copy gray: `#4a5e72`

## Placeholders to replace

Marked with dashed orange boxes / HTML comments in `index.html`. Search for `PLACEHOLDER`:

| Location | What's needed |
|---|---|
| Header (`.brand .logo-slot`) | AirTrack logo mark, ~34×34px SVG/PNG |
| Footer (`.brand .logo-slot`) | Light/white version of the logo for the dark footer background |
| "See it in the app" section (`.shot-placeholder`) | Real product screenshot, 1080×1920 recommended |

Everything else (App Store / Google Play badges, the Strava-compatible mention) already
uses locally-hosted official badge assets in `/assets`.

## Run locally

Any static file server works, e.g.:

```bash
python3 -m http.server 4173
```

Then open http://localhost:4173.

## Deploy

Deployed via Vercel as a static site (no build step). Pushing to `main` on GitHub
is connected to auto-deploy on Vercel.
