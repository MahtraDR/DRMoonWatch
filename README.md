# DRMoonWatch

A single self-contained page for the DragonRealms moons (Katamba, Xibar,
Yavash), the sun, and the Elanthian calendar. It includes a sky view that shows
each moon (and the sun) on its arc across the horizon - rising in the east,
climbing to zenith, setting in the west, dimly tracked below the horizon - each
drawn with its current phase, so you can see the trajectories at a glance.

**Open `index.html` in any browser. That is the entire thing.** No server, no
build, no dependencies, no external requests. It computes everything live from
the clock and works offline.

`index.html` is the whole project - one file, hand-contained (HTML + CSS +
JavaScript model, all inline). Nothing else is required to run or host it. To
deploy, drop it on any static host (e.g. Cloudflare Pages: framework preset
None, no build command).
