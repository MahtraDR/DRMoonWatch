<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>DRMoonWatch - Documentation</title>
<style>
  :root {
    --bg: #0b0d1a; --panel: #151830; --panel2: #1d2142;
    --ink: #e9e9f2; --dim: #9aa0c0; --accent: #b9a6ff;
    --katamba: #cbb6ff; --xibar: #9fc4e8; --yavash: #f0917f;
    --line: #262b52;
  }
  * { box-sizing: border-box; }
  body {
    margin: 0; background:
      radial-gradient(1200px 600px at 70% -10%, #1a1f45 0%, transparent 60%),
      var(--bg);
    color: var(--ink);
    font: 16px/1.65 -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
    min-height: 100vh; padding: 24px;
  }
  .wrap { max-width: 820px; margin: 0 auto; }
  h1 { font-weight: 600; font-size: 30px; margin: 0 0 4px; letter-spacing: .5px; }
  h2 {
    font-weight: 600; font-size: 20px; margin: 40px 0 12px;
    padding-bottom: 8px; border-bottom: 1px solid var(--line);
  }
  h3 { font-weight: 600; font-size: 16px; margin: 24px 0 8px; }
  .lede { color: var(--dim); font-size: 15px; margin-bottom: 8px; }
  a { color: var(--accent); }
  p { margin: 10px 0; }
  ul, ol { margin: 10px 0; padding-left: 22px; }
  li { margin: 5px 0; }
  code {
    background: #11142a; padding: 1px 6px; border-radius: 4px;
    color: #c8cdf5; font-size: .9em;
  }
  pre {
    background: #0c0f22; border: 1px solid var(--line); border-radius: 10px;
    padding: 14px 16px; overflow-x: auto; margin: 14px 0;
  }
  pre code { background: none; padding: 0; color: #c8cdf5; }
  .panel {
    background: var(--panel); border: 1px solid var(--line);
    border-radius: 12px; padding: 16px 20px; margin: 16px 0;
  }
  .kat { color: var(--katamba); font-weight: 600; }
  .xib { color: var(--xibar); font-weight: 600; }
  .yav { color: var(--yavash); font-weight: 600; }
  table { border-collapse: collapse; width: 100%; margin: 14px 0; font-size: 14px; }
  th, td { text-align: left; padding: 8px 12px; border-bottom: 1px solid var(--line); }
  th { color: var(--dim); font-weight: 600; text-transform: uppercase; letter-spacing: .06em; font-size: 12px; }
  .foot { margin-top: 44px; color: var(--dim); font-size: 13px; border-top: 1px solid var(--line); padding-top: 16px; }
  .back { display: inline-block; margin-bottom: 20px; font-size: 14px; }
</style>
</head>
<body>
<div class="wrap">

  <a class="back" href="/">&larr; Back to the dashboard</a>
  <h1>DRMoonWatch</h1>
  <p class="lede">
    A single self-contained page that tracks the three DragonRealms moons
    (<span class="kat">Katamba</span>, <span class="xib">Xibar</span>,
    <span class="yav">Yavash</span>), the sun, and the Elanthian calendar -
    computed live in your browser from the wall clock, with no server and no
    network.
  </p>

  <h2>What it shows</h2>
  <ul>
    <li><strong>The Elanthian date and time</strong> - year, month, day, anlas
      (hour) and roisaen (minute), plus the season, the named year in the
      seven-year cycle, and the descriptive time of day.</li>
    <li><strong>The sun</strong> - whether it is up or down, the current time of
      day, and a countdown to the next sunrise or sunset.</li>
    <li><strong>The sky now</strong> - a live diagram of the sun and all three
      moons on their arcs across the horizon, each drawn at its current phase.</li>
    <li><strong>Per-moon cards</strong> - current phase (with an illustrated
      disc), whether the moon is above or below the horizon, the countdown to its
      next rise or set, the countdown to its next phase change, and the time until
      it is next full.</li>
    <li><strong>Conjunctions</strong> - the next window in which all three moons
      are above the horizon at once, and the next window in which all three are
      below it.</li>
  </ul>

  <h2>The sky view</h2>
  <p>
    The sky diagram places each body on an arc: rising at one horizon, climbing to
    the zenith, and setting at the opposite horizon. Below the horizon a body
    continues along a shallow dipped arc so you can follow its full trajectory.
    Each moon is drawn as a small disc showing its current phase, with a curved
    terminator - waxing moons are lit on one side, waning on the other.
  </p>
  <h3>Facing north or south</h3>
  <p>
    The <strong>facing north</strong> checkbox flips the orientation. Facing north
    (the default) puts <strong>east on the right</strong> and west on the left, so
    the sun and moons travel right to left - the view you get looking up while
    facing north. Unchecking it faces you south, mirroring the sky so bodies
    travel left to right. Only the diagram is mirrored; the underlying times and
    positions are identical either way.
  </p>
  <h3>Below the horizon</h3>
  <p>
    Bodies below the horizon are drawn in the dark night band beneath the horizon
    line. To keep the darker moons legible there, below-horizon discs are lifted
    toward white and ringed with a dotted outline, rather than simply dimmed. The
    horizon itself is the solid line across the middle, and the faint dashed arc
    above it traces the daytime sky.
  </p>

  <h2>The model</h2>
  <p>
    Everything is derived from a single Unix timestamp - the current wall-clock
    time. There is no stored state, no calibration, and no randomness; given the
    same instant the page always computes the same result.
  </p>

  <h3>The moons</h3>
  <p>
    Each moon is defined by a small set of constants: an epoch (a known reference
    time), the length of its rise-to-rise cycle, how long it stays above the
    horizon within that cycle, and its sidereal period (used for the phase). The
    moon periods are the game developers' sidereal orbits, cross-validated against
    observation to under a second.
  </p>
  <table>
    <tr><th>Moon</th><th>Colour</th><th>Character</th></tr>
    <tr><td class="kat">Katamba</td><td>Black</td><td>The dark moon - deepest and hardest to spot.</td></tr>
    <tr><td class="xib">Xibar</td><td>Blue</td><td>The blue moon.</td></tr>
    <tr><td class="yav">Yavash</td><td>Red</td><td>The red moon.</td></tr>
  </table>
  <p>
    Horizon state is found by measuring how far the moon is through its current
    cycle: if that offset is less than the visible span the moon is up, otherwise
    it is down. Rise and set countdowns are the time to the next such boundary,
    quantized to the game's 60-second server tick.
  </p>

  <h3>Phases</h3>
  <p>
    Phase is computed from each moon's sidereal period combined with the day of
    the year, and reported as one of the eight standard phases:
  </p>
  <p>
    new &middot; waxing crescent &middot; first quarter &middot; waxing gibbous
    &middot; full &middot; waning gibbous &middot; third quarter &middot; waning
    crescent
  </p>
  <p>
    The disc illustration reflects the illuminated fraction and the direction of
    the terminator, so a waxing gibbous and a waning gibbous of the same
    illumination are drawn as mirror images. Phase is a model value - it is not
    calibrated per character or per instance.
  </p>

  <h3>The sun</h3>
  <p>
    Sunrise and sunset vary across the 400-day Elanthian year. Rather than model
    the solar geometry, the page uses empirical lookup tables of rise and set
    times indexed by day of year (0-399), which capture the seasonal swing
    directly. The time of day (dawn, midday, dusk, and so on) is derived from
    where the current moment falls between that day's sunrise and sunset.
  </p>

  <h3>The calendar</h3>
  <p>
    The Elanthian calendar is regular and fully derivable from the clock:
  </p>
  <ul>
    <li><strong>Day</strong> - 21,600 seconds, divided into 12 anlas (hours) of
      1,800 seconds; each anlas is 30 roisaen (minutes) of 60 seconds.</li>
    <li><strong>Month</strong> - 40 days.</li>
    <li><strong>Year</strong> - 400 days (10 months). Years cycle through seven
      named "Year of the..." titles.</li>
    <li><strong>Named cycles</strong> - the 12 anlas, the 10 months, and the 7
      year-names each have their own name, all shown alongside the numeric date.</li>
  </ul>

  <h2>Accuracy and caveats</h2>
  <ul>
    <li>Moon periods are the developers' sidereal orbits, cross-validated to under
      a second; sun and calendar use validated constants and empirical tables.</li>
    <li>All countdowns are quantized to the 60-second server tick, matching how
      the game advances time.</li>
    <li>Phase is a pure model value with no per-character calibration, so it may
      differ slightly from what a specific character observes if the game applies
      any personal offset.</li>
    <li>The page reads your device clock. If your clock is wrong, the readout will
      be off by the same amount.</li>
  </ul>

  <h2>Running and deploying</h2>
  <p>
    <strong>Open <code>index.html</code> in any browser. That is the entire
    thing.</strong> No server, no build step, no dependencies, and no external
    requests. It computes everything locally and works fully offline.
  </p>
  <p>To host it, drop the file on any static host. For example, on Cloudflare Pages:</p>
  <ul>
    <li>Framework preset: <strong>None</strong></li>
    <li>Build command: <em>(leave empty)</em></li>
    <li>Output directory: the folder containing <code>index.html</code></li>
  </ul>

  <h2>Project layout</h2>
  <p>
    <code>index.html</code> is the whole project - one file, hand-contained, with
    the HTML, CSS, and the JavaScript model all inline. Nothing else is required
    to run or host it. This documentation page lives alongside it and is linked
    from the footer of the dashboard.
  </p>

  <div class="foot">
    Source: <a href="https://github.com/MahtraDR/DRMoonWatch">github.com/MahtraDR/DRMoonWatch</a>.
    Deterministic from the Elanthian clock - no server, no network, no tracking.
  </div>

</div>
</body>
</html>
