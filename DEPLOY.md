# Portfolio Dashboard Static Deploy

This folder is the static deploy package for GitHub Pages or Cloudflare Pages.

## Files to publish

Upload or commit everything in this folder:

- `index.html`
- `portfolio-dashboard.html`
- `portfolio-config.js`
- `manifest.json`
- `service-worker.js`
- `portfolio-icon.svg`

## Google Sheets settings

The dashboard can work in two ways:

1. Recommended for privacy: leave `portfolio-config.js` blank and enter the Apps Script Web App URL and Google Sheet ID from the dashboard Settings screen on each device once.
2. Easier but less private: put the Apps Script Web App URL and Google Sheet ID directly in `portfolio-config.js` before publishing.

If the site is public, anyone who can open the published dashboard may be able to use the configured sheet sync endpoint.

## Notes

- PWA install works on HTTPS. GitHub Pages and Cloudflare Pages both provide HTTPS.
- Offline mode shows the last cached dashboard and the last local browser data.
- Naver market refresh may be limited on static hosting because there is no local `/api` proxy. Google Sheets sync is still available.
