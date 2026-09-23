# Cut-program

Push/pull/legs tracker for a carnivore cut. Single file, no build step, no dependencies
beyond two webfonts — charts are hand-drawn SVG.

- **7-day rotation** — Pull A / Legs A / Push A / Pull B / Legs B / Push B / Push C, plus a
  PM HIIT slot whose modality auto-matches the morning's day type.
- **Targets progress themselves.** Hit every working set at the target reps and the next
  target moves up (+10 lb on the big lifts, +5 on everything else). Nothing is hardcoded.
- **Navy body-fat** from weight, neck and waist, charted against the waist measurement
  that actually predicts abs.
- **Rest timer** starts on its own when a set is logged, and counts past zero.

## Where the data lives

Published as a Claude Artifact, the tracker keeps sessions, weigh-ins, targets and PRs in
the artifact's database — they survive clearing the browser and sync across devices.
Served from GitHub Pages there is no such host, so it falls back to `localStorage`
on that device only. The header pill says which mode you're in.
