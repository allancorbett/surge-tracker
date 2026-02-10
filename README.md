# Surge Tracker

A simple, private PWA for tracking surges (contractions) during labour. No accounts, no servers, no tracking — everything stays on your device.

## Features

- **Start/Stop timer** — tap to begin timing a surge, tap again to end it
- **Duration & intervals** — see how long each surge lasts and the time between them
- **Stats** — today's count, total count, average interval, average duration
- **Interval chart** — visual scatter plot of intervals over time
- **Add past surges** — manually log surges you didn't track live
- **CSV export/import** — back up or transfer your data
- **Offline support** — works without internet once installed
- **Installable PWA** — add to your home screen for a native app experience

## Privacy

No data leaves your device. All surges are stored locally in your browser using localStorage. No analytics, no cookies, no tracking.

## Tech

Single-file vanilla JS app. Zero dependencies, zero build step.

- `index.html` — the entire app (CSS + HTML + JS)
- `sw.js` — service worker for offline caching
- `manifest.json` — PWA manifest
- `vercel.json` — Vercel static deploy config
