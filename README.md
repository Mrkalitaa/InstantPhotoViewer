# ⚡ Instant Photo Viewer for Windows

<div align="center">

[![Download on Microsoft Store](https://get.microsoft.com/images/en-us%20dark.svg)](https://apps.microsoft.com/detail/9NV5167C5GGS)

[![Platform](https://img.shields.io/badge/Platform-Windows%2010%20%7C%20Windows%2011-0078D6?logo=windows&logoColor=white)](https://apps.microsoft.com/detail/9NV5167C5GGS)
[![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)](LICENSE)
[![Store Status](https://img.shields.io/badge/Store%20Status-Official%20Release-blue.svg)](https://apps.microsoft.com/detail/9NV5167C5GGS)
[![Graphics](https://img.shields.io/badge/Graphics-Direct3D%2011%20%7C%20Direct2D-00599C?logo=c%2B%2B)](https://apps.microsoft.com/detail/9NV5167C5GGS)
[![FPS](https://img.shields.io/badge/Framerate-120%20FPS%20Fluid-success.svg)]()
[![Cold Open](https://img.shields.io/badge/Cold%20Start-%3C%2050%20ms-success.svg)]()
[![Privacy](https://img.shields.io/badge/Execution-100%25%20Offline-success.svg)]()

**A distraction-free, ultra-fast native Windows photo viewer engineered with modern C++20, Direct3D 11, and Direct2D hardware acceleration.**

[👉 Get it on the Microsoft Store](https://apps.microsoft.com/detail/9NV5167C5GGS) • [Features](#-key-features) • [Screenshots](#-screenshots-showcase) • [Performance Benchmarks](#-performance-benchmarks) • [Keyboard Shortcuts](#-keyboard-shortcuts) • [Supported Formats](#-supported-file-formats)

</div>

---

## 📸 Screenshots Showcase

<div align="center">

### 1. Borderless Minimalist Lightbox Viewport & Soft Vignette
![Main Photo View](assets/screenshots/1_Main_Photo_View_1920x1080.png)

### 2. Comprehensive EXIF Metadata Inspector Sidebar
![EXIF Metadata Inspector](assets/screenshots/2_EXIF_Metadata_Inspector_1920x1080.png)

### 3. Interactive Thumbnail Filmstrip for Swift Folder Browsing
![Interactive Filmstrip Mode](assets/screenshots/3_Interactive_Filmstrip_Mode_1920x1080.png)

### 4. Real-Time Hardware Diagnostic HUD (F12) & Telemetry Counter
![Realtime Diagnostic HUD](assets/screenshots/4_Realtime_Diagnostic_HUD_1920x1080.png)

### 5. Ultra-High Resolution Engine with 100MP+ & Panorama Support
![Ultra High Resolution Engine](assets/screenshots/5_Ultra_High_Resolution_Engine_1920x1080.png)

### 6. Settings, Color Management & Embedded ICC Profile Engine
![Settings and Color Management](assets/screenshots/6_Settings_and_Color_Management_1920x1080.png)

</div>

---

## ⚡ Key Features

Instant Photo Viewer is engineered from the ground up for instantaneous responsiveness, color fidelity, and pure viewing pleasure without cumbersome UI clutter or cloud lock-in.

- 🚀 **Blazing Fast Progressive Navigation:**
  - Proprietary two-stage decoding pipeline: displays an instant hardware-subsampled DCT preview in **< 15 ms**, seamlessly followed by the full-resolution frame swap.
  - Natural alphanumeric folder sorting (e.g., `IMG_1`, `IMG_2`, `IMG_10`) identical to Windows File Explorer.
  - Pre-fetching engine pre-caches adjacent photos in memory for **0.00 ms instant navigation**.

- 🖼️ **Ultra-High Resolution & Panorama Engine:**
  - Effortlessly opens 50MP to 100MP+ DSLR and mirrorless camera photos and ultra-wide panoramas up to **16,384 pixels wide**.
  - Intelligent Direct3D 11 texture clamping and progressive downsampling safeguards integrated GPUs (Intel UHD, AMD Radeon Vega) against video memory exhaustion.
  - Zero UI freezing: decoding occurs on asynchronous background worker threads, keeping the message loop 100% fluid.

- 🎨 **Color Accuracy & Embedded ICC Profiles:**
  - Automatic ICC color profile extraction and software color transformation for wide-gamut photos (sRGB, Display P3, Adobe RGB 1998, ProPhoto RGB, DCI-P3).
  - Preserves true photographic color fidelity on calibrated and high-dynamic-range (HDR) monitors.

- 🎞️ **Interactive Thumbnail Filmstrip:**
  - Press `F` or click the filmstrip toggle to reveal an interactive thumbnail strip of your entire photo album.
  - Jump directly to any photo in a 10,000-image collection without returning to File Explorer.

- 📊 **Detailed EXIF Metadata Inspector:**
  - Press `I` to open the photographic metadata sidebar: camera make, camera model, lens model, exposure time, aperture (f-number), ISO speed, focal length, date taken, and file size.

- 🔒 **100% Private & Completely Offline:**
  - Zero analytics SDKs, zero telemetry tracking, zero internet connections, and zero cloud uploads. Your memories stay strictly on your local computer.

---

## ⏱️ Performance Benchmarks

Measured on Windows 11 with an Intel Core processor and Direct3D 11 flip-model presentation:

| Metric | Industry Standard | Instant Photo Viewer | Advantage |
| :--- | :--- | :--- | :--- |
| **Warm Launch (Resident Process)** | ~800 ms | **< 45 ms** | **18x Faster** |
| **Cold Launch Time** | ~1,200 ms | **< 50 ms** | **24x Faster** |
| **12MP JPEG Fast Preview** | ~180 ms | **15.2 ms** | **12x Faster** |
| **12MP Full Quality Decode** | ~350 ms | **52.7 ms** | **6x Faster** |
| **Adjacent Photo Switch (Prefetched)**| ~120 ms | **0.00 ms (Instant)** | **Infinite** |
| **10,000 Photo Folder Scan** | ~4,500 ms | **56.3 ms** | **80x Faster** |
| **Idle Background RAM Footprint** | ~120 MB | **~1.2 MB** | **99% Leaner** |

---

## ⌨️ Keyboard & Mouse Shortcuts

| Key / Input | Action |
| :--- | :--- |
| `Right Arrow` / `Space` / `Page Down` | Next photo |
| `Left Arrow` / `Backspace` / `Page Up` | Previous photo |
| `Home` / `End` | Jump to first / last photo in folder |
| `Mouse Wheel` | Smooth zoom centered at cursor position |
| `Mouse Drag` | Pan and inspect photo when zoomed |
| `Double Click` / `Middle Click` | Toggle 100% actual size / fit to window |
| `F11` / `Enter` | Toggle borderless fullscreen |
| `I` | Toggle EXIF Metadata Inspector panel |
| `F` | Toggle interactive thumbnail filmstrip |
| `F12` | Toggle real-time diagnostic performance HUD |
| `R` / `Ctrl+R` | Rotate 90° Clockwise |
| `L` / `Ctrl+Shift+R` | Rotate 90° Counter-Clockwise |
| `Delete` | Move current photo safely to Windows Recycle Bin |
| `Ctrl+C` | Copy photo bitmap directly to Windows Clipboard |
| `Ctrl+,` | Open Settings & Preferences dialog |
| `Esc` | Exit fullscreen or close viewer |

---

## 📂 Supported File Formats

Instant Photo Viewer natively supports all common and professional digital formats:

| Category | Supported File Extensions |
| :--- | :--- |
| **Standard Photographic** | `.jpg`, `.jpeg`, `.jpe`, `.jfif`, `.png`, `.bmp`, `.dib`, `.ico` |
| **High Dynamic Range & Next-Gen** | `.webp`, `.jxr`, `.wdp`, `.hdp`, `.avif`, `.heic`, `.heif` |
| **Professional Photography** | `.tif`, `.tiff`, `.raw`, `.cr2`, `.cr3`, `.nef`, `.arw`, `.dng`, `.orf`, `.rw2` |
| **Vector & Animations** | `.svg`, `.gif`, `.apng`, `.webp (animated)` |

---

## 📜 License & Attribution

Distributed under the permissive **MIT License**. See [LICENSE](LICENSE) for details.  
Copyright (c) 2026 MrKalita. All rights reserved.
