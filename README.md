# vaikhashi.github.io

My portfolio, live at **https://vaikhashi.github.io**.

It's laid out like an agent workflow, because that's what I build at work: you're the trigger, a router asks what you're after, and each branch jumps to a section. Switch to dark mode and the canvas dots turn into stars.

Press <kbd>/</kbd> (or <kbd>Ctrl</kbd>/<kbd>⌘</kbd> + <kbd>K</kbd>) on the page for a command palette. Try `help`, then `launch`.

## Under the hood

- One hand-written `index.html`: no framework, no build step, no dependencies besides two Google Fonts (Martian Mono and Instrument Sans).
- Workflow edges are SVG paths recomputed from node positions, so the graph re-flows from three columns on desktop to a vertical layout on phones.
- Respects `prefers-reduced-motion` and `prefers-color-scheme`, with a manual theme toggle.

## Run locally

```bash
git clone https://github.com/Vaikhashi/vaikhashi.github.io
cd vaikhashi.github.io
python -m http.server 8000   # then open http://localhost:8000
```
