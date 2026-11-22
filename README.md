# Cube Timer

A Rubik's cube timer with a full CFOP training mode, split timing, detailed stats, and animated backgrounds you can customize.

**Live demo:** https://tutorv102-lab.github.io/cube-timer/

## Features

### Timer
- Hold <kbd>Space</kbd> (or touch and hold on mobile) until the digits turn green, release to start, press any key to stop
- Optional WCA-style 15-second inspection with +2 / DNF rules and audio cues at 8 and 12 seconds
- Random-move scrambles for 2×2, 3×3, 4×4 and 5×5, with a cube-net preview of the scrambled state
- Mark solves as OK / +2 / DNF, or delete them
- Confetti and a chime when you set a new personal best

### CFOP training mode
- **Split timing** – press at the end of each stage (Cross → F2L → OLL → PLL, or 7 stages with F2L pair by pair) and see which stage costs you the most time
- **Cross trainer** – shows the optimal cross solution (breadth-first search over all 190,080 cross states) for white, yellow or every colour, with an option for harder 6+ / 7+ move crosses
- **F2L trainer** – all 41 front-right slot cases with shortest ⟨R, U, F⟩ solutions found by an IDA* search, plus 3D case diagrams
- **OLL (57) and PLL (21) trainers** – case setups with random AUF, a case picker, and per-case average times
- Every algorithm was checked with a sticker-level cube simulator

### Stats
- Single, mean, mo3, ao5, ao12, ao25, ao50 and ao100 (current and best, WCA trimming)
- Session goals, a sub-X ladder, a last-12 bar chart and a 50-solve trend chart
- Separate sessions for every puzzle and training mode

### Customization (✦ Studio)
- 10 ready-made looks
- Background: 12 animated canvas scenes, your own gradient, a solid colour, or your own image / GIF / video (with Ken Burns, pan, mouse-parallax, breathe and hue animations)
- 7 particle overlays (snow, sakura, bubbles, fireflies, rain, stars, falling cubes)
- 7 colour themes plus custom colours, 8 timer fonts, 6 Thai UI fonts, 4 digit styles
- 5 card styles, adjustable corner radius, glass opacity and blur, 4 layouts

## Tech
- A single self-contained `index.html`: vanilla JavaScript, Canvas 2D and SVG, with no build step and no dependencies
- Times and settings are saved in `localStorage`, and uploaded background files in IndexedDB. Everything stays in your own browser.

## Run locally
Open `index.html` in any modern browser.

## License
MIT
