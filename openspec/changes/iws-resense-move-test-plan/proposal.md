# Proposal: IWS / Resense Move — Comprehensive Q-SYS Designer Test Plan

## What

Create a comprehensive SQE test plan covering functional and GUI-level validation of the Resense Move (IWS) component as a native Q-SYS peripheral in Q-SYS Designer. Test cases are authored in TSV format for Excel storage and future TestRail XML conversion.

## Why

The U115 Resense Move (IWS) — Phase 1 brings the Distech Resense Move multi-sensor device into the Q-SYS ecosystem as a native peripheral. A thorough test plan is required to validate all PRD and SRD requirements before Summer 2026 launch. This plan covers:

- Component basics (inventory, schematic, properties)
- Sensor technologies (occupancy, people count, luminosity, temperature, humidity, TVOC, sound level)
- LED ring configuration (color, brightness, patterns)
- Peripheral Manager workflows (discovery, commissioning, firmware update)
- Control pins (sensor data I/O, status communication)
- Detection / presence zones
- Persistence (save/close/reopen design)

## References

- PRD: PRD - U115 Resense Move - IWS
- SRD: SRD - U115 Resense Move - IWS
- SRD Requirement IDs: IWS-SW-1, IWS-SW-2, IWS-CP-1, IWS-ST-3, IWS-ST-4/5, IWS-PM-1, IWS-RB-1

## Non-goals

- Device-level firmware/hardware testing (Distech responsibility)
- Unit tests, API-level assertions, code instrumentation
- Reflect integration testing (separate scope)
- Bluetooth qualification testing
