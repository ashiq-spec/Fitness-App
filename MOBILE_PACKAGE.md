# Mobile Packaging

This app is now packaged as a PWA.

## Files

- `Fit.html`: the app
- `index.html`: redirects GitHub Pages root to the app
- `manifest.webmanifest`: install metadata
- `icon.svg`, `icon-192.png`, `icon-512.png`, `apple-touch-icon.png`: app icons
- `sw.js`: offline cache

## Install On Phone

Host this folder with HTTPS, open `Fit.html`, then:

- iPhone Safari: Share -> Add to Home Screen
- Android Chrome: menu -> Install app

## Run On GitHub Pages

1. Create a new GitHub repository.
2. Upload these files to the repository root:
   - `index.html`
   - `Fit.html`
   - `manifest.webmanifest`
   - `sw.js`
   - `icon.svg`
   - `icon-192.png`
   - `icon-512.png`
   - `apple-touch-icon.png`
3. Go to GitHub repo `Settings` -> `Pages`.
4. Under `Build and deployment`, choose:
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/root`
5. Save.
6. Open:

```text
https://YOUR-USERNAME.github.io/YOUR-REPO/
```

Then install it from your phone browser.

For local testing on your computer, run:

```sh
python3 -m http.server 8080
```

Then open:

```text
http://localhost:8080/Fit.html
```
