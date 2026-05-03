# Changelog

## [1.0.0-beta.3] - 2026-05-03

### Fixed
- Flipper IR database import: non-standard carrier frequencies (e.g. 56 kHz
  for Dish) are now preserved and forwarded to the bridge on transmit
- Dev Docker build: `requirements.dev.txt` was incorrectly excluded from the
  build context via `.dockerignore`

### Documentation
- New dedicated hardware setup guide covering ESP32 board selection, IR
  wiring, ESPHome YAML configuration, and first-run walkthrough
- New `ir2mqtt_bridge` component reference with full config options,
  carrier frequency table per protocol, and status LED docs
- Automation recipes now include Mermaid flowcharts showing runtime logic
- IR database: documented code conversion internals, unsupported protocols
  (sharp, rca, sanyo, whynter, toshiba), and carrier frequency assumptions
- Corrected RC5 note: not an ESPHome bug — 36 kHz carrier mismatch with
  standard 38 kHz receiver modules

## 1.0.0-beta.2

- Bump app to 1.0.0-beta.2 (see app changelog for details)
