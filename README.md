# Marque — Brand Intelligence Studio

Audit, score and level up any brand. Runs entirely in the browser; installable as a PWA; works offline.

## Deploy to GitHub Pages
1. Create a new public repository (e.g. `marque`).
2. Upload **all** files from this folder to the repository root (keep them together):
   `index.html`, `sw.js`, `manifest.webmanifest`, `icon-192.png`, `icon-512.png`, `icon-maskable-512.png`, `apple-touch-icon.png`
3. Repository → Settings → Pages → Source: *Deploy from a branch* → Branch: `main`, folder `/ (root)` → Save.
4. After a minute your app is live at `https://<your-username>.github.io/marque/`.

## Updating
Edit `index.html`, then in `sw.js` change `VERSION = 'marque-v1.0.0'` to a new value (e.g. `v1.0.1`).
Visitors see a "new version is ready — Reload" message.

## Notes
- `index.html` contains the whole app. `sw.js` and `manifest.webmanifest` must be separate files — browsers require that for installing and offline use.
- Optional AI assist (Claude / OpenAI / Gemini) uses your own API key. **API keys are sensitive**: the key is stored only in that browser's local storage and sent directly to the provider. Use a key with a spending limit.
- Website text is read through the public reader `r.jina.ai` (can be switched off in Settings).
