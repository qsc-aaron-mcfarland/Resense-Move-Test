# Detection Zones Test Cases

## IWS - Verify presence zones configuration UI available

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. Select the "Occupancy Sensor Configuration" tab.<br>3. Verify Presence Zone 1–5 controls are visible. |
| **Expected Results** | 1. A presence zones configuration section is visible.<br>2. The UI shows controls for up to 5 presence zones.<br>3. Each zone has Enabled, Name, and Presence fields matching the control pins: "Presence Zone N Enabled", "Presence Zone N Name", "Presence Zone N Presence". |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Detection Zones |

---

## IWS - Verify default detection zones

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. Select the "Occupancy Sensor Configuration" tab.<br>3. Review the default zone setup. |
| **Expected Results** | 1. A default detection zone is present covering the full sensor field of view.<br>2. The zone has a default name and configuration. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Detection Zones |

---

## IWS - Add a new detection zone

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. Select the "Occupancy Sensor Configuration" tab.<br>3. Click the <add zone> button or control.<br>4. Configure the new zone (name, boundaries). |
| **Expected Results** | 1. A new detection zone is added to the list.<br>2. The zone can be named and its boundaries configured.<br>3. The zone appears in the zones list. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Detection Zones |

---

## IWS - Remove a detection zone

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network.<br>5. At least two detection zones are configured. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. Select the "Occupancy Sensor Configuration" tab.<br>3. Select a zone to remove.<br>4. Click the <remove zone> button or control.<br>5. Confirm removal if prompted. |
| **Expected Results** | 1. The selected zone is removed from the zones list.<br>2. The remaining zones are unaffected.<br>3. Associated control pins for the removed zone are no longer available. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Detection Zones |

---

## IWS - Rename a detection zone

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network.<br>5. At least one detection zone is configured. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. Select the "Occupancy Sensor Configuration" tab.<br>3. Select a zone and change its name to "Entrance Area". |
| **Expected Results** | 1. The zone name updates to "Entrance Area" in the zones list.<br>2. Any associated control pins update to reflect the new zone name. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Detection Zones |

---

## IWS - Verify presence detection per zone

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network.<br>5. Multiple detection zones are configured. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. Select the "Occupancy Sensor Configuration" tab.<br>3. Have a person stand in the area corresponding to Zone 1 only.<br>4. Observe the presence status for each zone. |
| **Expected Results** | 1. Zone 1 shows occupied/presence detected.<br>2. Other zones show unoccupied/no presence.<br>3. The per-zone occupancy status updates correctly as the person moves between zones. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Detection Zones |

---

## IWS - Verify people count per zone

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network.<br>5. Multiple detection zones are configured. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. Select the "Occupancy Sensor Configuration" tab.<br>3. Have a known number of people in the area corresponding to a specific zone.<br>4. Observe the people count for that zone. |
| **Expected Results** | 1. The per-zone people count reflects the approximate number of people in that zone.<br>2. The count updates as people enter or leave the zone area. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Detection Zones |

---

## IWS - Verify zone-specific control pins are exposed

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network.<br>5. Multiple detection zones are configured (e.g., Zone 1, Zone 2). |
| **Steps** | 1. Select the IWS component on Center Workspace > Canvas.<br>2. Review the output control pins.<br>3. Look for zone-specific pins (e.g., "Presence Zone 1 Enabled", "Presence Zone 1 Name", "Presence Zone 1 Presence"). |
| **Expected Results** | 1. Zone-specific output control pins are exposed for each configured zone.<br>2. Each zone has Enabled, Name, and Presence pins.<br>3. Pin names follow the pattern "Presence Zone N Enabled/Name/Presence". |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Detection Zones |

---

## IWS - Verify maximum of 5 presence zones

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. Select the "Occupancy Sensor Configuration" tab.<br>3. Enable all 5 presence zones (Presence Zone 1 through Presence Zone 5).<br>4. Verify no option to add a 6th zone exists. |
| **Expected Results** | 1. All 5 presence zones can be enabled and configured.<br>2. There is no option to create additional zones beyond 5.<br>3. The control pins confirm exactly 5 zone sets (Presence Zone 1–5). |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Detection Zones |

---

## IWS - Verify detection zone boundaries do not overlap error handling

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network.<br>5. At least one detection zone is configured. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. Select the "Occupancy Sensor Configuration" tab.<br>3. Add a second zone that overlaps with the first zone boundaries. |
| **Expected Results** | 1. Either the overlap is allowed (with expected behavior documented) or the UI displays a warning/validation message about overlapping zones.<br>2. If overlapping is allowed, people in the overlap area may be counted in both zones. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Detection Zones |

---

## IWS - Verify detection zones persist after save and reopen

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. Configure multiple detection zones with custom names and boundaries. |
| **Steps** | 1. Save the design via Menu Bar > File > Save.<br>2. Close the design.<br>3. Reopen the saved design.<br>4. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>5. Select the "Occupancy Sensor Configuration" tab and review zone configuration. |
| **Expected Results** | 1. All previously configured detection zones are present.<br>2. Zone names, boundaries, and settings are retained exactly as saved.<br>3. Zone-specific control pins are still exposed correctly. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Detection Zones |
