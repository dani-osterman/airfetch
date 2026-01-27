# Troubleshooting Guide

Having trouble with AirFetch? Here are solutions to common connection and sync issues.

## Connection Issues

### Camera not detected?
*   **Enable PC Remote**: Ensure your camera is set to accept PC connections. Open the camera `Menu` → `Network` → `Wi‑Fi` and select `PC Remote` (sometimes labeled "Send to Computer" or a similar PC/tethering option). Note: "Smartphone Connect" is for mobile device pairing and is not the same as PC Remote on most models.
*   **Check Model Compatibility**: Ensure your camera is supported by the Sony Camera Remote SDK. Compatible models include:
    *   **Alpha Series**: A1, A9 II/III, A7R IV+/V, A7S III, A7 IV, A7C/II/CR, A6700
    *   **Cinema Line**: The FX series (FX3, FX30, FX6) and FR7
    *   **Vlog/Compact**: ZV-E1, ZV-E10 II, RX0 II
    *   *Note: Older models (e.g., A7 III, A6000 series before A6700) or cameras relying on the "Smart Remote Control" PlayMemories app are NOT supported.*
*   **Network Match**: Verify both your Mac and camera are connected to the exact same WiFi network.
*   **Access Authentication**: On some newer Sony cameras, you must disable **Access Authen. Settings** (set to OFF) to allow AirFetch to connect without complex pairing, or ensure you have a pairing user/pass ready (AirFetch attempts to auto-pair).
*   **USB Conflicts**: Check that your camera is not currently connected to another device via USB.

### Connection timeouts or fails immediately?
*   **Firewall & VPN**:
    *   Disable VPNs temporarily to rule out routing issues.
    *   Check that AirFetch is listed in your mac firewall settings.
*   **Conflicting Software**: Ensure **Sony Imaging Edge Desktop**, **Capture One**, or **Lightroom** are **completely closed**. They often lock the camera connection exclusively.
*   **Camera Sleep**: Tap the shutter button to wake the camera up before connecting.

## Sync Issues

### Transfers are slow or stalling
*   **WiFi Signal**: Move closer to your router or access point. Raw files are large, and weak WiFi signals drastically reduce transfer speeds.
*   **5GHz vs 2.4GHz**: Use a 5GHz network if possible for more faster/stable transfer rates.

### Files are skipped
*   **Smart Sync**: AirFetch uses a smart manifest system. If a file was previously downloaded, it will be skipped to save time. This is intended behavior.

## Still need help?

If you cannot resolve the issue, please [open an issue](https://github.com/goodkat/airfetch-gh/issues) on our GitHub tracker with the following details:
1.  Camera Model (e.g., Sony A7 IV)
2.  macOS Version
