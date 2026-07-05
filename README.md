# Soso & Hip Run 🎀⛳

An endless runner for [sosohip.com](https://sosohip.com). Two sisters — **Soso**
(blonde, pink) and **Hip** (brunette, blue) — sprint down a country-club cart
path, hopping golf balls, startled deer, geese, sprinklers, and oblivious
golfers. Collect golden golf balls for bonus points. How far can they get?

## Play

- **Space / tap** — jump (hold for a higher hop)
- Works on desktop and phones; on iOS use *Share → Add to Home Screen* for
  fullscreen app mode.

## Tech

One self-contained `index.html`: vanilla JS + 2D canvas, faux-3D perspective
projection, WebAudio synth SFX (no asset files at all). High score persists in
`localStorage`.

- `manifest.webmanifest` + icons — PWA / home-screen support
- `CNAME` — custom domain for GitHub Pages

## Develop

No build step. Open `index.html` in a browser, or:

```sh
python3 -m http.server 8123
```

## Deploy

Pushing to `main` redeploys GitHub Pages automatically.
