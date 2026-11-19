# Vignette

An analog film camera for your phone. Load a film stock, meter the scene, focus with the split image, and shoot. Everything renders live in the viewfinder.

**Try it:** https://schwartzstudio.github.io/vignette/

## Features

- 36 film stocks simulated live: color, grain, halation, and exposure-dependent color crossover
- A center-weighted light meter with a needle, plus aperture priority and manual modes
- Split image focusing
- Six manual primes, 28mm to 105mm, with real aperture detents
- Saves photos with EXIF data (film stock, lens, aperture, shutter, location if you allow it)

## Add it to your home screen

Open the link in Safari on iPhone, tap Share, then **Add to Home Screen**. It opens full screen like a regular app, without the browser bar. On Android, use Chrome's **Install app**.

The app needs camera access. Location is optional and only used for photo metadata.

## Running it

It's one `index.html` with no build step. Serve the folder over HTTPS (or `localhost`) so the browser allows camera access:

```
npx serve .
```

## Files

- `index.html`: the whole app
- `manifest.webmanifest`: home screen / install settings
- `sample.jpg`: the sample scene shown on the welcome screen and when no camera is available
- `apple-touch-icon.png`, `favicon-32.png`, `icon/`: app icons, including the 1024px source

## License

MIT. See [LICENSE](LICENSE). A personal project by Ben Schwartz.
