# Soso & Hip Run 🎀⛳

An endless runner for [sosohip.com](https://sosohip.com). Two sisters — **Soso**
(blonde, pink) and **Hip** (brunette, blue) — sprint down a country-club cart
path, hopping golf balls, startled deer, geese, sprinklers, and oblivious
golfers. Collect golden golf balls for bonus points. How far can they get?

## Play

- **Space / tap** — jump (hold for a higher hop)
- **P** — pause (also auto-pauses when the tab is hidden)
- **M** or the speaker button — mute
- Collect golden balls in quick succession for combo multipliers; clearing an
  obstacle by jumping earns a +10 near-miss bonus.
- Works on desktop and phones; on iOS use *Share → Add to Home Screen* for
  fullscreen app mode (plays offline once installed).

## Tech

One self-contained `index.html`: vanilla JS + 2D canvas, faux-3D perspective
projection, WebAudio synth SFX (no asset files at all). High score persists in
`localStorage`.

- `manifest.webmanifest` + icons — PWA / home-screen support
- `sw.js` — service worker: offline play, network-first page loads
- `CNAME` — custom domain for GitHub Pages

## Develop

No build step. Open `index.html` in a browser, or:

```sh
python3 -m http.server 8123
```

## Deploy

Pushing to `main` redeploys GitHub Pages automatically.
