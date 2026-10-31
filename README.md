# Magnets & Magnetism – 3D PWA (Classes 5–6)
Developed by Mateen Yousuf — Teacher

Files: index.html (all code/content), manifest.json, service-worker.js, offline.html, three.min.js (local Three.js), icons/.
No backend, no API key, no CDN. Works offline after the first online visit.

## Run / test locally
Service workers need HTTPS or localhost (NOT file://).
    cd magnet_pwa
    python3 -m http.server 8000
Open http://localhost:8000 in Chrome.

## Deploy
Upload the whole folder to any HTTPS host (GitHub Pages, Netlify, Cloudflare Pages, school server). Keep the files together.

## Install on Android
Open the HTTPS address in Chrome → tap "Install App" in the top bar (or ⋮ menu → Install app / Add to Home screen). iPhone/iPad: Safari → Share → Add to Home Screen.

## Verify offline
Open once online and wait for "Saved for offline use" in Help. DevTools → Application → Service Workers shows it active and Cache Storage shows magnets-v1.0.0. Switch airplane mode on and reopen: the app still works.

## Update
After changing any file, edit VERSION in service-worker.js (e.g. 'v1.0.1'). Users see "A new version is ready – Refresh".

## Controls
Drag magnets/objects; drag empty space to rotate view; scroll/pinch to zoom; Q/E rotate selected magnet; Space pause. 📽 presentation mode; ⚙ reduced graphics.
