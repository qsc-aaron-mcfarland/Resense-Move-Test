# Web UI Test Cases

## 16.a - IWS - Verify No Sensors Available state

| Field | Details |
|---|---|
| **Preconditions** | 1. Q-SYS Designer design has no IWS Sensors added.<br>2. Open the IWS Sensor Web UI. |
| **Steps** | 1. Observe the Web UI page content.<br>2. Verify the "Edit Zones" and "Multi-Sensor" tabs are visible but disabled/grayed out.<br>3. Verify the empty state message is displayed.<br>4. Attempt to click the disabled tabs. |
| **Expected Results** | 1. The page displays the message: "There are no IWS Sensors added to your design. Please add at least one to begin using this application."<br>2. A sensor icon is displayed above the message.<br>3. The "Edit Zones" and "Multi-Sensor" tabs are grayed out and non-interactive.<br>4. Cancel and Save buttons are present but no functional controls are available. |
| **Execution Type** | Manual |
| **Section** | Web UI > No Sensors Available |

---

## 16.b - IWS - Verify Default View with single sensor

| Field | Details |
|---|---|
| **Preconditions** | 1. At least one IWS device is on the network and accessible.<br>2. Open the IWS Sensor Web UI. |
| **Steps** | 1. Verify the "Single" tab is selected by default.<br>2. Verify the "Select a Sensor" dropdown is present and populated.<br>3. Observe the IR thermal frame with the People Count Zone polygon (yellow draggable handles).<br>4. Verify the sensor orientation widget (4 directional arrows) is displayed.<br>5. Verify the properties panel shows: Luminosity, Temperature, Humidity, Dew Point, Sound Level, TVOC, People Count, Occupancy.<br>6. Verify the "Edit" button is visible (blue, top-right).<br>7. Verify zoom controls (zoom in, zoom out, reset view) and fullscreen button are at the bottom. |
| **Expected Results** | 1. The Single tab is active with the sensor selected in the dropdown.<br>2. The IR thermal frame renders a live image with the People Count Zone polygon overlay and yellow draggable handles.<br>3. The orientation widget displays 4 directional arrows indicating sensor mounting direction.<br>4. The properties panel displays all sensor readings with appropriate units.<br>5. The People Count value is displayed at the top of the canvas area.<br>6. Zoom and fullscreen controls are functional at the bottom of the frame. |
| **Execution Type** | Manual |
| **Section** | Web UI > Default View |

---

## 16.c - IWS - Verify Edit Regions mode entry and settings panel

| Field | Details |
|---|---|
| **Preconditions** | 1. IWS device is on the network and accessible.<br>2. Open the IWS Sensor Web UI in Default View. |
| **Steps** | 1. Click the "Edit" button (blue, top-right).<br>2. Verify the settings panel appears on the right with: Image Refresh Rate, Orientation Icon toggle, Color Scale, People Count Zone color.<br>3. Change Image Refresh Rate using the dropdown (default: 1 second).<br>4. Click the pause/play button next to the refresh rate.<br>5. Toggle the Orientation Icon on/off.<br>6. Verify the orientation icon appears/disappears on the IR frame. |
| **Expected Results** | 1. Clicking Edit enters Edit Regions mode.<br>2. The settings panel displays all controls: Image Refresh Rate (dropdown + pause/play), Orientation Icon (toggle), Color Scale (palette selector), People Count Zone (color swatch).<br>3. Image Refresh Rate can be changed via dropdown.<br>4. Pause button stops frame refresh; play resumes it.<br>5. Orientation Icon toggle shows/hides the directional indicator on the IR frame. |
| **Execution Type** | Manual |
| **Section** | Web UI > Default View |

---

## 16.d - IWS - Verify Color Scale selection in Edit Regions

