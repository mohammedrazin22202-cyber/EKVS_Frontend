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
