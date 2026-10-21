# 🎨 EKVS Food Decider — Frontend

Static web application frontend for EKVS Food Decider, ready for Vercel deployment.

## 🚀 Connecting to Backend

By default, the app attempts to reach the backend at:
1. `window.API_BASE_URL` (configured in `config.js`)
2. `localStorage.getItem("API_BASE_URL")` (configurable directly in the UI footer)
3. `http://localhost:8000` (when running locally)

To point to your hosted Render backend (e.g. `https://ekvs-backend.onrender.com`):
- Edit `config.js` and set `window.API_BASE_URL = "https://ekvs-backend.onrender.com";`, OR
- Open the app in your browser, click on the **⚙️ Server** pill in the bottom right corner, and paste your Render URL.

---

## ☁️ Deploying to Vercel

1. Create a new Git repository from this `frontend` folder and push to GitHub/GitLab.
2. In Vercel Dashboard (`vercel.com`), click **Add New** -> **Project**.
3. Import your frontend Git repository.
4. Framework Preset: **Other** (Static Site).
5. Build and Output Settings: Leave defaults (Root directory contains `index.html`).
6. Click **Deploy**!

Your frontend will be instantly live on a fast global Vercel CDN URL (e.g., `https://ekvs-food-decider.vercel.app`).

---

## ✨ Features Highlight

- **Top-Right Live Clock HUD:** Real-time digital clock updating every second, with quick click/keyboard toggle between 12-hour (AM/PM) and 24-hour formats, current date display, and minimizable neo-brutalist widget design.
- **300+ Curated Hourly Slogans:** Rotating collection of 330 unique, witty food & meal decision slogans synchronized to the epoch hour, complete with a live countdown timer until the next rotation, interactive peek/shuffle (`🎲`) controls, and accessible `aria-live` screen-reader support.
- **Offline PWA & Service Worker Caching:** Fully progressive web app with pre-cached slogans, offline assets, and app manifest for homescreen installation.
- **Retro Synth Audio FX:** Dynamically synthesized retro sound effects using the Web Audio API for interactive clicks, rolling reels, and successes.
- **Local User Profiles:** Manage user dining profiles directly in the browser using `localStorage`.
- **Group Dining Polls:** Real-time synchronized room polls using MongoDB backend connection.