| Field | Details |
|---|---|
| **Preconditions** | 1. IWS device is on the network.<br>2. Open the IWS Sensor Web UI.<br>3. Enter Edit Regions mode. |
| **Steps** | 1. Locate the Color Scale option in the settings panel.<br>2. Click the Color Scale selector.<br>3. Verify multiple palette options are available (rainbow, grayscale, hot, etc.).<br>4. Select a different palette.<br>5. Verify the IR frame updates to use the new color mapping.<br>6. Select each available palette and verify the frame updates. |
| **Expected Results** | 1. The Color Scale selector shows multiple palette options as gradient bars.<br>2. Selecting a palette immediately updates the IR frame rendering on the next refresh.<br>3. Thermal intensity gradients are clearly distinguishable in each palette.<br>4. No rendering errors occur when switching palettes. |
| **Execution Type** | Manual |
| **Section** | Web UI > Default View |

---

## 16.e - IWS - Verify People Count Zone color picker

| Field | Details |
|---|---|
| **Preconditions** | 1. IWS device is on the network.<br>2. Open the IWS Sensor Web UI in Edit Regions mode. |
| **Steps** | 1. Click the People Count Zone color swatch in the settings panel.<br>2. Verify a full color picker opens with gradient selector, hue bar, and hex input field.<br>3. Select a new color using the gradient picker.<br>4. Verify the hex value updates.<br>5. Enter a hex value manually (e.g., #FF0000).<br>6. Click outside the color picker to close it.<br>7. Verify the People Count Zone polygon on the IR frame reflects the new color. |
| **Expected Results** | 1. The color picker opens with a gradient area, hue/saturation bar, and hex input (#000000 format with opacity %).<br>2. Selecting a color updates the hex field in real-time.<br>3. Manual hex entry is accepted and the picker updates accordingly.<br>4. The People Count Zone polygon border color on the IR frame changes to match the selected color. |
| **Execution Type** | Manual |
| **Section** | Web UI > Zone Editing |

---

## 16.f - IWS - Verify People Count Zone polygon editing

| Field | Details |
|---|---|
| **Preconditions** | 1. IWS device is on the network.<br>2. Open the IWS Sensor Web UI in Edit Regions mode. |
| **Steps** | 1. Observe the People Count Zone polygon overlaid on the IR frame (orange/yellow border with yellow handle dots).<br>2. Click and drag one of the yellow handle points.<br>3. Verify the polygon shape changes.<br>4. Drag multiple handles to reshape the zone.<br>5. Verify the zone boundary stays within the circular FOV boundary. |
| **Expected Results** | 1. The People Count Zone polygon is displayed with clearly visible yellow handle points at each vertex.<br>2. Handles are draggable and the polygon reshapes in real-time.<br>3. The polygon defines the area used for people counting.<br>4. The circular FOV boundary (orange border) indicates the physical sensor coverage area. |
| **Execution Type** | Manual |
| **Section** | Web UI > Zone Editing |

---

## 16.g - IWS - Verify Presence Zone add and remove

| Field | Details |
|---|---|
| **Preconditions** | 1. IWS device is on the network.<br>2. Open the IWS Sensor Web UI in Edit Regions mode.<br>3. People Count Zone is configured. |
| **Steps** | 1. In the left panel, locate "Presence Zones" section.<br>2. Click "+ Add Presence Zone".<br>3. Verify a new rectangular presence zone appears on the IR frame.<br>4. Verify "Presence Zone 1" appears in the zone list with X/Y coordinates.<br>5. Add additional presence zones (up to 5 total).<br>6. Verify each zone appears as a distinct colored rectangle on the frame.<br>7. Remove a presence zone by clicking its delete/remove control.<br>8. Verify the zone disappears from both the list and the IR frame. |
| **Expected Results** | 1. Clicking "+ Add Presence Zone" creates a new rectangular zone overlay on the IR frame.<br>2. Each presence zone is listed with its name and X/Y position values.<br>3. Up to 5 presence zones can be added (Presence Zone 1 through 5).<br>4. Each zone renders as a distinct colored rectangle on the thermal frame.<br>5. Zones can be removed, updating both the list and the visual overlay. |
| **Execution Type** | Manual |
| **Section** | Web UI > Zone Editing |

---

## 16.h - IWS - Verify Presence Zone maximum limit (5 zones)

| Field | Details |
|---|---|
| **Preconditions** | 1. IWS device is on the network.<br>2. Open the IWS Sensor Web UI in Edit Regions mode. |
| **Steps** | 1. Add presence zones one at a time until 5 zones exist.<br>2. Verify all 5 zones are listed (Presence Zone 1-5) with X/Y values.<br>3. Verify all 5 zones are visible as colored rectangles on the IR frame.<br>4. Attempt to add a 6th presence zone.<br>5. Verify the UI prevents adding more than 5 zones or the "+ Add Presence Zone" link is no longer available. |
| **Expected Results** | 1. Five presence zones can be created, each with a unique color and listed individually.<br>2. All 5 zones render simultaneously on the IR frame without overlapping labels.<br>3. The UI enforces a maximum of 5 presence zones.<br>4. The "+ Add Presence Zone" option is disabled or hidden when the limit is reached. |
| **Execution Type** | Manual |
| **Section** | Web UI > Zone Editing |

---

## 16.i - IWS - Verify No Presence Regions warning state

| Field | Details |
|---|---|
| **Preconditions** | 1. IWS device is on the network.<br>2. Open the IWS Sensor Web UI in Edit Regions mode.<br>3. No presence zones are configured. |
| **Steps** | 1. Observe the Presence Zones section in the left panel.<br>2. Verify an informational message is displayed indicating no presence regions are configured.<br>3. Verify the "+ Add Presence Zone" link is visible and clickable.<br>4. Click "+ Add Presence Zone" to dismiss the warning state. |
| **Expected Results** | 1. When no presence zones exist, an info/warning message is displayed.<br>2. The "+ Add Presence Zone" link is prominently available.<br>3. Adding a presence zone transitions the UI out of the warning state to show the zone list. |
| **Execution Type** | Manual |
| **Section** | Web UI > Zone Editing |

---

## 16.j - IWS - Verify Region Outside Zone validation

| Field | Details |
|---|---|
| **Preconditions** | 1. IWS device is on the network.<br>2. Open the IWS Sensor Web UI in Edit Regions mode.<br>3. At least one presence zone is configured. |
| **Steps** | 1. Drag a presence zone rectangle partially or fully outside the People Count Zone polygon boundary.<br>2. Observe the visual feedback on the IR frame.<br>3. Verify the zone area outside the FOV boundary is indicated (red/pink region). |
| **Expected Results** | 1. The UI provides visual feedback when a presence zone is positioned outside the valid detection area.<br>2. The region outside the FOV boundary is clearly indicated with a distinct color (red/pink area).<br>3. The user is informed that zones outside the boundary may not produce valid detection data. |
| **Execution Type** | Manual |
| **Section** | Web UI > Zone Editing |

---

## 16.k - IWS - Verify Reset Zones confirmation dialog

| Field | Details |
|---|---|
| **Preconditions** | 1. IWS device is on the network.<br>2. Open the IWS Sensor Web UI in Edit Regions mode.<br>3. At least one zone (People Count or Presence) is configured. |
| **Steps** | 1. Locate and click the "Reset" button.<br>2. Verify a confirmation dialog appears with a warning message.<br>3. Verify the dialog has Cancel and Reset (destructive) action buttons.<br>4. Click Cancel and verify zones are unchanged.<br>5. Click Reset again and confirm the action.<br>6. Verify all zones are reset to default positions. |
| **Expected Results** | 1. Clicking Reset displays a confirmation dialog: "Reset Zones" with a warning about resetting zone configuration.<br>2. The dialog has a clearly labeled destructive Reset button.<br>3. Canceling the dialog preserves existing zone configuration.<br>4. Confirming the reset restores zones to their default positions/configuration. |
| **Execution Type** | Manual |
| **Section** | Web UI > Zone Editing |

---

## 16.l - IWS - Verify Image Background Noise toggle

| Field | Details |
|---|---|
| **Preconditions** | 1. IWS device is on the network.<br>2. Open the IWS Sensor Web UI in Edit Regions mode. |
| **Steps** | 1. Locate the "Image Background Noise" toggle in the settings panel.<br>2. Toggle the setting ON.<br>3. Observe the IR frame rendering.<br>4. Toggle the setting OFF.<br>5. Compare the frame rendering with the setting on vs. off. |
| **Expected Results** | 1. The Image Background Noise toggle is accessible in the settings panel.<br>2. Enabling the toggle applies background noise filtering to the thermal image.<br>3. Disabling the toggle shows the unfiltered thermal image.<br>4. The change is reflected on the next frame refresh. |
| **Execution Type** | Manual |
| **Section** | Web UI > Zone Editing |

---

## 16.m - IWS - Verify Dark Mode toggle

| Field | Details |
|---|---|
| **Preconditions** | 1. IWS device is on the network.<br>2. Open the IWS Sensor Web UI in Edit Regions mode. |
| **Steps** | 1. Locate the "Dark Mode" toggle in the settings panel.<br>2. Toggle Dark Mode ON.<br>3. Observe the UI appearance changes.<br>4. Toggle Dark Mode OFF.<br>5. Verify the UI returns to the light theme. |
| **Expected Results** | 1. Enabling Dark Mode changes the UI theme/appearance.<br>2. Disabling Dark Mode restores the default light theme.<br>3. The toggle state is clearly indicated (on/off). |
| **Execution Type** | Manual |
| **Section** | Web UI > Zone Editing |

---

## 16.n - IWS - Verify Multi-Sensor view with sensor group

| Field | Details |
|---|---|
| **Preconditions** | 1. Two or more IWS devices are on the network and grouped.<br>2. Open the IWS Sensor Web UI. |
| **Steps** | 1. Click the "Multiple" tab.<br>2. Verify the "Sensors" panel appears with "Select a Sensor Group" dropdown.<br>3. Select a sensor group (e.g., "IWS Sensor Group 1").<br>4. Verify all sensors in the group are listed (Sensor 01, 02, 03, 04) with individual people count values.<br>5. Verify the canvas shows all sensor IR frames arranged in a grid layout.<br>6. Verify the aggregate People Count is displayed at the top. |
| **Expected Results** | 1. The Multiple tab shows the multi-sensor view.<br>2. The sensor group dropdown lists available groups.<br>3. All sensors in the selected group are listed with their names and per-sensor people count.<br>4. The canvas displays all sensor IR frames in a default grid arrangement.<br>5. The total People Count at the top is the sum of all individual sensor counts. |
| **Execution Type** | Manual |
| **Section** | Web UI > Orientation & Relationship |

---

## 16.o - IWS - Verify sensor arrangement drag and positioning

| Field | Details |
|---|---|
| **Preconditions** | 1. Two or more IWS devices are grouped.<br>2. Open the IWS Sensor Web UI in Multiple tab.<br>3. Click Edit to enter edit mode. |
| **Steps** | 1. Verify Cancel and Save buttons appear (top-right).<br>2. Click and drag a sensor on the canvas to a new position.<br>3. Verify the sensor moves freely on the canvas.<br>4. Observe the properties bar at the bottom updates the Position X/Y values.<br>5. Arrange multiple sensors in a custom layout (not grid).<br>6. Click Save.<br>7. Reload the page and verify the arrangement persists. |
| **Expected Results** | 1. In edit mode, sensors can be dragged freely on the canvas.<br>2. The properties bar updates Position X and Y values in real-time as sensors are moved.<br>3. Sensors can be arranged in any custom spatial layout.<br>4. Clicking Save persists the arrangement.<br>5. The layout persists after page reload. |
| **Execution Type** | Manual |
| **Section** | Web UI > Orientation & Relationship |

---

## 16.p - IWS - Verify sensor rotation, scale, and opacity controls

| Field | Details |
|---|---|
| **Preconditions** | 1. Two or more IWS devices are grouped.<br>2. Open the IWS Sensor Web UI in Multiple tab, Edit mode. |
| **Steps** | 1. Select a sensor on the canvas or in the sensor list.<br>2. In the properties bar, change the Rotation value (degrees).<br>3. Verify the sensor rotates on the canvas.<br>4. Change the Scale value (%).<br>5. Verify the sensor scales on the canvas.<br>6. Change the Opacity value (%).<br>7. Verify the sensor opacity changes on the canvas.<br>8. Click Save and verify all changes persist. |
| **Expected Results** | 1. The properties bar shows Name, Group, Position (X/Y), Rotation (deg), Scale (%), and Opacity (%) for the selected sensor.<br>2. Rotation rotates the sensor view on the canvas by the specified degrees.<br>3. Scale increases/decreases the sensor view size proportionally.<br>4. Opacity changes the transparency of the sensor view on the canvas.<br>5. All property changes persist after Save. |
| **Execution Type** | Manual |
| **Section** | Web UI > Orientation & Relationship |

---

## 16.q - IWS - Verify Reset Multi Sensor Canvas

| Field | Details |
|---|---|
| **Preconditions** | 1. Two or more IWS devices are grouped.<br>2. Sensors have been arranged in a custom layout (non-default positions).<br>3. Open the IWS Sensor Web UI in Multiple tab. |
| **Steps** | 1. Click the "Reset" button at the bottom of the canvas.<br>2. Verify a confirmation dialog appears: "Reset Multi Sensor Canvas - Are you sure you want to reset the position, scale, and rotation of all the groups?"<br>3. Verify the message mentions fitting/resizing all sensors to the canvas.<br>4. Click Cancel and verify nothing changes.<br>5. Click Reset to confirm.<br>6. Verify all sensors return to default grid positions with default rotation, scale, and opacity. |
| **Expected Results** | 1. The Reset confirmation dialog warns about resetting position, scale, and rotation for all sensors in the group.<br>2. Canceling preserves the current arrangement.<br>3. Confirming the reset restores all sensors to their default grid layout with 100% scale, 0 rotation, and 100% opacity. |
| **Execution Type** | Manual |
| **Section** | Web UI > Orientation & Relationship |

---

## 16.r - IWS - Verify multi-sensor layout persistence

| Field | Details |
|---|---|
| **Preconditions** | 1. Two or more IWS devices are grouped with a custom arrangement saved.<br>2. Open the IWS Sensor Web UI in Multiple tab. |
| **Steps** | 1. Document the current sensor arrangement (positions, rotations, scales).<br>2. Close the browser and reopen the Web UI.<br>3. Navigate to the Multiple tab and select the same sensor group.<br>4. Verify the arrangement matches what was documented.<br>5. Power cycle one sensor in the group.<br>6. Reopen the Web UI and verify the layout. |
| **Expected Results** | 1. The multi-sensor layout persists after closing and reopening the Web UI.<br>2. The spatial arrangement is identical to what was saved.<br>3. Power cycling a single sensor does not affect the group layout.<br>4. All position, rotation, scale, and opacity values are preserved. |
| **Execution Type** | Manual |
| **Section** | Web UI > Orientation & Relationship |

---

## 16.s - IWS - Verify sensor grouping in Multi-Sensor view

| Field | Details |
|---|---|
| **Preconditions** | 1. Two or more IWS devices are on the network.<br>2. Open the IWS Sensor Web UI. |
| **Steps** | 1. Navigate to the Multiple tab.<br>2. Use the "Select a Sensor Group" dropdown to view available groups.<br>3. Select a group and verify all member sensors are listed.<br>4. Verify each sensor shows its individual people count.<br>5. Verify the canvas renders all group members. |
| **Expected Results** | 1. The sensor group dropdown lists all configured groups.<br>2. Selecting a group populates the sensor list with all member devices.<br>3. Each sensor displays its individual people count (colored icon + number).<br>4. The canvas shows all group member sensor frames. |
| **Execution Type** | Manual |
| **Section** | Web UI > Orientation & Relationship |

---

## 16.t - IWS - Verify Disabled State for offline sensors

| Field | Details |
|---|---|
| **Preconditions** | 1. Two or more IWS devices are grouped.<br>2. At least one sensor in the group is powered off or disconnected from the network.<br>3. Open the IWS Sensor Web UI in Multiple tab. |
| **Steps** | 1. Observe the warning banner at the top of the canvas area.<br>2. Verify the message reads: "Some of your sensors are offline. Connect them to see the thermal images from the device."<br>3. Identify the offline sensor(s) on the canvas.<br>4. Verify offline sensors render as gray placeholders with the orange FOV boundary but no thermal image.<br>5. Verify online sensors continue showing live thermal data.<br>6. Verify the People Count still aggregates from available (online) sensors.<br>7. Verify the sensor list still shows all sensors with their counts (offline sensors show 0). |
| **Expected Results** | 1. A warning banner is displayed indicating some sensors are offline.<br>2. Offline sensors appear as gray placeholder images with the FOV boundary outline visible.<br>3. Online sensors continue rendering live thermal data normally.<br>4. The total People Count reflects only data from online sensors.<br>5. The sensor list displays all sensors regardless of online status, with offline sensors showing 0 count.<br>6. Edit mode remains accessible for online sensors. |
| **Execution Type** | Manual |
| **Section** | Web UI > Disabled State |

---

## 16.u - IWS - Verify popout card view

| Field | Details |
|---|---|
| **Preconditions** | 1. IWS device(s) on the network.<br>2. Open the IWS Sensor Web UI. |
| **Steps** | 1. Trigger the popout card view (click the popout/expand control on a sensor).<br>2. Verify the card displays the sensor or group name.<br>3. Verify the card shows sensor thumbnail(s) and People Count.<br>4. Verify the card can be dismissed/closed. |
| **Expected Results** | 1. The popout card displays a compact view of the sensor/group with thumbnail images.<br>2. The People Count is shown on the card.<br>3. The card provides a quick overview without navigating away from the current view.<br>4. The card can be closed to return to the normal view. |
| **Execution Type** | Manual |
| **Section** | Web UI > Default View |

---

## 16.v - IWS - Verify Single/Multiple tab switching

| Field | Details |
|---|---|
| **Preconditions** | 1. At least one IWS device is on the network.<br>2. Open the IWS Sensor Web UI. |
| **Steps** | 1. Verify the "Single" tab is selected by default.<br>2. Click the "Multiple" tab.<br>3. Verify the view switches to the multi-sensor canvas layout.<br>4. Click the "Single" tab.<br>5. Verify the view returns to the single-sensor view with dropdown, IR frame, and properties. |
| **Expected Results** | 1. Single tab shows the individual sensor view with Select a Sensor dropdown, IR frame, orientation widget, zone list, and properties panel.<br>2. Multiple tab shows the multi-sensor canvas with Select a Sensor Group dropdown, sensor list, and spatial arrangement.<br>3. Switching between tabs preserves the selected sensor/group state. |
| **Execution Type** | Manual |
| **Section** | Web UI > Default View |

---

## 16.w - IWS - Verify zoom and fullscreen controls

| Field | Details |
|---|---|
| **Preconditions** | 1. IWS device is on the network.<br>2. Open the IWS Sensor Web UI (Single or Multiple tab). |
| **Steps** | 1. Click the zoom in button (+magnifier icon).<br>2. Verify the canvas/IR frame zooms in.<br>3. Click the zoom out button (-magnifier icon).<br>4. Verify the canvas zooms out.<br>5. Click the reset view button.<br>6. Verify the canvas returns to default zoom level.<br>7. Click the fullscreen button.<br>8. Verify the canvas expands to fullscreen. |
| **Expected Results** | 1. Zoom in enlarges the canvas/frame view.<br>2. Zoom out reduces the canvas/frame view.<br>3. Reset view returns to the default zoom level and position.<br>4. Fullscreen expands the frame to fill the available viewport.<br>5. All zoom controls respond immediately without lag. |
| **Execution Type** | Manual |
| **Section** | Web UI > Default View |
