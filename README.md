# 🏁 Pro Race Timer Suite

A complete web‑based race timing system with:

- **Control Center** — manage setup, roster, race flow, crossings, results, and Supabase sync.
- **Tracker** — lightweight mobile page for runners to share live GPS during the race.
- **Viewer** — public leaderboard with live map, filters, and runner detail drawer.

Built for real‑world running events where accuracy, clarity, and live sharing matter.

---

## ✨ Features

### Control Center
- Setup race name, lap distance, total laps, teams mode, and start sound.
- Randomized start delay with audio cue.
- Roster management: add/edit/delete, CSV/JSON import/export, duplicate bib guard.
- Race flow: start, pause, resume, end, reset.
- Crossing queue: log crossings in sequence, assign bibs later.
- Leaderboard: laps, last lap, averages, finish toggle, DQ toggle.
- Supabase integration: event log + runner_state snapshot, hash‑encoded viewer link generator.
- Local autosave/restore of config and state.

### Tracker
- Mobile‑friendly page for runners.
- Enter bib number and share GPS via `navigator.geolocation`.
- Sends `location` events to Supabase while race is running.
- Start/stop buttons with live log.

### Viewer
- Live leaderboard from Supabase `runner_state`.
- Interactive map (Leaflet) with course polyline and runner markers.
- Filters: search, team filter, show/hide finished or DQ, sort options.
- Runner selection for map (all, none, or specific bibs).
- Runner detail drawer: metrics, lap history (from `race_events`), latest location.
- Auto‑refresh with pause/resume.
- Responsive design for desktop and mobile.

---