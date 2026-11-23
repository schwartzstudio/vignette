# Vignette

An analog film camera for your phone. Load a film stock, meter the scene, focus with the split image, and shoot. Everything renders live in the viewfinder.

**Try it:** https://schwartzstudio.github.io/vignette/

## Features

- **66 film stocks**, simulated live: 27 color negative, 3 slide and 36 black and white, from Kodak, Fujifilm, Ilford, Harman, Kentmere, Lomography, CineStill, Rollei, Foma, Adox and AgfaPhoto. Each has its own color, contrast, grain, halation and color crossover when under or over exposed.
- **Push and pull:** set the ISO dial away from box speed and contrast and grain change the way they would in the darkroom.
- **Full view finder:** see the whole scene through the lens, with the photo area framed and the rest dimmed around it, in portrait and landscape.
- **Metering:** a center-weighted meter with a needle, aperture priority and manual, plus exposure compensation.
- **Long exposures:** Bulb and timed speeds of 1/8 and slower keep the shutter open for real and average the camera frames, so moving lights streak and still things stay sharp.
- **Focusing screens:** K2 (split image with a microprism collar), B2 (microprism) and E2 (grid).
- **Eight Nikkor primes,** 28mm to 105mm, with real aperture detents, closest focus distances and a depth of field preview.
- **Film and lens details:** the box, recipe and best uses for every stock, and the specs for every lens.
- **Your roll:** a frame counter, a contact sheet of the roll, and a full screen viewer you can swipe through.
- **Saves photos with EXIF data:** date, shutter, aperture, ISO, lens and, if you allow it, location, so Photos files them by when and where.
- Shutter and film wind sounds, which you can turn off.

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
- `lenses/`: lens pictures for the lens menu and lens details
- `sounds/`: shutter release and film wind, recorded from a Nikon FE2
- `apple-touch-icon.png`, `favicon-32.png`, `icon/`: app icons, including the 1024px source

## License

MIT. See [LICENSE](LICENSE). A personal project by Ben Schwartz.
