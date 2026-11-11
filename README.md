# Bandung Family Trip Planner

A mobile-first, editable Bandung travel dashboard for 22–27 November 2026.

## Files
- `index.html` — complete app
- `manifest.json` — Add to Home Screen / PWA metadata
- `sw.js` — offline app-shell caching
- Settings include light/dark/system theme, undo/redo history and reset-to-original-plan
- `icon-192.png`, `icon-512.png` — app icons

## Publish with GitHub Pages
1. Sign in or create a free account at https://github.com/
2. Create a **public** repository named `bandung-trip` (or another name).
3. Upload all files in this folder to the repository root. Keep the filenames unchanged.
4. Open repository **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Choose branch **main**, folder **/(root)**, then Save.
7. Wait for the Pages deployment to finish. Your URL will look like:
   `https://YOUR-USERNAME.github.io/bandung-trip/`
8. Open that URL in Safari on your iPhone. Tap **Share → Add to Home Screen**.

## Data and offline behaviour
- Edits autosave in local browser storage on the current device.
- Use **Export backup** regularly to save a JSON copy in Files/iCloud Drive.
- Use **Import backup** to restore it in this browser.
- The service worker caches the app shell after the first successful online visit. Open the site once while online before relying on offline access.
- The live SGD/IDR refresh requires internet. The saved/manual rate and converter remain usable offline.
- Local browser data does not sync between devices. Export/import is the way to move your plan.

## Important
This app is a planning tool, not a booking system. Check flight, hotel, transport, opening-hour, child-fare and payment details against providers before travelling. The exchange rate shown initially is an editable placeholder estimate; refresh it online before using it for actual conversions.

## v3 update
- Overview now reads flight and accommodation details from the same shared trip data as the editable tabs.
- Added explicit Save Changes button (autosave remains enabled).
- Added Settings with light/dark/system theme, undo/redo, and reset-to-original-plan.
- Improved iPhone safe-area spacing for the top camera/status area.
