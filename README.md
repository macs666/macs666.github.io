# macs666.github.io

Personal site of Muhammed Azhar, agentic AI & backend engineer. Live at https://macs666.github.io.

The page tells my journey to AI as a 3D circuit board that builds itself as you scroll. Each part on the board (R1, U1, SW1, R2, U2, D1) is one step, from teaching a camera to see with OpenCV in college to building AI at Recapp.

## How it works

- One static `index.html`, no build step. Three.js r128 loads from cdnjs.
- The words live once, in plain HTML inside `<main id="story">`. The 3D scene reads its chapters from there, so screen readers and search engines get the same text, and so do browsers without WebGL.
- Phones get a lighter scene, and the last shot turns the board upright to fit a tall screen.
- `cv.pdf` is the downloadable CV, and `og.jpg` is the link preview image.

## Run locally

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000. Add `#p=0.5` to the URL to jump halfway through the story.

## Deploy

Push to `main`. GitHub Pages serves the repo root.
