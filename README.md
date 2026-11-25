# PS4 PKG Web Downloader

A simple web page that lets you **download and install `.pkg` files directly on your PS4** through the PS4 browser — no PC tooling required.

## Features

- Paste a direct `.pkg` link and download/install in one tap
- Batch queue: paste many URLs (one per line) and download them one at a time
- Download history (stored locally in the browser)
- Works as a static site — host it anywhere (GitHub Pages included)
- PS4-themed dark UI, mobile-friendly

## Usage

1. Host this repo (enable **GitHub Pages** on `main` / root).
2. Open the page in your PS4 browser.
3. Paste a direct link to a `.pkg` file.
4. Tap **Download PKG** — the PS4 browser hands the file to the system package installer.

## Requirements

- PS4 with a working browser & package installer
- A **direct** link to the `.pkg` (no HTML wrapper / redirect-only pages)
- Enough free storage on the PS4

## Notes

- Everything runs locally in the browser. URLs and history live only in `localStorage`.
- Nothing is sent to any server except the PKG host you choose.
- Some hosts block hotlinking — try a different mirror if a download does not start.

## License

MIT
