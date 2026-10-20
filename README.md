# Morse Code Trainer

A self-contained International Morse code trainer for shhosting.net. The app is a single HTML file with inline CSS and JavaScript; it uses the site's shared stylesheet and site shell for navigation and footer.

## Features

- Interactive SVG Morse decision tree with highlighted branches and selectable characters.
- International Morse letters, digits, and common punctuation.
- Text-to-Morse conversion and audio playback through the Web Audio API.
- Receive practice with randomized questions, immediate feedback, and per-character accuracy.
- Manual dot/dash keying using pointer/touch controls or the space bar, plus character gaps and decoding.
- Adjustable character speed, effective/Farnsworth speed, tone frequency, and volume.
- Local settings and progress saved in browser storage.
- JSON progress export/import and reset controls.
- Responsive layout and light/dark themes inherited from the shared site stylesheet.
- No external runtime libraries, build step, remote APIs, or uploaded data.

## Run locally

Open `index.html` in a modern browser. Audio requires a user gesture and a browser with Web Audio API support. When deployed on shhosting.net, the page loads the site's shared assets from root-relative paths.

## Notes

- Progress is stored in this browser only. Export a JSON backup to transfer progress to another browser/device.
- Manual keying uses a configurable-in-code duration threshold to distinguish dots from dashes.
- Morse audio is generated in the browser; no audio files are downloaded.
