# Aqua Sense Website

React 19 single-page website for the Aqua Sense water quality monitoring prototype. Built with Vite 8, React Router, Tailwind CSS v4, GSAP/ScrollTrigger, Lenis, and Lucide icons.

## Development

```sh
npm install
npm run dev
npm run lint
npm run build
```

`npm run preview` serves the production build locally. The Vercel rewrite in `vercel.json` routes SPA paths to `index.html`.

## Project structure

- `src/main.jsx` mounts React and `BrowserRouter`.
- `src/App.jsx` defines `/`, `/home`, `/problem`, `/solution`, and `/privacy`, applies route metadata, and initializes Lenis unless reduced motion is requested.
- `src/pages/` contains route-level views.
- `src/components/layout/` contains navigation and footer; `src/components/home/` contains the hero, carousel, problem and solution sections, and project details.
- `src/components/common/` contains shared modals and the error boundary.
- `src/data/content.js` stores major project claims, sensor details, chapter copy, carousel records, and route metadata. Some small interface labels remain in components.
- `public/assets/` contains the logo, river art, news imagery, poster, and five solution videos. The Problem section background video is currently stored at the repository root as `problem video.mp4`.

## Data and backend

This repository is the website frontend only. It does not contain the Arduino/ESP8266 firmware, Flask backend, database, or a connected sensor API. The dashboard-style charts are illustrative; no live readings or verified field dataset are bundled. The intended hardware/data flow shown in the site must not be read as proof of an active integration.

Sensor specifications in `src/data/content.js` refer to manufacturer documentation where available. Calibration results, sampling frequency, field location, team details, and project links remain explicit placeholders until confirmed.

## Configuration and deployment

Set `VITE_SITE_URL` to the canonical production origin when deploying (for example, the actual HTTPS site origin). Without it, route-specific titles and descriptions still update in the SPA, but canonical URLs and absolute social preview URLs are omitted. No analytics or secrets are configured. Review `vercel.json` when changing routes or adding external services; it contains the SPA rewrite and basic response security headers.
