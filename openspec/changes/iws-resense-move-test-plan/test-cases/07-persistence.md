# Persistence Test Cases

## 07.a - IWS - Verify component properties persist after save and reopen

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. Rename the component to "Lobby Sensor".<br>5. Modify additional properties (e.g., temperature unit to °F). |
| **Steps** | 1. Save the design via Menu Bar > File > Save.<br>2. Close the design.<br>3. Reopen the saved design.<br>4. Select the IWS component on Center Workspace > Canvas.<br>5. Open Right Sidebar > Properties drawer. |
| **Expected Results** | 1. The component name is "Lobby Sensor".<br>2. All modified property values are retained exactly as saved.<br>3. No properties have reverted to defaults. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Persistence |

---

## 07.b - IWS - Verify LED configuration persists after save and reopen

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network.<br>5. Configure the LED ring to a specific color (e.g., blue) and brightness (e.g., 75%). |
| **Steps** | 1. Save the design via Menu Bar > File > Save.<br>2. Close the design.<br>3. Reopen the saved design.<br>4. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>5. Select the "LED Configuration" tab and review the LED configuration values. |
| **Expected Results** | 1. The LED color is still set to blue.<br>2. The LED brightness is still set to 75%.<br>3. The physical device LED ring matches the saved configuration after design is redeployed. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Persistence |

---

## 07.c - IWS - Verify control pin wiring persists after save and reopen

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component and a Script component to the canvas.<br>4. Wire at least three output pins from IWS to the Script component. |
| **Steps** | 1. Save the design via Menu Bar > File > Save.<br>2. Close the design.<br>3. Reopen the saved design.<br>4. Review the wiring on Center Workspace > Canvas. |
| **Expected Results** | 1. All wire connections between the IWS and Script components are intact.<br>2. The correct pins are connected as originally configured.<br>3. No broken or missing connections. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Persistence |

---

## 07.d - IWS - Verify Peripheral Manager assignment persists after save and reopen

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. Commission and assign an IWS device to the component via Peripheral Manager. |
| **Steps** | 1. Save the design via Menu Bar > File > Save.<br>2. Close the design.<br>3. Reopen the saved design.<br>4. Open Peripheral Manager.<br>5. Review the device assignment for the IWS component. |
| **Expected Results** | 1. The IWS device is still assigned to the IWS component.<br>2. The device connection status is correct (connected if device is still on network).<br>3. No re-commissioning is required. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Persistence |

---

## 07.e - IWS - Verify design with IWS component can be saved as a new file

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas with full configuration (name, LED settings, zones, wiring). |
| **Steps** | 1. Save the design via Menu Bar > File > Save As.<br>2. Choose a different file name and location.<br>3. Close the design.<br>4. Open the newly saved file.<br>5. Review all IWS component configuration. |
| **Expected Results** | 1. The new file opens successfully.<br>2. All IWS component configuration is preserved in the new file.<br>3. The original file remains unchanged. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Persistence |

---

## 07.f - IWS - Verify multiple IWS components persist independently

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add three IWS components to the canvas.<br>4. Configure each with unique names, LED settings, and detection zones. |
| **Steps** | 1. Save the design via Menu Bar > File > Save.<br>2. Close the design.<br>3. Reopen the saved design.<br>4. Review each IWS component's configuration individually. |
| **Expected Results** | 1. Each of the three IWS components retains its unique configuration.<br>2. Component names, LED settings, and detection zones are independent and correct.<br>3. No cross-contamination of settings between components. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Persistence |
