# XEON Cloud Handshake Protocol

This repository serves as the remote authority for the **IJAZ EXPO HUD**. 

### 📡 Features
- **Remote Handshake:** Automated SYN/ACK sequence for secure data tunneling.
- **Telemetry Mapping:** Real-time injection of CPU, Thermal, and Latency metrics.
- **Nexus variable integration:** Styled using the `--nexus` purple architecture.

### 🛠 Deployment
1. Update `data.json` with new hardware parameters.
2. The HUD will automatically poll this repository's 'Raw' endpoint.
3. Observe the `sys-feed` in the Nexus panel for connection logs.
