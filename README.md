# Knee Recovery Tracker

A personal PWA for tracking recovery after knee replacement surgery. Installable on iPhone or Android via the browser — no app store needed.

**Surgery date: May 5, 2026**

---

## Features

- **Daily log** — pain level (0–10), flexion & extension range of motion, step count, walking aid, exercises, swelling, and notes
- **PT & appointments** — log upcoming and past physical therapy and surgeon appointments
- **Ice & elevation** — customizable reminder schedules with a live today view showing what's done, next up, and upcoming
- **History** — scrollable log of past entries with pain, flexion, and step count at a glance
- **Milestones** — recovery goals that auto-complete when your logs hit the target (90°, 110°, 120° flexion, walking without aids, etc.)
- **Summary** — charts for flexion progress and pain trend over the last 7 days
- **Data tab** — export logs and appointments as CSV, import CSV, full JSON backup, and a 7-day backup reminder banner

---

## Installation

### iPhone (Safari)
1. Open the app URL in Safari
2. Tap the **Share** button
3. Tap **Add to Home Screen**
4. Tap **Add**

### Android (Chrome)
1. Open the app URL in Chrome
2. Tap the three-dot menu
3. Tap **Add to Home Screen**

Once installed, the app works offline.

---

## Deployment

This is a single-file PWA — everything is in `index.html`.

1. Fork or clone this repo
2. Enable GitHub Pages: **Settings → Pages → Source: main branch**
3. Your app will be live at `https://yourusername.github.io/knee-recovery`

---

## Data & privacy

All data is stored locally on your device using `localStorage`. Nothing is sent to any server. Clearing your browser data will erase your logs — use the **Data → Export** feature regularly to keep a CSV backup.

The app shows a reminder banner if it has been 7 or more days since your last export.

---

## Tech

Plain HTML, CSS, and vanilla JavaScript. No frameworks, no dependencies, no build step. Includes an inline PWA manifest and service worker for offline support.
