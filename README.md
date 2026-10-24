# GBoS GEOAI — Urban Travel Time & Intelligent Routing

An interactive web mapping research prototype for The Gambia.

## Files
- `index.html` — complete single-file web application (Leaflet 2D map, CesiumJS 3D globe, Chart.js charts and CSV exports).
- `README.md` — this guide.
- `LICENSE.txt` — project reuse note and third-party attribution reminder.

## Run locally
1. Extract the ZIP.
2. Open `index.html` in a modern browser while connected to the internet.
3. For GPS support, serve the folder from `localhost` (for example, VS Code Live Server) or use HTTPS.

The application loads Leaflet, CesiumJS and Chart.js from public CDNs and requests routing from public OSRM-compatible services. Internet access is required; public services may be rate-limited.

## Publish with GitHub Pages
1. Upload `index.html`, `README.md`, and `LICENSE.txt` to the root of your GitHub repository.
2. Open repository **Settings → Pages**.
3. Choose **Deploy from a branch**, branch `main`, folder `/ (root)`, then save.
4. Wait for the deployment to finish and open the URL GitHub Pages displays.

## Important limitations
- The 3D view is a globe visualization; this package does not include a local terrain dataset.
- Travel-time scenarios are browser-side sensitivity assumptions, not live traffic.
- LSTM/GNN selectors document a proposed model design. No trained neural network is included.
- Confirm routing results and coordinate quality locally before operational use.
- Follow OpenStreetMap and other tile/provider terms and attribution requirements.
