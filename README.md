# Aseprite Builder

[![Actions](https://img.shields.io/github/actions/workflow/status/inaniaehorrendum/aseprite-builder/builder.yml?branch=main&label=Actions&logo=github-actions&logoColor=white&color=238636)](https://github.com/inaniaehorrendum/aseprite-builder/actions)
[![License](https://custom-icon-badges.demolab.com/badge/License-EUPL--1.2-003399?logo=european-union&logoColor=FFCC00)](LICENSE)
[![Compliance](https://custom-icon-badges.demolab.com/badge/Compliance-EULA-003399?logo=law&logoColor=white)](https://github.com/aseprite/aseprite/blob/main/EULA.txt)
[![Platform](https://custom-icon-badges.demolab.com/badge/Windows_x64-00A4EF?logo=windows11&logoColor=white)](#)

## Legal Information

This repo contains autobuild script only. It doesn't contain Aseprite source code or binaries.

Compilation and usage of Aseprite are governed by [Aseprite EULA](https://github.com/aseprite/aseprite/blob/main/EULA.txt). To ensure compliance, this workflow generates **Draft Releases**, which remain private and visible only to the repo owner.

## Highlights

- **Pure Distribution:** Compiled with `-DENABLE_OPENSSL=OFF` and `-DENABLE_CURL=OFF`. Removes dependencies for true portable exe.
- **Modern Skia:** Utilizes the Skia m124 branch, ensuring full compat with Aseprite v1.3+.

## Usage

1. **Fork** or use this repo template.
2. Navigate to **Settings > Actions > General**.
3. Set **Workflow permissions >** `Read and write permissions`.
4. Enable **Allow all actions and reusable workflows**.
5. Use workflow manual or wait daily schedule (**00:00 UTC**).

## [![CMake](https://custom-icon-badges.demolab.com/badge/CMake-064F8C?logo=cmake&logoColor=white)](#)

```cmake
-DENABLE_OPENSSL=OFF
-DENABLE_CURL=OFF
-DENABLE_WEBSOCKET=OFF
-DENABLE_NEWS=OFF
-DENABLE_UPDATER=OFF