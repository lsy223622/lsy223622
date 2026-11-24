# lsy223622

Undergraduate student at **Xidian University**. I build self-contained software across systems, networking, desktop/mobile apps, and embedded hardware—mostly tools I wanted for myself and ended up polishing for others to use.

[Website](https://lsy223622.com) · [Blog](https://blog.lsy223622.com) · [All Repositories](https://github.com/lsy223622?tab=repositories)

## Systems, Audio & Networking

- **[HearPort](https://github.com/lsy223622/HearPort)** (`Swift`, `C++`, `WinUI 3`) — Turns an iPad into a low-latency speaker for a Windows 11 PC over Wi-Fi or USB. Supports automatic USB-to-Wi-Fi failover and PIN-based pairing backed by Windows Credential Manager and iPadOS Keychain. · [Releases](https://github.com/lsy223622/HearPort/releases)
- **[UniDERP](https://github.com/lsy223622/UniDERP)** (`Go`, `JavaScript`, `Docker`) — Shares self-hosted Tailscale DERP relays across multiple independent tailnets. Uses a Controller/Member split that keeps OAuth credentials isolated on the controller, with a patched `derper` enforcing bounded policy caches and per-tailnet traffic scheduling. · [Releases](https://github.com/lsy223622/UniDERP/releases)
- **[PinNode](https://github.com/lsy223622/PinNode)** (`Kotlin`, `Go`) — Turns an Android phone into a temporary, managed Tailscale node using a one-time 6-digit PIN. Keeps long-lived Tailscale API credentials on the server while handling short-lived auth keys, routing profiles, and automatic node cleanup. · [Releases](https://github.com/lsy223622/PinNode/releases)
- **[EveryTwins](https://github.com/lsy223622/EveryTwins)** (`C++`, `CMake`) — A Windows-native whole-disk duplicate-file finder. Queries Everything's local index instead of walking the filesystem, stays around ~2 MB+ baseline memory via bounded metadata and session spooling, and compares large files near-instantly using five-window BLAKE3 sample hashing.

## Self-Hosted Web & Embedded

- **[BloGo](https://github.com/lsy223622/BloGo)** (`Go`, `JavaScript`) — Single-binary static-rendering blog engine with zero runtime dependencies, built-in lightweight analytics, and live-reload `dev` preview. Powers [blog.lsy223622.com](https://blog.lsy223622.com). · [Releases](https://github.com/lsy223622/BloGo/releases) · [Live Demo](https://blog.lsy223622.com)
- **[PathBay](https://github.com/lsy223622/PathBay)** (`Go`, `Docker`) — Lightweight self-hosted HTTP route and response server with an embedded admin UI and JSON API for redirects, static files, downloads, custom 404 pages, and in-memory 429 rate limiting. · [Releases](https://github.com/lsy223622/PathBay/releases)
- **[NanoInk](https://github.com/lsy223622/NanoInk)** (`C`, `C++`, `ESP32`) — Compact ESP32 + 2.13" e-paper information terminal displaying daily class schedules, weather, time, battery voltage, and TOTP codes, combining a DS3231 RTC, partial screen refresh, and periodic deep sleep.

## Desktop, Mobile & Daily Utilities

- **[XDUClassVideoDownloader](https://github.com/lsy223622/XDUClassVideoDownloader)** (`Python`, `Flask`, `JavaScript`) — Course video downloader for Xidian University's lecture capture platform (179★, 20 forks). Rebuilt in v5 with a unified `core` facade serving a local Flask WebUI, CLI, and automated batch mode. · [Releases](https://github.com/lsy223622/XDUClassVideoDownloader/releases)
- **[MotionPhotoManager](https://github.com/lsy223622/MotionPhotoManager)** (`Kotlin`, `Jetpack Compose`) — Offline Android tool for batch-splitting Motion Photos (`MVIMG_*`, `PXL_*`, `*_MP.jpg`) into JPEG stills and embedded MP4 videos by parsing XMP/`MicroVideoOffset` metadata locally, with zero network permissions. · [Releases](https://github.com/lsy223622/MotionPhotoManager/releases)
- **[DiaryAssistant](https://github.com/lsy223622/DiaryAssistant)** (`Python`) — Local Markdown diary companion using the DeepSeek API to maintain an evolving user profile, generate reflective comments, and compile weekly summaries.

## Technical Focus

- **Systems & Networking:** C++, Go, Tailscale / DERP relay internals, low-latency audio streaming, Windows native tooling
- **Client & Mobile:** Swift (iPadOS), Kotlin (Android / Jetpack Compose), WinUI 3, Python / Flask
- **Embedded & Infrastructure:** C/C++ (ESP32, e-paper, low-power scheduling), Docker, Linux self-hosting
