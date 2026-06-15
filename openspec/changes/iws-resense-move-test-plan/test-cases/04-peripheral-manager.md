# Peripheral Manager Test Cases

## IWS - Verify device appears in Peripheral Manager discovery

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. IWS device is powered on and connected to the same network as the Q-SYS Core. |
| **Steps** | 1. Open Menu Bar > Tools > Peripheral Manager (or Configurator).<br>2. Initiate device discovery / scan.<br>3. Review the discovered devices list. |
| **Expected Results** | 1. The IWS device appears in the discovered devices list.<br>2. The device shows its correct model identifier, IP address, and status.<br>3. The device is listed as "Not Commissioned" or equivalent. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Peripheral Manager |

---

## IWS - Commission a discovered IWS device

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. IWS device is discovered in Peripheral Manager but not yet commissioned. |
| **Steps** | 1. Open Peripheral Manager.<br>2. Select the discovered IWS device.<br>3. Enter the device credentials (username/password).<br>4. Click the commission/add button. |
| **Expected Results** | 1. The device status changes from "Not Commissioned" to "Connected" or "OK".<br>2. The device appears in the design inventory as an assigned peripheral.<br>3. Sensor data begins flowing to the component. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Peripheral Manager |

---

## IWS - Commission with incorrect credentials

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. IWS device is discovered in Peripheral Manager but not yet commissioned. |
| **Steps** | 1. Open Peripheral Manager.<br>2. Select the discovered IWS device.<br>3. Enter incorrect credentials (wrong username or password).<br>4. Click the commission/add button. |
| **Expected Results** | 1. A clear error message is displayed indicating authentication failure.<br>2. The device remains in "Not Commissioned" state.<br>3. No crash or unhandled exception occurs. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Peripheral Manager |

---

## IWS - Commission with empty credentials

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. IWS device is discovered in Peripheral Manager but not yet commissioned. |
| **Steps** | 1. Open Peripheral Manager.<br>2. Select the discovered IWS device.<br>3. Leave credential fields empty.<br>4. Click the commission/add button. |
| **Expected Results** | 1. A validation message indicates that credentials are required.<br>2. The device is not commissioned.<br>3. The UI does not allow proceeding without credentials. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Peripheral Manager |

---

## IWS - Decommission a commissioned device

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. IWS device is commissioned and connected. |
| **Steps** | 1. Open Peripheral Manager.<br>2. Select the commissioned IWS device.<br>3. Click the decommission/remove button.<br>4. Confirm the action if prompted. |
| **Expected Results** | 1. The device status changes to "Not Commissioned" or is removed from the assigned list.<br>2. Sensor data stops flowing to the component.<br>3. The component on the canvas shows a disconnected/unassigned state. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Peripheral Manager |

---

## IWS - Verify firmware version displayed

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. IWS device is commissioned and connected. |
| **Steps** | 1. Open Peripheral Manager.<br>2. Select the commissioned IWS device.<br>3. Locate the firmware version information. |
| **Expected Results** | 1. The current firmware version of the IWS device is displayed.<br>2. The version string is in a recognizable format. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Peripheral Manager |

---

## IWS - Firmware update when update is available

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. IWS device is commissioned and connected.<br>4. A firmware update is available for the IWS device. |
| **Steps** | 1. Open Peripheral Manager.<br>2. Select the commissioned IWS device.<br>3. Locate the firmware update option.<br>4. Initiate the firmware update.<br>5. Wait for the update to complete. |
| **Expected Results** | 1. A progress indicator shows during the firmware update.<br>2. The update completes successfully.<br>3. The firmware version updates to the new version.<br>4. The device reconnects after the update without manual intervention. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Peripheral Manager |

---

## IWS - Firmware update when device is already up to date

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. IWS device is commissioned, connected, and running the latest firmware. |
| **Steps** | 1. Open Peripheral Manager.<br>2. Select the commissioned IWS device.<br>3. Check for firmware update availability. |
| **Expected Results** | 1. The UI indicates that the device firmware is already up to date.<br>2. No update is offered or initiated. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Peripheral Manager |

---

## IWS - Verify device status indicators in Peripheral Manager

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. IWS device is commissioned and connected. |
| **Steps** | 1. Open Peripheral Manager.<br>2. Review the status column for the IWS device.<br>3. Note the status indicator (icon, color, text). |
| **Expected Results** | 1. The status indicator shows a healthy/connected state (e.g., green icon, "OK" text).<br>2. Device name, model, IP address, and firmware version are all visible. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Peripheral Manager |

---

## IWS - Verify Peripheral Manager status when device goes offline

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. IWS device is commissioned and connected. |
| **Steps** | 1. Open Peripheral Manager.<br>2. Disconnect the IWS device from the network.<br>3. Wait for the status to update.<br>4. Observe the device status. |
| **Expected Results** | 1. The device status changes to a fault/disconnected state (e.g., red icon, "Fault" or "Not Present" text).<br>2. The status update occurs within a reasonable timeout period. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Peripheral Manager |

---

## IWS - Verify Peripheral Manager status when device comes back online

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. IWS device is commissioned but currently disconnected from network. |
| **Steps** | 1. Open Peripheral Manager.<br>2. Reconnect the IWS device to the network.<br>3. Wait for the status to update.<br>4. Observe the device status. |
| **Expected Results** | 1. The device status returns to healthy/connected state.<br>2. No manual re-commissioning is required.<br>3. Sensor data resumes flowing. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Peripheral Manager |

---

## IWS - Assign IWS device to component in design

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is discovered but not assigned to any component. |
| **Steps** | 1. Open Peripheral Manager.<br>2. Select the IWS device.<br>3. Assign it to the IWS component in the design (e.g., via dropdown or drag). |
| **Expected Results** | 1. The device is assigned to the IWS component.<br>2. The component on the canvas reflects the connected state.<br>3. Sensor data begins appearing in Floating Window "Intelligent Workspace Sensor". |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Peripheral Manager |

---

## IWS - Reassign IWS device to a different component

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add two IWS components to the canvas.<br>4. IWS device is assigned to the first component. |
| **Steps** | 1. Open Peripheral Manager.<br>2. Select the IWS device currently assigned to "IWS 1".<br>3. Reassign it to "IWS 2". |
| **Expected Results** | 1. The device is removed from "IWS 1" assignment.<br>2. The device is now assigned to "IWS 2".<br>3. "IWS 1" shows unassigned/disconnected state.<br>4. "IWS 2" shows connected state and receives sensor data. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Peripheral Manager |

---

## IWS - Verify device discovery with multiple IWS devices

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Multiple IWS devices (at least 2) are powered on and connected to the network. |
| **Steps** | 1. Open Peripheral Manager.<br>2. Initiate device discovery.<br>3. Review the discovered devices list. |
| **Expected Results** | 1. All IWS devices on the network are discovered and listed.<br>2. Each device shows a unique identifier (IP address, serial number, or MAC address).<br>3. Devices can be individually selected and managed. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Peripheral Manager |

---

## IWS - Verify Peripheral Manager with device password change

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. IWS device is commissioned and connected with known credentials. |
| **Steps** | 1. Change the IWS device password via the device web interface or other management tool.<br>2. Return to Peripheral Manager in Q-SYS Designer.<br>3. Observe the device status after the password change. |
| **Expected Results** | 1. The device status changes to indicate an authentication error or fault.<br>2. A clear message indicates the credentials are no longer valid.<br>3. Re-entering the new credentials restores the connection. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Peripheral Manager |
