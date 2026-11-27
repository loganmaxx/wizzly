<div align="center">

# Wizzly

**macOS-style Dock, Dynamic Island Notch & Spotlight for Windows**

Lightweight desktop companion built with Rust & Tauri — bringing a customizable glass Dock, interactive Notch/Dynamic Island, Desktop Widgets, and instant Spotlight search to Windows.

[Download Latest Release](https://github.com/loganmaxx/wizzly/releases/latest) · [Contribute a Translation](locales/README.md) · [Privacy & Data](#privacy--data) · [Report a Bug](https://github.com/loganmaxx/wizzly/issues) · [Support Wizzly](#support--donate)

</div>

---

<p align="center">
  <img src="assets/preview.jpg" alt="Wizzly Desktop Preview" width="850" />
</p>

## Features

### Dock & Desktop Experience
- **Customizable Glass Dock** — Choose between **Frosted**, **Liquid**, **Matte**, and **Classic** glass materials with optional **Wallpaper Tint** and **Dark / Light** themes.
- **Icon Styles & Animations** — Smooth magnification, launch bounce, running indicators, `HSHELL_FLASH` attention badges, window previews, and icon styles (*Windows*, *Squircle*, *macOS Pack*, *Normalized*).
- **Interactive Drag & Drop** — Drag apps from Launchpad to pin, drag icons out to unpin, or drop files directly onto Dock icons to open them.
- **Folders, Stacks & Virtual Desktops** — Pin custom folders, browse your **Downloads Stack** (Grid or List view), access Trash, and switch **Spaces / Virtual Desktops** right from the Dock.
- **Built-in System Panels** — Quick access to Launchpad, Wi-Fi, **Per-App Volume Mixer**, Control Center, Calendar, and System Tray.
- **Multi-Monitor & Smart Auto-Hide** — Uniform **Smart / Always / Never** auto-hide modes for Dock and Notch, target Primary monitor, Follow Cursor, or a specific display, with fullscreen detection.

### Wizzly Notch (Notch / Dynamic Island)
- **Media, Winamp & Synced Lyrics** — Now-playing widget (including classic **Winamp** support), WASAPI reactive equalizer, playback controls, seek bar, live synced lyrics with manual picker, and **Karaoke Mode**.
- **Live Privacy & Hardware Alerts** — Real-time **Mic & Camera** active indicators, charging/battery alerts, Bluetooth battery ring, and exclusive Volume/Brightness OSD.
- **File Shelf (AirDrop-style Tray)** — Drag files from Explorer onto the Notch to hold them temporarily, then drag them out into browsers, Discord, WhatsApp, etc.
- **Clipboard History, Calendar & Prayer Times** — Search, pin, and quick-paste copied items; view upcoming events; and track daily Prayer Times.
- **Focus / Pomodoro Timer** — Built-in timer modes right inside the Notch.

### Spotlight Search & Desktop Widgets
- Press **`Alt + Space`** (fallback: `Ctrl + Alt + Space`) to search and launch apps, run system items, or calculate math expressions inline.
- **Desktop Widgets** — Clock (with Depth Wallpaper cutout support), Vinyl player, Calendar, and Memo widgets.

### Localization
- Available in **English** and **Indonesian**, plus **Community Translations** (`locales/*.json` + live import via **Settings → General → Import JSON...**).

---

## Download & Installation

1. Go to [**Releases**](https://github.com/loganmaxx/wizzly/releases/latest).
2. Download **`Wizzly_0.1.3_x64-setup.exe`**.
3. Run the installer and follow the setup wizard (supports English & Indonesian).

> **Note about Windows SmartScreen**
> Because Wizzly is an independent app without a paid EV code-signing certificate yet, Windows Defender SmartScreen may show *"Windows protected your PC"* on first launch. Click **More info → Run anyway** to proceed.

---

## Contribute a Language / Translation

Want to translate **Wizzly** into your language or improve an existing translation?
You don't need access to the main app source code — all UI strings live right here in [`locales/`](locales/)!

- Read the step-by-step guide in **[`locales/README.md`](locales/README.md)**.
- Copy [`locales/en.json`](locales/en.json) to `locales/<your-code>.json` (e.g. `ja.json`, `de.json`, `es.json`, `tr.json`, `pt-br.json`).
- Test your translation live inside Wizzly using **Settings → Interface Language → Import JSON...** (or place it in `%AppData%\com.wizzly.app\locales\`).
- Submit a **Pull Request** with your `.json` file, or open a [**Translation Submission Issue**](https://github.com/loganmaxx/wizzly/issues/new/choose) and attach your file!

See [`CONTRIBUTING.md`](CONTRIBUTING.md) for quick PR instructions.

---

## System Requirements

- **OS:** Windows 10 / Windows 11 (64-bit)
- **Runtime:** Microsoft Edge WebView2 Runtime (already pre-installed on Windows 11 and most Windows 10 systems)

---

## Privacy & Data

Wizzly is built to run **locally on your PC** with **no ads, no analytics, and no telemetry**.

### What Wizzly Accesses Locally (Never Leaves Your Device)
- **Installed Apps, Running Windows & Shortcuts** — Used locally to populate the Dock, Launchpad, and Spotlight search (`Alt + Space`).
- **Windows Notifications & Privacy Indicators** — Read locally via Windows APIs to display alert previews and active Mic/Camera indicators in the Notch.
- **Clipboard History & File Shelf** — Stored locally on your device so you can search, pin, or drag items from the Notch, and can be cleared anytime.
- **System Controls (Audio, Wi-Fi, Bluetooth, Battery, Wallpaper)** — Accessed via local Windows APIs to power the Dock status panels, per-app volume mixer, and wallpaper tinting.
- **App Settings & Notes** — Saved locally on your PC (`%APPDATA%\com.wizzly.app` and local app storage).

### Optional External Network Requests
- **Synced Lyrics (`lrclib.net`)** — When fetching lyrics for a playing track, Wizzly sends only the track title, artist, album, and duration to the public [LRCLIB](https://lrclib.net) API.
- **Prayer Times City Lookup (`get.geojs.io` / `geocoding-api.open-meteo.com`)** — Used only when auto-detecting or searching a city for Prayer Times.
- **No personal data, clipboard contents, notifications, or usage logs are ever sent to any developer server.**

---

## Support & Donate

Wizzly is free to download and use. If you enjoy using it and want to support future updates, you can support the project via:

- **PayPal:** [paypal.me/adrn87](https://paypal.me/adrn87)
- **Binance Pay (UID):** `977044132`
- **QRIS (Indonesia):**

<p align="left">
  <img src="assets/qris.png" alt="Wizzly QRIS Donate" width="220" />
</p>

---

## Feedback & Support

Found a bug or have an idea for Wizzly?
Open an issue on the [**Issues**](https://github.com/loganmaxx/wizzly/issues) tab!

<p align="center">
  Made with ❤️ by Adrian
</p>
