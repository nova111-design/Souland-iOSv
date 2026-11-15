# Souland.net — iOS starter

This repository contains an **iOS WebKit wrapper** and a **mobile UI prototype**, NOT a playable Tibia client.

## Build on GitHub Actions (no Mac required locally)
1. Upload all files/folders from this package to the root of the private `Souland-iOSv` repository (keep `.github/workflows/ios-build.yml`).
2. Open **Actions → Build iOS test IPA → Run workflow**.
3. Download artifact `Souland-iOS-unsigned` after a successful run.
4. Unzip artifact to get `Souland-iOS-unsigned.ipa`; sign/install using Sideloadly and your own Apple ID on Windows.

The workflow has not been executed here. An unsigned IPA requires signing to install; free Apple ID signing may require renewal.

## What it does
- Native SwiftUI shell with landscape WKWebView opening `https://souland.net/mobile/`.
- Midnight Sapphire theme and branded icon.
- `web/index.html` is a standalone mobile control-selection **prototype**. Upload it to `/mobile/index.html` on your website if you want to see the placeholder page inside the app.

## What is NOT implemented
- Tibia 7.92 game engine / WebAssembly client.
- Login protocol, server authentication, character rendering, battle, spells, and actual joystick movement.
- WebSocket-to-TCP gateway and production security controls.
- Device testing, App Store provisioning, signed distributable IPA.

To make it playable, integrate and validate a compatible web game client with Souland 1.1 before publishing it to players.
