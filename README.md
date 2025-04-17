# Tokungaku - Visual Music Composition on Images

Tokungaku is a free browser-based music notation tool that lets you draw musical sequences directly on images. Create, edit, and play back compositions with an intuitive piano-roll interface. No installation required. The name combines Japanese words "Ongaku" (音楽, music) and "Tokuten" (得点, scoring/notes/marks).

**⚠️ This codebase was completely generated by AI (Claude AI).**

## Features

- Upload and display background images
- Piano-roll grid overlay (3 octaves, configurable columns)
- Create, edit, move, and resize notes
- Play back the created sequences
- Adjustable BPM and time signature
- Keyboard shortcuts for common operations
- Export sequences as MIDI files
- Save and load projects using local storage

## Getting Started

### Installation

No installation is required. Simply download the project files and open `index.html` in a web browser.

```bash
git clone https://github.com/rotten77/tokungaku.git
cd tokungaku
```

### Usage

1. Open `index.html` in a web browser.
2. (Optional) Upload a background image.
3. Add notes by clicking on the grid.
4. Adjust note properties using the controls or keyboard shortcuts.
5. Play back the sequence with the play button or spacebar.
6. Save your project to local storage.

## Project Structure

```
tokungaku/
├── index.html       # Main HTML structure
├── css/
│   └── styles.css   # Application styling
├── js/
│   ├── app.js       # Main application logic
│   ├── grid.js      # Grid rendering and management
│   ├── notes.js     # Note handling (add, edit, delete)
│   ├── audio.js     # Audio playback and MIDI export
│   ├── storage.js   # Local storage management
│   └── ui.js        # UI interactions and event handling
└── README.md        # Project documentation
```

## Keyboard Shortcuts

- **A**: Add note
- **D**: Delete selected note
- **W**: Increase note length
- **S**: Decrease note length
- **Arrow keys**: Move selected note
- **Space**: Play/Stop

## Technical Details

### Browser Compatibility

Tokungaku is built using modern web standards and should work in all modern browsers, including:

- Chrome (recommended)
- Firefox
- Safari
- Edge

### Dependencies

Tokungaku is built with vanilla JavaScript and doesn't require any external libraries or frameworks.

## Limitations

- MIDI export is currently implemented as a JSON representation. A proper MIDI export would require a MIDI library.
- Audio playback uses simple sine wave oscillators. More advanced sound synthesis would improve the audio quality.
