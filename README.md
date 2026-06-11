# Uz-AR Windows — Shahrisabz

An interactive web app showcasing the historical monuments of Shahrisabz, Uzbekistan, with an AR camera view and an interactive map. Available in Uzbek, Russian, and English.

## Features

- **Landing screen** — language switcher (UZ / RU / EN) with quick navigation to AR mode or the map.
- **AR Camera mode** — opens the device camera, overlays animated Timurid-style geometric patterns and a scan frame, shows info about the selected historical site, supports voice narration (text-to-speech) and screenshot capture.
- **Interactive map** — built with Leaflet + OpenStreetMap, shows markers for each site with popups (name, year built, description, UNESCO badge, link to Google Maps).
- **Sites included**:
  - Ak-Saray Palace (1380–1404)
  - Kok Gumbaz Mosque (1435–1436)
  - Dorussaodat Complex (XIV century)

## Tech Stack

- Pure HTML, CSS, and JavaScript (no build step required)
- [Leaflet.js](https://leafletjs.com/) for the map
- Web APIs: `getUserMedia` (camera), `SpeechSynthesis` (voice guide), `Canvas` (AR overlay & screenshots)

## How to Run

Just open `index.html` in a browser. **Note:** camera access requires HTTPS (or `localhost`) — it will not work over a plain `http://` connection on a remote server.

## Deployment

You can deploy this as a static site on:

- **GitHub Pages** — push to a repo, enable Pages in Settings, and it's live at `https://<username>.github.io/<repo>/`.
- **Netlify / Vercel** — drag-and-drop the folder or connect the repo for automatic HTTPS hosting.
- **Any static hosting / shared hosting** — upload `index.html` to the `public_html` (or equivalent) directory.

## Project Structure

```
index.html   # Single-file app: HTML, CSS, and JS all included
```

## Browser Permissions

- **Camera**: required for AR mode — the browser will prompt the user to allow access.
- **Audio**: not required, but Speech Synthesis (voice guide) needs to be supported by the browser.

## License

Add your preferred license here (e.g., MIT).
