# PS4 PKG Homebrew Store

A web-based **homebrew store** for PS4: browse a catalog of `.pkg` files and download/install them **directly on your PS4** through the PS4 browser — no PC tooling required.

## Features

- Storefront of packages loaded from `packages.json`
- Search + category filter
- One-tap **Download** that hands the `.pkg` to the PS4 system installer
- **Add PKG** tab to add your own packages (stored in your browser)
- **Manage** tab: export/import `packages.json`, clear added packages
- Download history
- Works as a static site (GitHub Pages)

## Usage

1. Host this repo (enable **GitHub Pages** on `main` / root).
2. Open the page in your PS4 browser.
3. Tap **Download** on a package.

## Add your own packages

- **Option A (personal):** use the **Add PKG** tab — saved in your browser.
- **Option B (shared):** edit `packages.json` in the repo, or use **Manage → Export packages.json** and commit it.

Each entry needs at least `name` and `url` (direct link to a `.pkg`). Optional: `version`, `author`, `category`, `size`, `icon` (emoji or image URL), `description`.

## Requirements

- PS4 with a working browser & package installer
- Direct links to `.pkg` files
- Enough free storage on the PS4

## Privacy

Everything runs locally in your browser. Added packages and history live in `localStorage`. Nothing is sent anywhere except the PKG host you choose.

## License

MIT
