# DopaDeck

**Pick your energy. Pick your time. Get a thing to do.**

ADHD dopamine menu — no decision fatigue, no overwhelm. One input, one card.

## Run locally
```bash
# Any static server works
python3 -m http.server 8000
# → http://localhost:8000
```

## Deploy (Vercel)
```bash
cd _shared/projects/dopadeck
npx vercel --prod
```
Or connect the repo to Vercel — deploys automatically from this directory.

## Features
- 50+ starter activities across all energy/time combos
- Add/edit/delete your own activities (localStorage)
- Swipe or tap for another card
- Streak tracker (days used)
- PWA — install to home screen, works offline
- Zero backend, zero account, zero tracking

## Stack
- Pure HTML/JS — no framework
- Service worker for offline/PWA
- LocalStorage for all data

## Adding analytics
Drop a Plausible script tag before `</body>`:
```html
<script defer data-domain="yourdomain.com" src="https://plausible.io/js/script.js"></script>
```
