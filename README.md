# Preflight Briefing

Offline preflight briefing tool for C-GVOT, C-GVOJ and C-FLCT: airport info, notes, time keeping,
weight and balance, weather, aircraft checks and performance. Print, Print Fold Over (booklet),
Email and Export TXT.

## Files
- `index.html` – the tool
- `sw.js` – service worker so the tool works offline after the first visit
- `manifest.webmanifest`, `icon-*.png`, `apple-touch-icon.png` – home-screen install

## Put it on GitHub Pages
1. Copy this folder into your repo (for example as `preflight-briefing/`, next to your other tools).
2. Commit and push. With Pages already on, it will be at
   `https://<your-user>.github.io/<repo>/preflight-briefing/`.
3. Open that link on the iPad once while online, then Share → Add to Home Screen.

## Updating
After changing `index.html`, edit `VERSION` in `sw.js` (for example `preflight-v2`) so devices
refresh their offline copy.

## Things to test
- **METAR paste** (Weather): pasting a METAR auto-fills winds, altimeter and OAT.
- **Print** and **Print Fold Over**: Fold Over prints double-sided, flip on short edge, then fold on
  the dashed line with the airport page outside.
- **Email** opens your mail app with the briefing text; **Export TXT** saves it as a file.

Planning aid only. Confirm weights, limits and performance against the aircraft documents and POH/AFM.
