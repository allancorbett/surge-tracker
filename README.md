# Surge Tracker — Free & Private Contraction Timer

A **free**, **private**, **offline-first** contraction timer for labour. No accounts. No servers. No tracking. Your data never leaves your device.

## Why Surge Tracker?

Most contraction timer apps harvest your data, require accounts, or bombard you with ads — during one of the most intense experiences of your life. Surge Tracker is different:

- **100% free** — no premium tier, no in-app purchases, no ads
- **100% private** — your data is stored locally in your browser and never sent anywhere
- **No accounts** — nothing to sign up for, just open and start timing
- **No analytics, no cookies, no tracking** — zero third-party scripts
- **Works offline** — install it as a PWA and use it anywhere, even without signal
- **Open source** — read every line of code yourself

## Features

- **One-tap timing** — tap to start a surge, tap again to end it
- **Duration & intervals** — see how long each surge lasts and the gap between them
- **Live stats** — today's count, total count, average interval, average duration
- **Interval chart** — visual plot of intervals over time to spot patterns
- **Add past surges** — manually log surges you didn't track live
- **CSV export/import** — back up or transfer your data
- **Installable PWA** — add to your home screen for a native app feel

## Privacy

No data leaves your device. All surges are stored in your browser's localStorage. There are:

- No servers receiving your data
- No analytics or telemetry
- No cookies
- No third-party scripts
- No accounts or sign-ups

The entire app is a single HTML file you can audit in minutes.

## Tech

Single-file vanilla JS app. Zero dependencies, zero build step, zero bundlers.

| File | Purpose |
|------|---------|
| `index.html` | The entire app — CSS, HTML, and JS in one file |
| `sw.js` | Service worker for offline caching |
| `manifest.json` | PWA manifest |
| `vercel.json` | Vercel static deploy config |
