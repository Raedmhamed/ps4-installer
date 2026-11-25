# PS5 WebKitty Test Host

A web-based **jailbreak-style test host** for the PS5 browser, modeled on
[webkitty.arabpixel.net](https://webkitty.arabpixel.net). Runs a real diagnostic chain
on click of the **JAILBREAK** button and logs every step — successes and failures —
including a notification delivery test. Designed to be used **directly in the PS5
browser** (not on PC).

## Features

- Big **JAILBREAK** button running a multi-step diagnostic chain
- Real per-step logs (success + failure), even when APIs are missing
- Notification permission flow + delivery test fired at the end
- WebKit / Gamepad / Storage / Vibration / Audio / Fullscreen / PS5 reachability probes
- Auto-Jailbreak, Auto-Retry, Reload-after-success, Barebone (quiet) modes
- Payload selector (GoldHEN-style list + custom upload)
- WebKitty-style settings (language, theme, layout, fan threshold)
- Device / screen info dump
- Exportable combined log

## Usage

1. Host this repo (enable **GitHub Pages** on `main` / root).
2. Open the page in the PS5 browser (target IP `192.168.8.26`).
3. Click **JAILBREAK** (or let Auto-Jailbreak run). Watch the log.

## Notes

- PS5 remote-play port `9295` is auth-gated: an opaque/403 response means the console
  is alive (expected).
- Nothing here can harm the console — it only probes browser capabilities and PS5
  reachability.

## License

MIT
