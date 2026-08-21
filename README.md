# GoosyKnit — Selbuvott chart maker

A browser-based knitting chart editor for classic Selbu mittens (selbuvotter):
a mitten-shaped grid with a rectangular body and a triangular tip, drawn in
the style of a vintage Norwegian pattern leaflet.

**Live:** https://echter.github.io/GoosyKnit/

## Features

- Mitten-shaped chart: configurable width (default 27 stitches, kept odd so a
  center stitch exists for the selburose) and body rows; the tip tapers one
  stitch per side per row down to a single stitch.
- Yarn palette (black, madder red, blue) plus custom colors via a color picker.
- Tools: knit (paint), erase, and a 15×15 selburose stamp. Keyboard: 1/2/3.
- Front and back sides: separate charts for the back of the hand and the palm,
  with tabs showing which side is active (keyboard: F flips).
- Mirror mode paints both halves symmetrically, as Selbu patterns are.
- Right-click drag erases; undo/redo buttons plus Ctrl+Z / Ctrl+Y, per stroke.
- The whole mitten fits the window by default; zoom in/out/fit controls.
- Chart conventions: bold gridline every 5 stitches/rows, stitch numbers along
  the bottom (stitch 1 at the right), row numbers up the side.
- Export: PNG of the current side, or a two-page vector PDF of both sides
  (hand-built in plain JS, no libraries); work autosaves to localStorage.

## Development

It is a single static `index.html` — open it in a browser. No build step.
