# LineUp — Rehearsal Partner

A single-file browser app that helps musicians, actors, and speakers rehearse more effectively.

## Features

- **Script Capture** — Upload images of scripts, extract text with OCR (Tesseract.js)
- **Rehearsal Mode** — Practice with speech recognition that tracks your lines
- **Playback** — Hear your script read aloud with text-to-speech
- **Practice Tools** — Line tracking, cue practice, timers

## Quick Start

1. Download `lineup.html`
2. Open it in Chrome or Edge (requires HTTPS or localhost for speech features)
3. Start rehearsing

No build step, no install, no dependencies beyond the CDN-loaded Tesseract.js.

## Requirements

- Chrome or Edge (for speech recognition)
- HTTPS or `localhost` (speech APIs require secure context)

## Tech Stack

- Single HTML file — CSS, JS, and markup all inline
- [Tesseract.js](https://tesseract.projectnaptha.com/) for OCR
- Web Speech API (SpeechRecognition + SpeechSynthesis)
- No package manager, no build tool

## License

MIT
