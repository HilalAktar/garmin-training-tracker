# Garmin Antrenman Takip

Personal training dashboard — Garmin activity and wellness data in one page.

**Live:** https://hilalaktar.github.io/garmin-training-tracker/

## What it shows

- **Pano** — daily readiness, training volume by category, form (fitness / fatigue / form), running pace trend
- **Garmin** — sleep score, resting heart rate, HRV, Body Battery, steps, intensity minutes
- **Beceriler** — pole and calisthenics skill progression, flexibility log, fingerboard sessions
- **Hedefler** — goal tracking
- **Motor** — motorcycle rides, kept out of training load on purpose
- **AI Koç** — optional coaching chat (bring your own Google Gemini API key)

## How it works

Single static page, no build step, no backend. `index.html` holds the app;
`data.js` holds the activity and wellness data. Manually entered records
(skills, flexibility, goals) live in the browser's local storage and survive
data refreshes. The Gemini API key, if used, is stored in the browser only and
never leaves it.

## Categories

Training is grouped into eight categories: running, strength, cardio, water
sports, flexibility, pole, climbing, other. Motorcycle rides are tracked but
excluded from training volume and form calculations — they are not training.

Chart colours were validated for colour-vision deficiency; light and dark
themes carry separate, independently checked palettes.

## Licence

Personal project. Data belongs to its owner.
