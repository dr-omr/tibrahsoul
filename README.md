# Tibrahsoul – Vercel Migration

This project is now Vercel-ready! Deploy your Arabic-language multidimensional healing dashboard with one click.

---

## 🚀 Quick Deploy (Recommended)
1. **Push to GitHub** (or connect your repo to Vercel)
2. Go to [vercel.com/import](https://vercel.com/import) and select your repo
3. Vercel auto-detects the config (`vercel.json`)
4. Deploy! (Free plan is enough)

---

## 📁 Project Structure
- `/api/` — All backend logic (converted from Firebase Functions)
- `/js/` — Frontend scripts (dashboard, views, logic)
- `/dashboard.html` — Main SPA dashboard (RTL Arabic)
- `/style.css` — Styles (RTL, Arabic)
- `/functions/` — Legacy Firebase code (for reference)

---

## 🛠️ Development & Local Testing
- Install [Vercel CLI](https://vercel.com/download):
  ```sh
  npm i -g vercel
  ```
- Run locally:
  ```sh
  vercel dev
  ```
- Visit [http://localhost:3000/dashboard](http://localhost:3000/dashboard)

---

## 🔗 Firestore Integration
- **Live:** For production, you can connect Firestore by installing `firebase-admin` and using service credentials in `/api/` routes.
- **Demo/Local:** By default, the backend uses a mock in-memory DB for signals/entries. See `/api/signals.js`, `/api/analyzeEntry.js`.

---

## 📝 API Endpoints
- `POST /api/analyzeEntry` — Analyze a new entry (returns signals)
- `POST /api/patternResonanceNightly` — Run pattern engine for a user
- `GET /api/signals` — List all signals (mock)

---

## 🌍 RTL & Arabic Support
- All UI and dashboard content is RTL and Arabic by default.

---

## 🧑‍💻 Prerequisites
- Node.js 18+
- [Vercel CLI](https://vercel.com/download) (for local dev)
- (Optional) Firebase Admin SDK for Firestore integration

---

## 📦 One-Click Deploy
[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/import/project?template=github.com/YOUR_GITHUB_USERNAME/tibrahsoul)

---

## Questions?
Open an issue or ping @YOUR_GITHUB_USERNAME
