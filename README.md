# GammaLab OTA Distribution

Public machine-readable update channel for `GammaLab-ESP32`.

This repository intentionally contains no application source code, credentials, or signing private keys. Release automation publishes only:

- `latest.json` - signed release metadata
- `latest.sig` - detached Ed25519 signature of the exact `latest.json` bytes
- `firmware.bin` - ESP32 OTA application image

The authoritative source project remains private. Devices verify the manifest signature and firmware SHA256 before activating an update.
