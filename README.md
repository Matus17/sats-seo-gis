# SATS-SEO-GIS – základ projektu

Mapa vrcholov Slovenska (MapLibre GL JS + Vite), mapa sa načíta až po kliknutí kvôli LCP.

## Spustenie
```
npm install
npm run dev            # vývoj
npm run build && npm run preview   # produkčný build na :4173
npx playwright install chromium
npm run test:e2e       # Playwright
npm run lhci           # Lighthouse CI (desktop preset, prah 80 %)
```
CI (`.github/workflows/ci.yml`) beží pri push/PR; ťažké testy sa dajú vypnúť pri manuálnom spustení.

## Ďalšie kroky
1. Zmeniť `example.com` v index.html, robots.txt, sitemap.xml
2. PostGIS + OSM trasy, PMTiles
3. Podstránky pre trasy (SEO)
4. PSI API + dashboard
5. Mobilný Lighthouse profil (bonus)

Poznámka: súradnice vrcholov sú približné, over ich.
