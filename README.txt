EBON HOLLOW — PERSONAL GAME LIBRARY
====================================

WHAT'S INCLUDED
- index.html: the responsive library interface and a tiny built-in supernatural story
- manifest.webmanifest: installable web app metadata
- sw.js: service worker for caching the library shell for offline launch
- icon.svg: app icon artwork drawn in SVG

IMPORTANT IPHONE OFFLINE NOTES
1. A PWA must first be served from a secure HTTPS website for service workers to work.
2. Open the hosted site in Safari on your iPhone while online.
3. Use Safari's Share menu > Add to Home Screen. If offered, enable "Open as Web App".
4. Open the installed app once while online and wait for it to finish loading.
5. Then test by enabling Airplane Mode and reopening it.
6. The library's entries and favorites are saved in local storage on that iPhone. Clearing Safari website data or uninstalling/resetting the web app may remove them. Keep a separate record of important entries.

FREE HOSTING OPTION: GITHUB PAGES
1. Sign in to GitHub and create a new public repository, e.g. ebon-hollow.
2. Upload index.html, manifest.webmanifest, sw.js, and icon.svg to the repository root.
3. In the repository, open Settings > Pages.
4. Under Build and deployment, choose Deploy from a branch, select the main branch and /(root), then Save.
5. Wait for GitHub Pages to publish the site. Its URL will look like https://YOUR-USERNAME.github.io/ebon-hollow/
6. Open that exact URL in Safari on your iPhone and follow the install steps above.

This is a static starter project; it is not published yet. The files cannot prevent an initial 404 if the host URL is wrong or the host is unavailable. Once the service worker has successfully cached the app, the library shell should launch offline on that device. Test before relying on it.

ADDING GAMES
- Use the "+ Add a game" button in the library to create a card.
- A web URL can launch another game, but that other game may require internet and may have its own 404 risk.
- For reliable offline individual games, each game's assets and code need to be included in the app's offline cache or hosted as its own offline-capable PWA. We'll build each game with this in mind.
- The sample "The Lantern in the Attic" is included and runs locally.

PRIVACY
The starter library does not use accounts, analytics, or a server-side database. Your collection is stored in the browser storage on your device.
