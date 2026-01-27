# Troubleshooting Guide

Having trouble with AirFetch? Here are solutions to common connection and sync issues.

## Connection Issues

### Camera not detected?
*   **Enable PC Remote**: Ensure your camera is in **PC Remote** (or "Send to Computer") mode. Check `Menu` → `Network` → `Smartphone Connect` or `Transfer/Remote`.
*   **Network Match**: Verify both your Mac and camera are connected to the exact same WiFi network.
*   **Access Authentication**: On some newer Sony cameras, you must disable **Access Authen. Settings** (set to OFF) to allow AirFetch to connect without complex pairing, or ensure you have a pairing user/pass ready (AirFetch attempts to auto-pair).
*   **USB Conflicts**: Check that your camera is not currently connected to another device via USB.

### Connection timeouts or fails immediately?
*   **Firewall & VPN**:
    *   Disable VPNs temporarily to rule out routing issues.
    *   Allow AirFetch through your firewall if prompted. The Sony SDK requires UDP ports 1900 & 64321 and dynamic TCP ports.
*   **Conflicting Software**: Ensure **Sony Imaging Edge Desktop**, **Capture One**, or **Lightroom** are **completely closed**. They often lock the camera connection exclusively.
*   **Camera Sleep**: Tap the shutter button to wake the camera up before connecting.

## Sync Issues

### Transfers are slow or stalling
*   **WiFi Signal**: Move closer to your router or access point. Raw files are large, and weak WiFi signals drastically reduce transfer speeds.
*   **5GHz vs 2.4GHz**: Use a 5GHz network if possible for significantly faster transfer rates.

### Files are skipped
*   **Smart Sync**: AirFetch uses a smart manifest system. If a file was previously downloaded, it will be skipped to save time. This is intended behavior.

## Still need help?

If you cannot resolve the issue, please [open an issue](https://github.com/goodkat/airfetch-gh/issues) on our GitHub tracker with the following details:
1.  Camera Model (e.g., Sony A7 IV)
2.  macOS Version
3.  Connection Method (Infrastructure WiFi or Camera Access Point)
