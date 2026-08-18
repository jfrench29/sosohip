# Soso & Hip Run 🎀⛳

An endless runner for [sosohip.com](https://sosohip.com). Two sisters — **Soso**
(blonde, pink) and **Hip** (brunette, blue) — sprint down a country-club cart
path, dodging golf balls, startled deer, swooping geese, sprinklers, and
oblivious golfers. Steer between three lanes, jump the ground hazards, duck the
flyers, and collect golden golf balls. How far can they get?

## Play

- **Swipe ◀ ▶ / arrow keys** — steer between lanes
- **Tap / Space / ▲** — jump (hold Space for a higher hop)
- **Swipe ▼ / down arrow** — duck under flying geese (mid-air: fast-fall)
- **P** — pause (also auto-pauses when the tab is hidden)
- Speaker / note chips (or **M**) — mute sound effects and music separately
- Golden balls collected in quick succession build combo multipliers, and every
  ball banks into your all-time stash. Clearing an obstacle in your lane earns
  a near-miss bonus.
- **Power-ups**: shield bubble (absorbs one hit), magnet (pulls gold to you),
  ×2 score, and a springboard super-jump.
- **Daily missions** (three per day) pay bonus gold balls; spend the stash in
  the **STYLE** shop on hats for the sisters — visor, bow, cap, daisy, crown.
- The course cycles through four looks as you run: front nine → back nine →
  sunset → starry night, changing every 1,000 points.
- Works on desktop and phones; on iOS use *Share → Add to Home Screen* for
  fullscreen app mode (plays offline once installed).

## Tech

One self-contained `index.html`: vanilla JS + 2D canvas, faux-3D perspective
projection, WebAudio synth SFX **and a procedural music loop** (no asset files
at all). Obstacles arrive in hand-authored patterns tuned to stay fair. High
score, gold-ball stash, cosmetics, mute prefs, and daily-mission progress
persist in `localStorage`.

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
