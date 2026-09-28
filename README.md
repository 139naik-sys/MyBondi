# Spank Meter

A tiny installable web app. Tap "+ Add a mistake" to bump the counter — every 10 rolls up into one "special" spank, so 53 shows as 5 special + 3 normal.

## Files
- `index.html` — the app
- `manifest.json` — makes it installable (PWA)
- `sw.js` — lets it work offline once installed
- `icon-192.png`, `icon-512.png` — app icons

## 1. Put it on GitHub Pages
1. Create a new **public** GitHub repo (e.g. `spank-meter`).
2. Upload all 5 files above to the root of the repo (drag-and-drop on the GitHub web UI works fine).
3. Go to **Settings → Pages**.
4. Under "Build and deployment", set **Source** to "Deploy from a branch", branch `main`, folder `/ (root)`. Save.
5. Wait ~1 minute, then your app is live at:
   `https://<your-username>.github.io/spank-meter/`

## 2. Install it on your phone
**iPhone (Safari):** open the link → tap the Share icon → **Add to Home Screen**.
**Android (Chrome):** open the link → tap the ⋮ menu → **Add to Home screen** / **Install app**.

It'll then open full-screen like a real app, with its own icon.

## Notes
- The count is stored only in the browser/app on that one phone (`localStorage`). It won't sync across devices, and reinstalling or clearing site data will reset it.
- Want it to sync between your phone and his, or want a "reasons" log instead of just a number? Happy to add that.
