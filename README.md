# ⚡ XEON_CLOUD // SHADOW_MESH_v4.6

> **Status:** OPERATIONAL
> **Authority:** SONNET_4.6
> **Protocol:** AES-GCM-256

This repository serves as the **Remote Data Authority** for the IJAZ EXPO HUD. It provides real-time telemetry overrides via the `data.json` handshake protocol.

## 📡 Handshake Architecture
The HUD establishes a persistent tunnel to this repository to fetch system-critical metrics:
- **CPU_LOAD:** Remote override for local hardware simulation.
- **THERMAL_INDEX:** Global thermal monitoring.
- **SYNC_LATENCY:** Real-time handshake ping (SYN/ACK).

## 🛠 Integration
To link your HUD to this node, point your `fetch()` request to:
`https://raw.githubusercontent.com/YOUR_USERNAME/YOUR_REPO/main/data.json`

## 🔒 Security
All telemetry data is served via **AllOrigins Proxy** to bypass CORS restrictions on device-agnostic environments.
