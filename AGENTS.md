# AGENTS.md

## Repo structure
Single-file app: `lineup.html` — no build step, no package manager, no tests.

## Dependencies
- Tesseract.js loaded from CDN (line 7). No local `node_modules` or lockfile.
- Browser APIs: `SpeechRecognition` (Chrome/Edge only), `SpeechSynthesis`, `getUserMedia`.

## Workflow
- Open `lineup.html` directly in a browser. No dev server or build command.
- Speech recognition requires HTTPS or `localhost`.
- Editing the file: all CSS (lines 8–176), JS (lines 274–834), and markup are inline.
