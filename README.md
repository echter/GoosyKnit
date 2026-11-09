# GoosyKnit — selbu mitten chart maker

A browser-based knitting chart editor for classic Selbu mittens (selbuvotter):
a mitten-shaped grid with a rectangular body and a triangular tip, drawn in
the style of a vintage Norwegian pattern leaflet.

**Live:** https://echter.github.io/GoosyKnit/

## Features

- Mitten-shaped chart: configurable width (default 30 stitches) and body rows
  (default 73); the tip tapers one stitch per side per row down to a point.
  Front (back of hand) and palm are shown joined edge to edge, as knit in the
  round, with red dividers every 15 stitches and a ribbed cuff (ribbekant).
- Yarn: a **base** color fills the whole mitten, and **patterns** are knit on
  top. One pattern (black) by default; add more with the + swatch. Clicking the
  selected pattern recolors every stitch knit with it, live. Right-click removes
  a pattern. Old charts migrate automatically.
- Tools: knit, erase, fill (flood a connected area; right-click fills with the
  base), select, and the slash \ / and dot symbol marks. Keyboard 1–7.
  Hold Shift while dragging to lock a straight horizontal, vertical or
  diagonal line.
- Selection: drag a rectangle, then copy / cut / paste (Ctrl+C / X / V), Delete
  clears it, Esc deselects. Paste floats a ghost under the cursor; click to
  place it. H / V flip the ghost.
- Stamps: a library of motifs (ships with a selburose). Draw a new one in the
  stamp editor (with its own mirror option), or save a selection as a stamp.
  Pick a stamp and click the chart to place it; each placement is one undo
  step. A one-color stamp takes the selected pattern; "See-through base" stamps
  only the pattern stitches.
- Mirror mode paints, fills and stamps both halves symmetrically.
- Knitting row tracker: +/− beside the chart steps the row currently on the
  needles and highlights it in red. Keyboard: + and −. Knitting mode (K) hides
  the tools and shows the current row magnified.
- Thumb opening marker on the palm side: customizable width, row, chart side
  (left/right), and inset from the edge; included in PNG and PDF exports.
- A resident goose in the bottom-right corner. It honks.
- Right-click drag erases; undo/redo buttons plus Ctrl+Z / Ctrl+Y, per stroke.
  Clear front/back and Clear everything ask first and are undoable too.
- The whole mitten fits the window by default; zoom in/out/fit controls.
- Chart conventions: bold gridline every 5 stitches/rows, stitch numbers along
  the bottom (stitch 1 at the right), row numbers up the side.
- Export: PNG of both sides, or a vector PDF (hand-built in plain JS, no
  libraries) as one joined page or one page per side. The page turns portrait
  or landscape, whichever gives the chart larger squares. Work autosaves to
  localStorage.

## Development

It is a single static `index.html` — open it in a browser. No build step.
