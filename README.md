# DisciplineOS 🏋️

> A daily discipline tracker PWA — built for champions.

Dark-themed, mobile-first Progressive Web App for tracking your daily habits: meals, gym, and steps.

---

## Features

- **Meal Tracker** — Log 5 meals with protein grams. Visual progress bar vs. your daily goal.
- **Workout Tracker** — One-tap toggle with workout type (Push/Pull/Legs/Cardio/Rest) + streak counter.
- **Steps Tracker** — Circular progress ring with color states (red → yellow → green).
- **Daily Score** — 0–100% composite score across all three trackers.
- **History** — Last 7 days at a glance.
- **Settings** — Custom name, protein goal, step goal.
- **PWA** — Installable, offline-capable, full-screen standalone mode.
- **Midnight Auto-Reset** — All daily data resets at midnight automatically.

## Stack

- Vanilla HTML + CSS + JS (single `index.html`)
- `localStorage` for persistence
- `manifest.json` + `sw.js` for PWA/offline

## Run Locally

```bash
# Any static server works — e.g.:
npx serve .
# or
python -m http.server 8080
```

Then open `http://localhost:8080` and tap "Add to Home Screen" on mobile.

## File Structure

```
disciplineos/
├── index.html        ← Full app (HTML + CSS + JS)
├── manifest.json     ← PWA manifest
├── sw.js             ← Service worker (offline caching)
├── icons/            ← App icons (72–512px)
└── README.md
```

## Color Palette

| Token | Value | Use |
|---|---|---|
| `--bg` | `#0a0a0a` | App background |
| `--card` | `#1a1a1a` | Card surfaces |
| `--accent` | `#6c63ff` | Primary purple |
| `--accent2` | `#00ff88` | Success green |
| `--warn` | `#ffa502` | Warning amber |
| `--danger` | `#ff4757` | Danger red |

---

Built with discipline. For the disciplined.
