# PS5 Jailbreak Test

A web-based **jailbreak test harness** for the PS5 browser, styled like webkitty.arabpixel.net — but only the jailbreak section and the PS button. Runs real browser-capability probes and collects honest logs (successes and failures).

## Features

- Big **PS button** to start a jailbreak attempt (auto-retry toggle + stop)
- Real **timestamped logs** of every step: environment, notification, PS5 endpoint fetch, ArrayBuffer, WebAssembly, SharedArrayBuffer, WebGL, storage, gamepad, vibration
- **Notification test** (permission flow + send)
- **Collect Logs** + export `.txt` (also persisted in localStorage)
- Success rate tracking

## Usage

1. Host this repo (enable **GitHub Pages** on `main` / root).
2. Open the page in the PS5 browser (target IP `192.168.8.26`).
3. Press the **PS** button. Watch the real logs. Export when done.

## Notes

- PS5 remote-play port `9295` is auth-gated: an opaque/403 response means the console is alive (expected, logged).
- No actual exploit payload is shipped; this is a capability probe + log collector.

## License

MIT
