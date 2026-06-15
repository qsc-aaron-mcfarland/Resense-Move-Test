# Design: IWS / Resense Move — Test Plan Structure

## Test Organization

Test cases are organized into 7 sections under `Designer > Components > IWS`:

| # | Section | SRD Coverage | Approx Cases |
|---|---------|-------------|--------------|
| 1 | Component Basics | IWS-SW-1, IWS-SW-2 | ~12 |
| 2 | Sensor Technologies | IWS-ST-1 through IWS-ST-7 | ~18 |
| 3 | LED Configuration | IWS-LED-1 | ~10 |
| 4 | Peripheral Manager | IWS-PM-1, IWS-RB-1, IWS-SW-2 | ~15 |
| 5 | Control Pins | IWS-CP-1 | ~17 |
| 6 | Detection Zones | IWS-ST-3, IWS-ST-5 | ~11 |
| 7 | Persistence | IWS-SW-2 | ~6 |

## Output Format

- **TSV files** — one per section, paste-ready for Excel
- **Columns**: Title, Preconditions, Steps, Expected Results, Execution Type, Section
- All test cases default to `Manual` execution type

## Assumptions

- Tests use a **new design** with the IWS component added
- IWS device is network-reachable and commissioned unless the test is specifically about commissioning
- Q-SYS Designer is running on Windows
- No additional license required (IWS-SW-1: license-free)
- Q-SYS API pulls data from Distech API on device; we validate Q-SYS UI, not device internals

## Sensor Units Reference

| Sensor | Unit | Range |
|--------|------|-------|
| Luminosity | Lux | 0–4,000 |
| Temperature | °C | +5°C to +35°C |
| Humidity | % | — |
| Dewpoint | °C | — |
| Sound Level | dBA | — |
| TVOC | ppm | 0 - 100|
| People Count | integer | — |
| Occupancy State | boolean | — |

## Control Pin Reference

All control pin names are documented in `test-cases/00-pin-reference.tsv`.
**When pin names change**, update that file and find/replace the old display name across the TSV test case files.

### Pin Categories

| Category | Pins |
|----------|------|
| **Sensor** | Humidity, Luminosity, Temperature, Dewpoint, Sound Level, TVOC, Occupancy State, People Count |
| **Sensor Config** | Occupancy Timeout, Poll Rate |
| **LED** | LED Brightness, LED Color, LED Enable, LED Pattern, LED Speed |
| **Presence Zone** (×5) | Presence Zone N Enabled, Presence Zone N Name, Presence Zone N Presence |
| **Device Info** | Status, Hostname, Model ID, Framework Version, Kernel Version, System Uptime, CPU Temperature, Motherboard Temperature |
| **Device Control** | Identify |
| **Group** | Sensor Group |
| **Zone Data** | Zone JSON |

## Component Window Layout

The component window title is **"Intelligent Workspace Sensor"** and contains 3 tabs:

### Status Tab
| Section | Fields |
|---------|--------|
| Status | Status indicator, ID button (Identify) |
| (inline) | CPU Temp., Mobo Temp. |
| Network | Hostname, Model ID, System Uptime, Kernel Ver., Framework Ver. |
| Sensor Output | Luminosity, Temperature, Humidity, Dewpoint, Sound Level, TVOC, People Count, Occupancy |
| Timeout Settings | Timeout (mins), Poll Rate (secs) |
| Group | Sensor Group |

### LED Configuration Tab
LED color, brightness, enable, pattern, and speed controls.

### Occupancy Sensor Configuration Tab
Presence zone configuration (Zones 1–5: Enabled, Name, Presence).

## UI Navigation Convention

Steps reference Q-SYS Designer regions using this grammar:
- `Left Sidebar > Inventory` — inventory panel / tree
- `Center Workspace > Canvas` — schematic surface
- `Right Sidebar > Properties drawer` — component properties
- `Floating Window "Intelligent Workspace Sensor"` — component control window (3 tabs: Status, LED Configuration, Occupancy Sensor Configuration)
- `Peripheral Manager` — Configurator / Peripheral Manager dialog
