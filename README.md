# QR Standee Generator

A small browser tool that turns a checkpoint name and a link into a clean, printable **QR standee card** — the kind you place at gates, lobbies, lift lobbies and help desks so visitors can scan and go.

**Try it:** open `index.html` in a browser (internet needed once, for the QR library). No build step, no server.

## What it does

- Live preview while you type: top band text, checkpoint name, link, and the card's bottom line
- **Add card to sheet** — build a full sheet of checkpoints, one card per scan point
- **Print sheet** — print-ready layout (cards sized for A4, remove buttons and controls hidden automatically)
- Remove any single card with the × button

## Why I built this

At [SlopeMaps](https://slopemaps.in), every venue onboarding ends with the same job: print QR standees for each checkpoint so visitors can start navigating from the gate. Making those cards by hand — one QR at a time, pasted into a document — was slow and error-prone. This generator makes a checked, uniform sheet in minutes: type the checkpoint, check the preview, add, print.

## Tech

- Plain HTML, CSS and JavaScript in one file
- QR codes drawn with the [`qrcode-generator`](https://www.npmjs.com/package/qrcode-generator) library (loaded from CDN)
- Print styles via a CSS `@media print` block
