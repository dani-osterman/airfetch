# AirFetch

**AirFetch** is a macOS menu bar app for wirelessly syncing photos from Sony cameras. It uses a custom implementation of PTP-IP to transfer files quickly and efficiently without cables.

> **Note**: This repository serves as the public hub for AirFetch releases, issue tracking, and documentation. The core application logic resides in a separate private repository.

## Features

- **Automatic Discovery**: Instantly finds Sony cameras on your network.
- **Smart Sync**: Incrementally backs up your files, skipping data you've already transferred.
- **Wireless**: Works over standard WiFi using PTP-IP.
- **Native macOS Experience**: Lives in your menu bar, designed with SwiftUI.

## Supported Cameras

Currently, AirFetch is optimized for **Sony cameras** with WiFi capability (PC Remote function).

Supported models include:
- Sony Alpha series (A7, A9, A6xxx, etc.)
- Sony RX series
- Other Sony models supporting the "PC Remote" connection method.

*The app is built with an extensible architecture, allowing for potential support of other camera manufacturers in the future.*

## Downloads

Support for Apple Silicon macOS.

[**Download Latest Release**](https://github.com/goodkat/airfetch-gh/releases)

## Quick Start

1.  **Prepare your Camera**:
    *   Go to `Menu` → `Network` → `Wi-Fi` (or `Connect`).
    *   Enable **PC Remote** (sometimes called **Send to Computer** or **Ctrl with Smartphone/PC** depending on the model).
    *   Connect your camera to the same WiFi network as your Mac (Infrastructure mode) or connect your Mac to the camera's hotspot (Access Point mode).
2.  **Run AirFetch**:
    *   Launch the app from your Applications folder.
    *   Click the AirFetch icon in the menu bar.
3.  **Sync**:
    *   Select your camera from the detected list.
    *   Choose a destination folder on your Mac.
    *   Click **Sync** to start transferring.

## Troubleshooting

### Camera not detected?
*   Ensure your camera is in **PC Remote** mode (not Mass Storage or MTP).
*   Verify both devices are on the exact same network subnet.
*   Try toggling the camera's WiFi off and back on.
*   Check that your camera is not currently connected to another device via USB.

### Connection timeouts or authentication failures?
*   Check your firewall settings. AirFetch needs to communicate on:
    *   UDP ports 1900 & 64321 (Discovery)
    *   TCP port 15740 (Data Transfer)
*   Ensure no other Sony imaging software (like Imaging Edge or Remote) is running and holding the connection.
*   If using a VPN, try disabling it temporarily.

### Sync issues?
*   Make sure the camera hasn't gone to sleep during the process.
*   Verify you have write permissions for the selected destination folder.
