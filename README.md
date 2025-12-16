# Flipper-Zero-PC-Monitor-USB-Backend
Backend for **PC Monitor (USB Version)** written in Rust.

This backend collects system statistics (CPU, RAM, GPU) and sends them to the Flipper Zero via USB Serial (CDC).

**Please note that GPU info is only displayed on Nvidia cards (inherited from original project).**

## How to run
1. Connect your Flipper Zero via USB.
2. Launch the **PC Monitor USB** app on the Flipper.
3. Run this backend:
   ```bash
   cargo run --release
   ```
   Or build it and run the binary:
   ```bash
   cargo build --release
   ./target/release/flipper-pc-monitor-backend-usb
   ```

The backend automatically detects the Flipper Zero (VID: 0x0483, PID: 0x5740).

## Credits & Acknowledgments
- **Original Backend**: [TheSainEyereg](https://github.com/TheSainEyereg/flipper-pc-monitor-backend)
- **USB Adaptation**: [DonJulve](https://github.com/DonJulve)
