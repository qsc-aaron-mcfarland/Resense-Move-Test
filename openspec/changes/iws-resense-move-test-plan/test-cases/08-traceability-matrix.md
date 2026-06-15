# Traceability Matrix

| Test Case Title | Test Section | SRD Req ID | Jira Story | Jira Story Title | Notes |
|---|---|---|---|---|---|
| IWS - Verify component available in inventory | Component Basics | IWS-COMP-2 | QSYSDEV-53104 | Implement Control of IWS - device_lib / control_lib / designer components | Designer inventory presence |
| IWS - Add component to schematic via drag and drop | Component Basics | IWS-COMP-2 | QSYSDEV-53104 | Implement Control of IWS - device_lib / control_lib / designer components | |
| IWS - Verify default component properties | Component Basics | IWS-COMP-2 | QSYSDEV-58457 | IWS - Q-SYSify defaults of Resense Move | Default property values |
| IWS - Rename component | Component Basics | IWS-COMP-2 | QSYSDEV-53104 | Implement Control of IWS - device_lib / control_lib / designer components | |
| IWS - Rename component with special characters | Component Basics | IWS-COMP-2 | QSYSDEV-53104 | Implement Control of IWS - device_lib / control_lib / designer components | |
| IWS - Add multiple IWS components | Component Basics | IWS-COMP-2 | QSYSDEV-53104 | Implement Control of IWS - device_lib / control_lib / designer components | |
| IWS - Delete component from design | Component Basics | IWS-COMP-2 | QSYSDEV-53104 | Implement Control of IWS - device_lib / control_lib / designer components | |
| IWS - Double-click to open component window | Component Basics | IWS-COMP-2, IWS-DI-1 | QSYSDEV-56207 | IWS control panel (QDS) UX Implementation | Verifies 3 tabs: Status, LED Configuration, Occupancy Sensor Configuration |
| IWS - Verify no license required | Component Basics | IWS-SW-1 | QSYSDEV-51758 | License Free IWS-SW-1 | |
| IWS - Verify Sensor Group configuration | Component Basics | IWS-COMP-2 | QSYSDEV-56207 | IWS control panel (QDS) UX Implementation | Status tab group field |
| IWS - Verify Timeout setting in minutes | Component Basics | IWS-ST-2 | QSYSDEV-51747 | People Counting and Presence Detection Reporting & Configuration IWS-ST-2/3 | Timeout Settings section |
| IWS - Verify Poll Rate setting in seconds | Component Basics | IWS-ST-2 | QSYSDEV-53104 | Implement Control of IWS - device_lib / control_lib / designer components | Timeout Settings section |
| IWS - Verify Status tab Network section displays device info | Component Basics | IWS-DI-1 | QSYSDEV-56207 | IWS control panel (QDS) UX Implementation | |
| IWS - Verify ID button triggers device identification | Component Basics | IWS-LED-2 | QSYSDEV-51745 | LED Configuration and Presets IWS-LED-1/2 | ID behavior: Blue, 100%, Flashing, Standard |
| IWS - Verify CPU Temp and Mobo Temp display | Component Basics | IWS-DI-1 | QSYSDEV-56207 | IWS control panel (QDS) UX Implementation | |
| IWS - Verify Bluetooth is not available | Component Basics | IWS-BLE-1 | QSYSDEV-53097 | Minimize resense services | Bluetooth out of scope for Phase 1; verify not exposed |
| IWS - Verify status indicator shows Fault when device is not connected | Component Basics | IWS-ST-10 | QSYSDEV-51756 | Fault Status IWS-ST-10 | Status bar turns red with "Fault" text when device is not connected |
| IWS - Verify occupancy detection status displays | Sensor Technologies | IWS-ST-2 | QSYSDEV-51747 | People Counting and Presence Detection Reporting & Configuration IWS-ST-2/3 | |
| IWS - Verify people count displays correctly | Sensor Technologies | IWS-ST-2 | QSYSDEV-51747 | People Counting and Presence Detection Reporting & Configuration IWS-ST-2/3 | |
| IWS - Verify people count with zero occupants | Sensor Technologies | IWS-ST-2 | QSYSDEV-51747 | People Counting and Presence Detection Reporting & Configuration IWS-ST-2/3 | |
| IWS - Verify luminosity sensor value and unit | Sensor Technologies | IWS-ST-4, IWS-ST-5 | QSYSDEV-51749 | Luminosity Sensing and Level Calibration ISW-ST-4/5 | |
| IWS - Verify luminosity sensor boundary at 0 Lux | Sensor Technologies | IWS-ST-4, IWS-ST-5 | QSYSDEV-51749 | Luminosity Sensing and Level Calibration ISW-ST-4/5 | |
| IWS - Verify luminosity sensor boundary at max Lux | Sensor Technologies | IWS-ST-4, IWS-ST-5 | QSYSDEV-51749 | Luminosity Sensing and Level Calibration ISW-ST-4/5 | |
| IWS - Verify temperature sensor value in Celsius | Sensor Technologies | IWS-ST-6 | QSYSDEV-53104 | Implement Control of IWS - device_lib / control_lib / designer components | No dedicated story for IWS-ST-6; covered by component implementation |
| IWS - Verify temperature sensor value in Fahrenheit | Sensor Technologies | IWS-ST-6 | QSYSDEV-53104 | Implement Control of IWS - device_lib / control_lib / designer components | |
| IWS - Verify humidity sensor value and unit | Sensor Technologies | IWS-ST-7 | QSYSDEV-53104 | Implement Control of IWS - device_lib / control_lib / designer components | No dedicated story for IWS-ST-7 |
| IWS - Verify TVOC sensor value and unit | Sensor Technologies | IWS-ST-8 | QSYSDEV-53104 | Implement Control of IWS - device_lib / control_lib / designer components | No dedicated story for IWS-ST-8 |
| IWS - Verify sound level sensor value and unit | Sensor Technologies | IWS-ST-9 | QSYSDEV-53104 | Implement Control of IWS - device_lib / control_lib / designer components | No dedicated story for IWS-ST-9 |
| IWS - Verify all sensor values update in near real-time | Sensor Technologies | IWS-ST-1 | QSYSDEV-53104 | Implement Control of IWS - device_lib / control_lib / designer components | |
| IWS - Verify sensor values when device is disconnected | Sensor Technologies | IWS-ST-1 | QSYSDEV-51756 | Fault Status IWS-ST-10 | Fault/disconnect state |
| IWS - Verify sensor values restore after reconnection | Sensor Technologies | IWS-ST-1 | QSYSDEV-53104 | Implement Control of IWS - device_lib / control_lib / designer components | |
| IWS - Verify dewpoint sensor value | Sensor Technologies | IWS-ST-10 | QSYSDEV-53104 | Implement Control of IWS - device_lib / control_lib / designer components | |
| IWS - Verify all sensor types are listed | Sensor Technologies | IWS-ST-1 | QSYSDEV-56207 | IWS control panel (QDS) UX Implementation | Status tab > Sensor Output section |
| IWS - Verify sensor data with multiple IWS devices | Sensor Technologies | IWS-ST-1 | QSYSDEV-53104 | Implement Control of IWS - device_lib / control_lib / designer components | |
| IWS - Verify sensor data display in emulate mode | Sensor Technologies | IWS-SW-2 | QSYSDEV-53104 | Implement Control of IWS - device_lib / control_lib / designer components | |
| IWS - Verify sensor reading precision and formatting | Sensor Technologies | IWS-ST-1 | QSYSDEV-55467 | Units as control | Sensor unit text fields |
| IWS - Verify sensor fault status reporting | Sensor Technologies | IWS-ST-10 | QSYSDEV-51756 | Fault Status IWS-ST-10 | Per-sensor fault state; also QSYSDEV-55466 |
| IWS - Verify LED ring color control available | LED Configuration | IWS-LED-1 | QSYSDEV-51745 | LED Configuration and Presets IWS-LED-1/2 | |
| IWS - Set LED ring to a specific color | LED Configuration | IWS-LED-1 | QSYSDEV-51745 | LED Configuration and Presets IWS-LED-1/2 | |
| IWS - Set LED ring brightness to maximum | LED Configuration | IWS-LED-1 | QSYSDEV-51745 | LED Configuration and Presets IWS-LED-1/2 | Default brightness = 100% |
| IWS - Set LED ring brightness to minimum | LED Configuration | IWS-LED-1 | QSYSDEV-51745 | LED Configuration and Presets IWS-LED-1/2 | |
| IWS - Set LED ring brightness to midrange value | LED Configuration | IWS-LED-1 | QSYSDEV-51745 | LED Configuration and Presets IWS-LED-1/2 | |
| IWS - Turn LED ring off | LED Configuration | IWS-LED-1 | QSYSDEV-51745 | LED Configuration and Presets IWS-LED-1/2 | Default = Off after power up |
| IWS - Turn LED ring on after being off | LED Configuration | IWS-LED-1 | QSYSDEV-51745 | LED Configuration and Presets IWS-LED-1/2 | |
| IWS - Cycle through multiple LED colors | LED Configuration | IWS-LED-1 | QSYSDEV-51745 | LED Configuration and Presets IWS-LED-1/2 | |
| IWS - Verify LED control with device disconnected | LED Configuration | IWS-LED-1 | QSYSDEV-51745 | LED Configuration and Presets IWS-LED-1/2 | |
| IWS - Verify LED settings via control pins | LED Configuration | IWS-LED-1, IWS-CP-1 | QSYSDEV-51745 | LED Configuration and Presets IWS-LED-1/2 | LED Color, Brightness, Enable, Pattern, Speed pins |
| IWS - Verify LED Pattern control | LED Configuration | IWS-LED-1 | QSYSDEV-51745 | LED Configuration and Presets IWS-LED-1/2 | Same pattern options as NM-T1 |
| IWS - Verify LED Speed control | LED Configuration | IWS-LED-1 | QSYSDEV-51745 | LED Configuration and Presets IWS-LED-1/2 | Same speed options as NM-T1 |
| IWS - Verify device appears in Peripheral Manager discovery | Peripheral Manager | IWS-PM-1 | QSYSDEV-53099 | Implement QDP (Q-SYS Discovery Protocol) on resense | QDP discovery |
| IWS - Commission a discovered IWS device | Peripheral Manager | IWS-PM-1 | QSYSDEV-53100 | Implement QPM (Q-SYS Peripheral Manager) on resense (IWS-PM-1) | |
| IWS - Commission with incorrect credentials | Peripheral Manager | IWS-PM-1 | QSYSDEV-53100 | Implement QPM (Q-SYS Peripheral Manager) on resense (IWS-PM-1) | See also bug QSYSDEV-60405 |
| IWS - Commission with empty credentials | Peripheral Manager | IWS-PM-1 | QSYSDEV-53100 | Implement QPM (Q-SYS Peripheral Manager) on resense (IWS-PM-1) | |
| IWS - Decommission a commissioned device | Peripheral Manager | IWS-PM-1 | QSYSDEV-53100 | Implement QPM (Q-SYS Peripheral Manager) on resense (IWS-PM-1) | |
| IWS - Verify firmware version displayed | Peripheral Manager | IWS-SW-2 | QSYSDEV-53101 | Implement QFU (Q-SYS Firmware Updates) for resense | |
| IWS - Firmware update when update is available | Peripheral Manager | IWS-SW-2 | QSYSDEV-53101 | Implement QFU (Q-SYS Firmware Updates) for resense | Also QSYSDEV-59810 (Peripheral firmware infrastructure) |
| IWS - Firmware update when device is already up to date | Peripheral Manager | IWS-SW-2 | QSYSDEV-53101 | Implement QFU (Q-SYS Firmware Updates) for resense | |
| IWS - Verify device status indicators in Peripheral Manager | Peripheral Manager | IWS-PM-1 | QSYSDEV-53100 | Implement QPM (Q-SYS Peripheral Manager) on resense (IWS-PM-1) | |
| IWS - Verify Peripheral Manager status when device goes offline | Peripheral Manager | IWS-PM-1 | QSYSDEV-53100 | Implement QPM (Q-SYS Peripheral Manager) on resense (IWS-PM-1) | |
| IWS - Verify Peripheral Manager status when device comes back online | Peripheral Manager | IWS-PM-1, IWS-RB-1 | QSYSDEV-53100 | Implement QPM (Q-SYS Peripheral Manager) on resense (IWS-PM-1) | Also QSYSDEV-51757 (Reset Button IWS RB-1) |
| IWS - Assign IWS device to component in design | Peripheral Manager | IWS-PM-1 | QSYSDEV-53100 | Implement QPM (Q-SYS Peripheral Manager) on resense (IWS-PM-1) | |
| IWS - Reassign IWS device to a different component | Peripheral Manager | IWS-PM-1 | QSYSDEV-53100 | Implement QPM (Q-SYS Peripheral Manager) on resense (IWS-PM-1) | |
| IWS - Verify device discovery with multiple IWS devices | Peripheral Manager | IWS-PM-1 | QSYSDEV-53099 | Implement QDP (Q-SYS Discovery Protocol) on resense | |
| IWS - Verify Peripheral Manager with device password change | Peripheral Manager | IWS-PM-1 | QSYSDEV-51760 | Security IWS-SW-2 | Credential management; see also bug QSYSDEV-60405 |
| IWS - Verify all control pins are listed | Control Pins | IWS-CP-1 | QSYSDEV-53104 | Implement Control of IWS - device_lib / control_lib / designer components | |
| IWS - Verify "Occupancy State" control pin value | Control Pins | IWS-CP-1 | QSYSDEV-51747 | People Counting and Presence Detection Reporting & Configuration IWS-ST-2/3 | |
| IWS - Verify "People Count" control pin value | Control Pins | IWS-CP-1 | QSYSDEV-51747 | People Counting and Presence Detection Reporting & Configuration IWS-ST-2/3 | |
| IWS - Verify "Luminosity" control pin value | Control Pins | IWS-CP-1 | QSYSDEV-51749 | Luminosity Sensing and Level Calibration ISW-ST-4/5 | |
| IWS - Verify "Temperature" control pin value | Control Pins | IWS-CP-1 | QSYSDEV-53104 | Implement Control of IWS - device_lib / control_lib / designer components | |
| IWS - Verify "Humidity" control pin value | Control Pins | IWS-CP-1 | QSYSDEV-53104 | Implement Control of IWS - device_lib / control_lib / designer components | |
| IWS - Verify "Dewpoint" control pin value | Control Pins | IWS-CP-1 | QSYSDEV-53104 | Implement Control of IWS - device_lib / control_lib / designer components | |
| IWS - Verify "TVOC" control pin value | Control Pins | IWS-CP-1 | QSYSDEV-53104 | Implement Control of IWS - device_lib / control_lib / designer components | |
| IWS - Verify "Sound Level" control pin value | Control Pins | IWS-CP-1 | QSYSDEV-53104 | Implement Control of IWS - device_lib / control_lib / designer components | |
| IWS - Verify "Status" control pin value | Control Pins | IWS-CP-1 | QSYSDEV-55466 | Fault state as control | Per-sensor fault state exposed as control pin |
| IWS - Verify "Identify" control pin triggers device identification | Control Pins | IWS-LED-2 | QSYSDEV-51745 | LED Configuration and Presets IWS-LED-1/2 | ID: Blue, 100%, Flashing, Standard |
| IWS - Verify "LED Brightness" control pin | Control Pins | IWS-CP-1, IWS-LED-1 | QSYSDEV-51745 | LED Configuration and Presets IWS-LED-1/2 | |
| IWS - Verify "LED Color" control pin | Control Pins | IWS-CP-1, IWS-LED-1 | QSYSDEV-51745 | LED Configuration and Presets IWS-LED-1/2 | |
| IWS - Verify "LED Enable" control pin | Control Pins | IWS-CP-1, IWS-LED-1 | QSYSDEV-51745 | LED Configuration and Presets IWS-LED-1/2 | |
| IWS - Verify "LED Pattern" control pin | Control Pins | IWS-CP-1, IWS-LED-1 | QSYSDEV-51745 | LED Configuration and Presets IWS-LED-1/2 | |
| IWS - Verify "LED Speed" control pin | Control Pins | IWS-CP-1, IWS-LED-1 | QSYSDEV-51745 | LED Configuration and Presets IWS-LED-1/2 | |
| IWS - Verify "Occupancy Timeout" control pin | Control Pins | IWS-CP-1, IWS-ST-2 | QSYSDEV-51747 | People Counting and Presence Detection Reporting & Configuration IWS-ST-2/3 | |
| IWS - Verify "Poll Rate" control pin | Control Pins | IWS-CP-1 | QSYSDEV-53104 | Implement Control of IWS - device_lib / control_lib / designer components | |
| IWS - Verify device info pins display correct values | Control Pins | IWS-CP-1, IWS-DI-1 | QSYSDEV-53104 | Implement Control of IWS - device_lib / control_lib / designer components | Hostname, Model ID, Framework Version, Kernel Version, System Uptime |
| IWS - Verify "CPU Temperature" and "Motherboard Temperature" pins | Control Pins | IWS-CP-1, IWS-DI-1 | QSYSDEV-53104 | Implement Control of IWS - device_lib / control_lib / designer components | |
| IWS - Verify "Zone JSON" control pin outputs valid JSON | Control Pins | IWS-CP-1, IWS-ST-3 | QSYSDEV-51747 | People Counting and Presence Detection Reporting & Configuration IWS-ST-2/3 | |
| IWS - Verify Presence Zone control pins (per zone) | Control Pins | IWS-CP-1, IWS-ST-3 | QSYSDEV-51747 | People Counting and Presence Detection Reporting & Configuration IWS-ST-2/3 | Zones 1-5: Enabled, Name, Presence |
| IWS - Verify control pin values update in real-time | Control Pins | IWS-CP-1 | QSYSDEV-53104 | Implement Control of IWS - device_lib / control_lib / designer components | |
| IWS - Verify control pin values when device is disconnected | Control Pins | IWS-CP-1 | QSYSDEV-51756 | Fault Status IWS-ST-10 | Fault/disconnect behavior |
| IWS - Connect control pins via wiring on canvas | Control Pins | IWS-CP-1 | QSYSDEV-53104 | Implement Control of IWS - device_lib / control_lib / designer components | |
| IWS - Verify control pin naming convention | Control Pins | IWS-CP-1 | QSYSDEV-53104 | Implement Control of IWS - device_lib / control_lib / designer components | iws_ prefix convention |
| IWS - Verify presence zones configuration UI available | Detection Zones | IWS-ST-3 | QSYSDEV-51747 | People Counting and Presence Detection Reporting & Configuration IWS-ST-2/3 | Occupancy Sensor Configuration tab |
| IWS - Verify default detection zones | Detection Zones | IWS-ST-3 | QSYSDEV-51747 | People Counting and Presence Detection Reporting & Configuration IWS-ST-2/3 | |
| IWS - Add a new detection zone | Detection Zones | IWS-ST-3 | QSYSDEV-51747 | People Counting and Presence Detection Reporting & Configuration IWS-ST-2/3 | Inclusion zones |
| IWS - Remove a detection zone | Detection Zones | IWS-ST-3 | QSYSDEV-51747 | People Counting and Presence Detection Reporting & Configuration IWS-ST-2/3 | |
| IWS - Rename a detection zone | Detection Zones | IWS-ST-3 | QSYSDEV-51747 | People Counting and Presence Detection Reporting & Configuration IWS-ST-2/3 | Presence Zone N Name pin |
| IWS - Verify presence detection per zone | Detection Zones | IWS-ST-3, IWS-ST-5 | QSYSDEV-51747 | People Counting and Presence Detection Reporting & Configuration IWS-ST-2/3 | |
| IWS - Verify people count per zone | Detection Zones | IWS-ST-3 | QSYSDEV-51747 | People Counting and Presence Detection Reporting & Configuration IWS-ST-2/3 | |
| IWS - Verify zone-specific control pins are exposed | Detection Zones | IWS-ST-3, IWS-CP-1 | QSYSDEV-51747 | People Counting and Presence Detection Reporting & Configuration IWS-ST-2/3 | |
| IWS - Verify maximum of 5 presence zones | Detection Zones | IWS-ST-3 | QSYSDEV-51747 | People Counting and Presence Detection Reporting & Configuration IWS-ST-2/3 | 5 zone max per control pins |
| IWS - Verify detection zone boundaries do not overlap error handling | Detection Zones | IWS-ST-3 | QSYSDEV-51747 | People Counting and Presence Detection Reporting & Configuration IWS-ST-2/3 | |
| IWS - Verify detection zones persist after save and reopen | Detection Zones | IWS-ST-3, IWS-SW-2 | QSYSDEV-51747 | People Counting and Presence Detection Reporting & Configuration IWS-ST-2/3 | |
| IWS - Verify component properties persist after save and reopen | Persistence | IWS-SW-2 | QSYSDEV-53104 | Implement Control of IWS - device_lib / control_lib / designer components | |
| IWS - Verify LED configuration persists after save and reopen | Persistence | IWS-SW-2, IWS-LED-2 | QSYSDEV-51745 | LED Configuration and Presets IWS-LED-1/2 | SRD: LED settings recall (presets) |
| IWS - Verify control pin wiring persists after save and reopen | Persistence | IWS-SW-2 | QSYSDEV-53104 | Implement Control of IWS - device_lib / control_lib / designer components | |
| IWS - Verify Peripheral Manager assignment persists after save and reopen | Persistence | IWS-SW-2, IWS-PM-1 | QSYSDEV-53100 | Implement QPM (Q-SYS Peripheral Manager) on resense (IWS-PM-1) | |
| IWS - Verify design with IWS component can be saved as a new file | Persistence | IWS-SW-2 | QSYSDEV-53104 | Implement Control of IWS - device_lib / control_lib / designer components | |
| IWS - Verify multiple IWS components persist independently | Persistence | IWS-SW-2 | QSYSDEV-53104 | Implement Control of IWS - device_lib / control_lib / designer components | |
| IWS - Verify LLDP is enabled on single Resense Move | LLDP / Network | | | | LLDP discovery for single device |
| IWS - Verify single Resense Move network topology in Q-SYS | LLDP / Network | | | | Topology view validation |
| IWS - Verify daisy-chained Resense Move devices are discovered | LLDP / Network | | | | Daisy-chain discovery |
| IWS - Verify LLDP topology shows daisy-chain order | LLDP / Network | | | | Chain order in topology |
| IWS - Verify sensor data flows through daisy-chained devices | LLDP / Network | | | | Independent sensor data per device |
| IWS - Verify daisy-chain resilience when middle device is disconnected | LLDP / Network | | | | Middle device removal |
| IWS - Verify daisy-chain recovery when disconnected device is reconnected | LLDP / Network | | | | Chain recovery |
| IWS - Verify LLDP updates when daisy-chain order changes | LLDP / Network | | | | Topology update after reorder |
| IWS - Verify maximum daisy-chain depth | LLDP / Network | | | | Max chain length |
| IWS - Verify LED control works on all daisy-chained devices | LLDP / Network | | | | LED control through chain |
| IWS - Verify firmware update on daisy-chained devices | LLDP / Network | | | | Firmware update through chain |
