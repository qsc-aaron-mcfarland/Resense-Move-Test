# Peripheral Manager Test Cases

## 04.a - IWS - Verify device appears in Configurator via Q-SYS Discovery

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. IWS device is powered on and connected to the same network as the Q-SYS Core. |
| **Steps** | 1. Open Menu Bar > Tools > Configurator.<br>2. Review the discovered devices list. |
| **Expected Results** | 1. The IWS device automatically appears in the Configurator device list via Q-SYS Discovery.<br>2. The device shows its correct model identifier, IP address, and status.<br>3. No manual scan or discovery initiation is required. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Configurator |

---

## 04.b - IWS - Verify device connects when inventory name matches device name

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas (creating an inventory item).<br>4. IWS device is on the network and visible in Configurator.<br>5. Secured Communications is NOT enabled on the Core. |
| **Steps** | 1. Set the IWS inventory item name to match the device name shown in Configurator.<br>2. Deploy the design to the Core (F5).<br>3. Observe the device status. |
| **Expected Results** | 1. The IWS device automatically connects to the component.<br>2. The device reaches "OK" state without any credential entry.<br>3. Sensor data begins flowing to the component. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Configurator |

---

## 04.c - IWS - Verify device does not connect when inventory name does not match

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is on the network and visible in Configurator.<br>5. Secured Communications is NOT enabled on the Core. |
| **Steps** | 1. Set the IWS inventory item name to a value that does NOT match any device name in Configurator.<br>2. Deploy the design to the Core (F5).<br>3. Observe the device status. |
| **Expected Results** | 1. The IWS component does not connect to any device.<br>2. The component shows a disconnected/unassigned state.<br>3. No sensor data flows.<br>4. No crash or unhandled error occurs. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Configurator |

---

## 04.d - IWS - Verify device connects with Secured Communications enabled

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is on the network and visible in Configurator.<br>5. Secured Communications IS enabled on the Core.<br>6. Device password has been set via QPM. |
| **Steps** | 1. Set the IWS inventory item name to match the device name in Configurator.<br>2. Deploy the design to the Core (F5).<br>3. Observe the device status. |
| **Expected Results** | 1. The IWS device connects to the component without any credential prompt in Designer.<br>2. The device reaches "OK" state.<br>3. Sensor data begins flowing to the component.<br>4. No authentication dialogs appear in Designer. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Configurator |

---

## 04.e - IWS - Verify device fails to connect with Secured Communications enabled and no password set

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is on the network and visible in Configurator.<br>5. Secured Communications IS enabled on the Core.<br>6. Device password has NOT been set via QPM. |
| **Steps** | 1. Set the IWS inventory item name to match the device name in Configurator.<br>2. Deploy the design to the Core (F5).<br>3. Observe the device status. |
| **Expected Results** | 1. The device fails to connect.<br>2. A fault status is displayed indicating the device is not trusted or not configured for secure communication.<br>3. The component does not receive sensor data.<br>4. No crash or unhandled exception occurs. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Configurator |

---

## 04.f - IWS - Verify firmware version displayed in QPM

| Field | Details |
|---|---|
| **Preconditions** | 1. Open Q-SYS Peripheral Manager (QPM) in a web browser.<br>2. IWS device is on the network and accessible.<br>3. Log in to QPM with valid credentials. |
| **Steps** | 1. Navigate to the IWS device in QPM.<br>2. Locate the firmware version information. |
| **Expected Results** | 1. The current firmware version of the IWS device is displayed.<br>2. The version string is in a recognizable format. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > QPM Management |

---

## 04.g - IWS - Verify firmware is automatically updated through the Core

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design with an IWS component.<br>3. IWS device is on the network and connected.<br>4. The IWS device is running an older firmware version than what the Core provides. |
| **Steps** | 1. Deploy the design to the Core (F5).<br>2. Observe the IWS device status during and after deployment.<br>3. Wait for the firmware update to complete. |
| **Expected Results** | 1. The Core automatically pushes the firmware update to the IWS device.<br>2. The firmware update completes without manual intervention.<br>3. The device firmware version updates to the version provided by the Core.<br>4. The device reconnects and reaches "OK" state after the update. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Firmware |

---

## 04.h - IWS - Verify no firmware update when device is already up to date

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design with an IWS component.<br>3. IWS device is on the network and connected.<br>4. The IWS device is already running the firmware version provided by the Core. |
| **Steps** | 1. Deploy the design to the Core (F5).<br>2. Observe the IWS device status during and after deployment. |
| **Expected Results** | 1. No firmware update is initiated.<br>2. The device reaches "OK" state without a reboot or update cycle.<br>3. The device connects in the normal expected timeframe. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Firmware |

---

## 04.i - IWS - Verify device status indicators across Designer, Configurator, and QPM

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design with an IWS component.<br>3. IWS device is on the network, name matches inventory item.<br>4. Design is deployed to the Core and device is connected. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. Select the Status tab and review the device status.<br>3. Open Menu Bar > Tools > Configurator and locate the IWS device.<br>4. Open QPM in a web browser, navigate to the IWS device, and review the status at the top of the page. |
| **Expected Results** | 1. The component Status tab shows device is connected and healthy.<br>2. In Configurator, the IWS device shows a green box indicating the device is running normally and reachable (able to communicate with device and available to add to a design if not already in use).<br>3. In QPM, the top of the page displays "Status:" with a healthy/connected state.<br>4. Device name, model, and IP address are visible in each location. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Status |

---

## 04.j - IWS - Verify device status when device goes offline

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Design deployed to Core with an IWS component.<br>3. IWS device is connected and in "OK" state. |
| **Steps** | 1. Verify the IWS device is in "OK" state on the component Status tab.<br>2. Disconnect the IWS device from the network (unplug Ethernet).<br>3. Wait for the status to update.<br>4. Check the component Status tab in Designer.<br>5. Check Configurator for the device.<br>6. Attempt to access the device in QPM via its IP address. |
| **Expected Results** | 1. The component Status tab shows a fault/disconnected state.<br>2. In Configurator, the IWS device no longer appears (device not visible when offline).<br>3. QPM does not load for the device (web interface unreachable since it is accessed via IP).<br>4. The status update occurs within a reasonable timeout period. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Status |

---

## 04.k - IWS - Verify device status when device comes back online

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Design deployed to Core with an IWS component.<br>3. IWS device was previously connected but is currently disconnected from network. |
| **Steps** | 1. Verify the IWS device shows a fault/disconnected state.<br>2. Reconnect the IWS device to the network (plug in Ethernet).<br>3. Wait for the status to update.<br>4. Check the component Status tab in Designer.<br>5. Check the device in Configurator.<br>6. Check the device in QPM. |
| **Expected Results** | 1. The component Status tab returns to a healthy/connected state ("OK").<br>2. In Configurator, the green box reappears indicating the device is reachable and running normally.<br>3. In QPM, the "Status:" field reflects the device is back online.<br>4. Sensor data resumes flowing without manual intervention. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Status |

---

## 04.n - IWS - Verify multiple IWS devices appear in Configurator

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Multiple IWS devices (at least 2) are powered on and connected to the same network as the Q-SYS Core. |
| **Steps** | 1. Open Menu Bar > Tools > Configurator.<br>2. Review the discovered devices list. |
| **Expected Results** | 1. All IWS devices on the network automatically appear in Configurator.<br>2. Each device shows a unique identifier (name, IP address, serial number, or MAC address).<br>3. Devices can be individually selected. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Configurator |
