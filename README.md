# Elanthian Moons

A fully self-contained dashboard for the three DragonRealms moons (Katamba,
Xibar, Yavash), the sun, and the Elanthian calendar. Everything is computed in
the browser from the wall clock -- **no server, no network, no build, no npm.**

Open `index.html` in any browser (double-click, or host it anywhere static). It
works offline.

## What it shows

- Each moon: current phase, above/below horizon, countdown to next rise/set,
  countdown to the next phase, and time to the next full moon.
- Conjunctions: next time all three moons are up together, and all three down.
- Elanthian calendar: date, hour (anlas/rois), named hour, season, year name.
- Sun: up/down, time of day, countdown to next sunrise/sunset.

## How it works

The moon model is deterministic: each moon's period is the game developers'
sidereal orbit (cross-validated against observed rise/set to under a second), and
phase / sun / calendar come from validated constants and lookup tables. Because
it is pure math off the clock, the page is always correct and never needs a data
feed. See the moonwatch technical model doc for the derivation.

Notes:
- Uses the raw model (no per-character self-correction offsets); values are
  accurate to a few seconds, which is invisible on a whole-minute display.
- Moon rise/set timers are quantized to the 60-second server tick, like the game.
- Phase is a computed model value (DR reveals phase only via the `observe` verb,
  which this page does not have; the model has been validated against those
  readings separately).

## Deploying to Cloudflare Pages

No build step. In the Cloudflare dashboard: Pages -> connect this repo (or direct
upload), Framework preset **None**, Build command **empty**, Build output
directory **/** (repo root). It serves `index.html` as-is and redeploys on push.
Nothing is installed on your machine or theirs.

## Regenerating

`index.html` is the shipped artifact and is committed. It is generated from the
validated constants in `moonwatch.lic` so the sun tables and name arrays stay
byte-accurate:

```
python3 generate.py /path/to/moonwatch.lic
```

Only re-run this if the underlying moon/sun constants change (they have not since
DR 0.7.5). `generate.py` is kept for reproducibility; it is not needed to run or
host the page.
