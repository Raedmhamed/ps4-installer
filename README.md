# PS5 Web Click Test

A web-based **test harness** for the PS5 browser: click tests, notification tests, gamepad (DualSense) reading, vibration, audio, fullscreen, pointer lock, storage, and device info — all runnable directly on the PS5.

## Features

- Big **click counter** with latency measurement
- **Notification test** (permission flow + send, custom title/body)
- **Gamepad API** polling for the DualSense controller
- Vibration, audio beep, fullscreen, pointer lock, storage tests
- Device / screen info dump
- Network test against the PS5 (default IP `192.168.8.26`, remote-play port `9295`)
- Exportable log

## Usage

1. Host this repo (enable **GitHub Pages** on `main` / root).
2. Open the page in the PS5 browser (target IP `192.168.8.26`).
3. Run the tests from the tabs.

## Notes

- PS5 remote-play port `9295` is auth-gated: an opaque/403 response means the console is alive (expected).
- Notification delivery on PS5 varies by firmware; use this page to probe support.

## License

MIT
