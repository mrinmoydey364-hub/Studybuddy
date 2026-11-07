# StudyBuddy PWA starter

This is a small Progressive Web App (PWA) starter built with plain HTML, CSS and JavaScript.

## Run locally
A service worker needs HTTPS or localhost. From this folder run:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000` in your browser.

## Publish on the web / Chrome
1. Upload the contents of this folder to a static HTTPS host (for example GitHub Pages, Cloudflare Pages, or Netlify).
2. Open the HTTPS URL in Chrome.
3. Check that `manifest.webmanifest` and `sw.js` load successfully.
4. Test installability, offline behavior, keyboard use, and mobile layouts on real devices.

## Android / Google Play
A PWA is not automatically a Play Store app. One common route is to publish the PWA at a stable HTTPS URL and use a Trusted Web Activity (TWA), commonly generated with Bubblewrap, or a service such as PWABuilder. Follow current Android and Play Console requirements, configure asset links, sign the Android package, and test it before submitting. Play Store review and developer-account requirements still apply.

## Before using this as a business
This is a prototype, not a finished commercial service. It currently stores tasks and flashcards only in the visitor's browser using localStorage. It has no account system, cloud sync, AI tutor, payment system, analytics, or admin dashboard. Do not promise those features to customers yet.

Before launch:
- Choose a distinct name and check trademark/domain availability.
- Add a privacy policy and support contact that accurately describe the data you collect.
- Test accessibility, security, performance, and data-loss scenarios.
- If adding accounts, AI APIs, or payments, build a secure backend. Never put secret API keys in browser JavaScript.
- Check Google Play's current target API, data safety, content rating, testing, and billing policies.
- If the app is aimed at children, review the applicable child-safety and family policies carefully.

## Project files
- `index.html` — app interface and functionality
- `manifest.webmanifest` — install metadata
- `sw.js` — offline cache
- `icons/` — app icons
