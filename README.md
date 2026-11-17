# BEDC Substation Logbook PWA

## Deploy to GitHub Pages

1. Create or open a GitHub repository.
2. Upload **all files and folders in this package** to the repository root. Keep `index.html`, `manifest.webmanifest`, and `service-worker.js` together.
3. Commit the files to the branch you want to publish.
4. Open **Settings → Pages** in the repository.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select your publishing branch (usually `main`) and folder `/ (root)`, then save.
7. Wait for GitHub Pages to publish the site. Open the published HTTPS URL in Chrome.
8. In Chrome, use **Install app** or **Add to Home screen**.

## Included

- `index.html`: the supplied application with PWA metadata added. Existing app layout, styles, controls and application logic are retained.
- `manifest.webmanifest`: install name, display mode, scope and icon declarations.
- `service-worker.js`: app-shell caching for offline launch after the first successful visit.
- `icon-192.png`, `icon-512.png`, `apple-touch-icon.png`: resized versions of the supplied icon artwork.

## Data storage

The application continues to use the browser's local storage as implemented in the original HTML. Records remain on the device/browser profile. Use the app's Backup and Restore page before changing devices or clearing browser data.

## Important

- GitHub Pages must serve the app over HTTPS for PWA installation and service-worker features.
- Do not open `index.html` directly as a local file. Test through the GitHub Pages URL or a local HTTP server.
- Keep the repository path and the app files together at the published root. The relative URLs in this package also support a GitHub Pages project site.
