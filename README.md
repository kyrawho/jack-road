# The JACK Road

A self-contained interactive map tracing 22 years of family trips (2003–2026) as one
continuous journey across a stylized world map — in the spirit of the Silk Road.

*Jeff · Amy · Carly · Kyra*

## Run locally

From inside this folder:

```bash
python3 -m http.server 8000
```

Then open **http://localhost:8000** in your browser.

(A local server is required — opening `index.html` directly via `file://` will block the
photo/manifest loading in Chrome.)

## What's here

- `index.html` — the entire site (HTML + CSS + JS in one file)
- `manifest.json` — the 22 stops, coordinates, notes, and ordered photo lists
- `photos/<slug>/` — copied trip photos (112 total)
- `.nojekyll` — tells GitHub Pages to serve folders as-is

D3, topojson-client, the world-atlas map data, and fonts load from public CDNs, so an
internet connection is needed the first time it renders. All photo paths are relative,
so the site works correctly under the `/jack-road` subpath on GitHub Pages.

## Deploy to GitHub Pages

See the deploy commands provided in chat. Final URL: https://kyrawho.github.io/jack-road
