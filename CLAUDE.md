# Contraction Tracker

## Architecture
Single-file vanilla JS PWA. Zero dependencies, zero build step.

- `index.html` — entire app (CSS + HTML + JS in one file)
- `sw.js` — service worker for offline support (network-first caching)
- `manifest.json` — PWA manifest
- `vercel.json` — Vercel static deploy config

## Data Model
`localStorage` key: `"contractions"`
Array of objects: `{ start: ISO8601, end: ISO8601 | null }`
Sorted by `start` ascending.

## Key Functions
- `toggleContraction()` — start/stop a contraction timer
- `render()` — full re-render of stats, log, and chart
- `getContractions()` / `saveContractions()` — localStorage read/write
- `drawChart()` — Canvas 2D scatter plot of intervals over time
- `exportCSV()` / `handleImport()` — CSV import/export

## Conventions
- No frameworks, no npm, no build tools
- All UI in one HTML file with embedded `<style>` and `<script>`
- Mobile-first, touch-optimized
- Purple/lavender color scheme (#7a5ab3 primary)
