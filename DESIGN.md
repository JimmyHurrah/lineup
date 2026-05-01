# LineUp — Rehearsal Partner

## Overview
LineUp is a single-file browser application that helps musicians, actors, and speakers rehearse more effectively. It combines OCR, speech recognition, and text-to-speech in one offline-capable HTML file.

## Core Features

### 1. Script Capture (OCR)
- Upload or capture images of scripts/text
- Tesseract.js extracts text from images
- Edit extracted text in a built-in editor

### 2. Rehearsal Mode
- Displays script line-by-line or full view
- Speech recognition tracks spoken words (Chrome/Edge)
- Highlights current line being spoken
- Tracks progress through the script

### 3. Playback & Review
- Text-to-speech reads script aloud
- Adjustable speed and voice selection
- Repeat difficult sections

### 4. Practice Tools
- Line skipping / cue practice
- Timer and session tracking
- Notes and annotations

## Architecture

```
lineup.html
├── CSS (lines 8–176)       — All styles inline
├── HTML (lines 177–273)    — Markup structure
└── JavaScript (lines 274–834) — Application logic
    ├── OCR Module           — Tesseract.js integration
    ├── SpeechRecognition    — Browser API
    ├── SpeechSynthesis      — Browser API
    ├── Script Editor        — Contenteditable/text area
    └── Rehearsal Engine     — Line tracking & playback
```

## Tech Stack
- **Runtime**: Browser (Chrome/Edge recommended for speech recognition)
- **OCR**: Tesseract.js v5 (CDN)
- **Speech**: Web Speech API (SpeechRecognition + SpeechSynthesis)
- **No build step**, no package manager, no dependencies beyond CDN

## Constraints
- Speech recognition requires HTTPS or localhost
- Speech recognition works only in Chrome/Edge
- Single HTML file — all code inline
- No backend, no data persistence (localStorage only)

## Future Considerations
- Export/import scripts as files
- Cloud sync option
- Mobile responsive improvements
- Multi-language support
- Recording rehearsals
