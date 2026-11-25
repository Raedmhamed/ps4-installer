# PS5 WebKitty Jailbreak Test

A web-based **jailbreak test harness** for the PS5 browser, in the style of [WebKitty](https://github.com/ArabPixel/WebKitty) (ArabPixel) — only the jailbreak section and the PS button, with the same dark theme, PS logo, DebugConsole span-based colored logs, global error handlers, and success-rate tracking.

## Features

- Big **PS button** (WebKitty's PS logo) to start a jailbreak attempt
- Auto-retry + Stop Auto Jailbreak
- **Real timestamped logs** in a WebKitty-style `DebugConsole` (`<pre id="console">`, colored spans)
- Global `window.onerror` / `unhandledrejection` handlers reporting to the console (WebKitty style)
- Each attempt runs real probes: environment, **notification debug test** (permission + send, logged), ArrayBuffer, WebAssembly, SharedArrayBuffer, WebGL, storage, gamepad, vibration
- Collect / export `.txt` logs (localStorage persisted)
- Success rate tracking
- No separate IP test or notification section — notification is tested inside the attempt

## Usage

1. Host this repo (enable **GitHub Pages** on `main` / root).
2. Open the page in the PS5 browser.
3. Press the **PS** button. Watch the real logs in the DebugConsole.

## Notes

- No actual exploit payload is shipped; this is a capability probe + log collector in WebKitty's style.

## License

MIT
