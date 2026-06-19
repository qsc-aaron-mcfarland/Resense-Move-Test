# Web UI Test Cases

## 16.a - IWS - Verify IR frame renders in Web UI

| Field | Details |
|---|---|
| **Preconditions** | 1. IWS device is on the network and accessible via IP address.<br>2. Open the device Web UI in a web browser.<br>3. Navigate to the detection zone / live view page. |
| **Steps** | 1. Observe the IR frame view area.<br>2. Verify the live thermal image is displayed within the circular lens boundary (red border indicates physical FOV edge).<br>3. Wait for the auto-refresh cycle to complete.<br>4. Verify the frame updates. |
| **Expected Results** | 1. The IR frame renders a live thermal image of the sensor's field of view.<br>2. The circular lens boundary is clearly visible (red area outside the FOV).<br>3. The frame refreshes automatically without manual intervention.<br>4. No rendering artifacts or blank frames appear. |
| **Execution Type** | Manual |
| **Section** | Web UI > IR Frame / Detection Zones |

---

## 16.b - IWS - Verify color palette switching in Web UI

| Field | Details |
|---|---|
| **Preconditions** | 1. IWS device is on the network and accessible via IP address.<br>2. Open the device Web UI in a web browser.<br>3. Navigate to the detection zone / live view page.<br>4. The IR frame is rendering with the default color palette. |
| **Steps** | 1. Click the color palette dropdown.<br>2. Select the rainbow/jet palette. Verify the IR frame updates to use the new colors.<br>3. Select the hot/yellow palette. Verify the IR frame updates.<br>4. Select the grayscale palette. Verify the IR frame updates.<br>5. Select the blue-to-red (cool-warm) palette. Verify the IR frame updates. |
| **Expected Results** | 1. Each palette option renders the IR frame with distinct, correct color mapping.<br>2. Switching palettes updates the view immediately (on next frame refresh).<br>3. Thermal intensity gradients are clearly distinguishable in each palette.<br>4. No rendering errors or fallback to a default palette on switch. |
| **Execution Type** | Manual |
| **Section** | Web UI > IR Frame / Detection Zones |

---

## 16.c - IWS - Verify color palette selection persists on page reload

| Field | Details |
|---|---|
| **Preconditions** | 1. IWS device is on the network and accessible via IP address.<br>2. Open the device Web UI in a web browser.<br>3. Navigate to the detection zone / live view page. |
| **Steps** | 1. Select a non-default color palette (e.g., grayscale).<br>2. Verify the IR frame renders with the selected palette.<br>3. Refresh the browser page (F5).<br>4. Observe the color palette selection and IR frame rendering. |
| **Expected Results** | 1. After page reload, the previously selected color palette is still active.<br>2. The IR frame renders with the persisted palette, not the default.<br>3. The dropdown shows the correct palette as selected. |
| **Execution Type** | Manual |
| **Section** | Web UI > IR Frame / Detection Zones |

---

## 16.d - IWS - Verify layout persistence for multi-sensor group

| Field | Details |
|---|---|
| **Preconditions** | 1. Two or more IWS devices are on the network, grouped together in the Web UI.<br>2. Open the Web UI for the sensor group.<br>3. A spatial layout (arrangement of sensors relative to each other) has been configured. |
| **Steps** | 1. Document the current multi-sensor layout arrangement.<br>2. Close the browser and reopen the Web UI for the sensor group.<br>3. Verify the layout is the same as documented.<br>4. Power cycle one of the sensors in the group.<br>5. Reopen the Web UI for the sensor group and verify the layout. |
| **Expected Results** | 1. The multi-sensor layout persists after closing and reopening the Web UI.<br>2. The spatial arrangement of sensors is identical to what was configured.<br>3. Power cycling a single sensor does not affect the group layout.<br>4. No sensors are displaced or missing from the layout view. |
| **Execution Type** | Manual |
| **Section** | Web UI > Multi-Sensor Layout |

---

## 16.e - IWS - Verify sensor grouping logic in Web UI

| Field | Details |
|---|---|
| **Preconditions** | 1. Two or more IWS devices are on the network and accessible.<br>2. Open the device Web UI in a web browser. |
| **Steps** | 1. Create a new group containing two or more sensors.<br>2. Verify all selected sensors appear in the group.<br>3. Remove one sensor from the group.<br>4. Verify the removed sensor is no longer part of the group.<br>5. Add the sensor back to the group.<br>6. Verify the sensor reappears in the group. |
| **Expected Results** | 1. Sensors can be grouped together in the Web UI.<br>2. The group reflects the correct membership after add/remove operations.<br>3. Grouped sensors share a combined coverage view.<br>4. Ungrouped sensors operate independently. |
| **Execution Type** | Manual |
| **Section** | Web UI > Multi-Sensor Layout |

---

## 16.f - IWS - Verify grouped sensors show combined zone coverage

| Field | Details |
|---|---|
| **Preconditions** | 1. Two or more IWS devices are grouped together in the Web UI.<br>2. Detection zones are configured on each sensor. |
| **Steps** | 1. Open the group view in the Web UI.<br>2. Verify that each sensor's detection zone is visible in the combined layout.<br>3. Verify that overlapping coverage areas between sensors are represented correctly. |
| **Expected Results** | 1. All grouped sensors' detection zones are visible in a single combined view.<br>2. The spatial relationship between sensors is accurately represented.<br>3. Overlapping zones are clearly identifiable.<br>4. Person counts from the group reflect the combined coverage. |
| **Execution Type** | Manual |
| **Section** | Web UI > Multi-Sensor Layout |
