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
- Mirror mode paints both halves symmetrically, as Selbu patterns are.
- Right-click drag erases; Ctrl+Z undoes per stroke.
- Chart conventions: bold gridline every 5 stitches/rows, stitch numbers along
  the bottom (stitch 1 at the right), row numbers up the side.
- Download the chart as a PNG; work autosaves to the browser's localStorage.

## Development

It is a single static `index.html` — open it in a browser. No build step.
