# ED LR Richmond — iPhone web app

This package is an installable Progressive Web App (PWA). It must be served over HTTPS for installation and offline caching; opening `index.html` directly from the Files app does not activate the service worker.

## Fastest deployment

1. Upload this entire folder to a static HTTPS host such as Netlify, Cloudflare Pages, GitHub Pages, or an approved VCU web server.
2. Open the resulting HTTPS URL in Safari on the iPhone.
3. Tap Share → Add to Home Screen.
4. Turn on **Open as Web App**, then tap Add.

## Files

- `index.html`: application
- `manifest.webmanifest`: install metadata
- `service-worker.js`: offline cache
- `icons/`: iPhone and PWA icons

## Updating

Replace the deployed files. Change `CACHE_NAME` in `service-worker.js` when publishing a new release so installed devices refresh the offline cache.

Educational reference only; not validated clinical decision-support software. Verify current VCU and national protocols before clinical use.
