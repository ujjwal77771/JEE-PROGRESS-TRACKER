# JEE Progress Track

[![Status](https://img.shields.io/badge/status-active-brightgreen.svg)]()
[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)]()
[![Built with: Chart.js](https://img.shields.io/badge/Chart.js-v4-orange.svg)]()

**JEE Progress Track** is a single-file, self-contained web application (`update.html`) for tracking JEE-style study progress: daily practice entries (Physics / Maths / Chemistry), week/month analytics, a Codeforces-style heatmap, timelines for class 11/12, and simple local account handling (stored in browser `localStorage`).

---

## 🔎 Project overview

- Single-file web app (HTML/CSS/JS) — no backend required.
- Save per-day scores, visualize trends, and track streaks.
- Codeforces/GitHub-style heatmap covering the last 180 days.
- Register/login using numeric phone ID + SHA-256 hashed password (client-side).
- Export/import account data as JSON.

> **Quick demo**: Save `update.html` and open in Chrome/Firefox/Edge. Use phone `9999999999` + any password for a fast demo and click **Fill Sample**.

---

## ✨ Features

- Single-file (drop-in `update.html`)
- Register / Login (phone + password), auto-login support
- SHA-256 client-side hashing for stored passwords
- Daily input: Physics / Maths / Chemistry (0–100)
- Charts: donut (today), 7-day line, average bar (Chart.js)
- Heatmap (last 180 days) with buckets:
  - `0` → very light
  - `1–49` → **yellow**
  - `50–100` → **green**
  - `101–150` → **purple**
  - `151+` → **red**
- Hover tooltip (date + total + breakdown) and click-to-edit modal
- Timeline for JEE dates per selected grade
- Streak counters (current + longest)
- Export account JSON; fill sample data for demo

---

## ▶️ Quick start

**Open locally (fast):**

1. Download or copy `update.html`.
2. Double-click to open in a modern browser (Chrome/Firefox/Edge recommended).

**Serve via a simple local HTTP server (recommended):**

```bash
# Python 3
python -m http.server 8000
# then open http://localhost:8000/update.html
