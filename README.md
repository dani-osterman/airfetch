![Banner](assets/Banner.png)

### ⚠️ Currently not in active development due to other projects and limitiations in Sony SDK for XML transfer. Might get updated later.

# AirFetch

**AirFetch** is a macOS menu bar utility for wireless file syncing from camera to your mac. Currently exclusively supporting **Sony cameras**, it delivers reliability, ease-of-use, and seamless integration into your photography workflow.

[![Download Latest](https://img.shields.io/badge/Download-Latest-blue?style=for-the-badge&logo=github)](https://github.com/dani-osterman/airfetch/releases/tag/v.0.1.0-stable)

### Support development

Consider sponsoring AirFetch. Contributions help us maintain the project and develop compatibility for other camera manufacturers (Canon, Nikon, Fuji, Panasonic).

[![Sponsor](https://img.shields.io/badge/Sponsor-GitHub-brightgreen?style=flat&logo=github)](https://github.com/sponsors/dani-osterman)

### Why AirFetch?

| <img src="assets/tick.svg" width="64"> | <img src="assets/wifi.svg" width="64"> | <img src="assets/apple.svg" width="64"> |
| :---: | :---: | :---: |
| **Reliability** | **Wireless Syncing** | **Native macOS Design** |
| Stable pairing and file transfer. Native compatibility for the latest **Sony Alpha** cameras. | Automatic detection and **Smart Sync** (transfers new files only). Runs silently in the background. | Built with **Swift** and **SwiftUI**. A lightweight menu bar utility that fits the ecosystem. |


## Supported Cameras

AirFetch currently supports **Sony cameras** capable of "PC Remote" functionality via WiFi. 

Detection and transfers are powered by the **official Sony Camera Remote SDK**, ensuring compatibility with:

**Alpha Series**: A1, A9 II/III, A7R IV+/V, A7S III, A7 IV, A7C/II/CR, A6700<br>
**Cinema Line**: The FX series (FX3, FX30, FX6) and FR7<br>
**Vlog/Compact**: ZV-E1, ZV-E10 II, RX0 II

## Downloads

- **Supported platforms:** macOS 13.0 or later (Apple Silicon)
- **Package:** DMG for Apple Silicon available from the Releases page; universal builds are not provided at this time
- **Notarization:** Final signed & notarized DMG will be published later. Builds may be unsigned.

[**See all releases**](https://github.com/dani-osterman/airfetch/releases)

## Quick Start

1.  **Prepare Camera**:
    *   Turn on the **Wifi connect**
    *   Set **PC Remote** on. (might differ based on model)
2.  **Launch AirFetch**:
    *   Open the app; it sits in your menu bar.
3.  **Sync**:
    *   Select your camera from the dropdown.
    *   Pick a destination folder.
    *   Hit **Sync**.

## Support & Commercial Use

### Troubleshooting
Encountering connection issues? Read our [**Troubleshooting Guide**](troubleshooting/TROUBLESHOOTING.md) for detailed solutions regarding firewalls, router settings, and camera configurations.

### License
AirFetch is free for personal and professional use. See [LICENSE](LICENSE) for full terms.

---

<p>
  <sub>Copyright © 2026 AirFetch. All rights reserved.</sub>
</p>
