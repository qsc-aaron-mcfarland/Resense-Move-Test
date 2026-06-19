# LLDP / Network Discovery Test Cases

## 09.a - IWS - Verify LLDP information on single Resense Move

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. A single IWS (Resense Move) device is connected to the Q-SYS Core network via Ethernet.<br>5. IWS device is on the network, inventory item name matches device name in Configurator.<br>6. Deploy the design to the Core. |
| **Steps** | 1. Open QPM in a web browser and navigate to the IWS device.<br>2. Open the "Basic" network page.<br>3. Review the LLDP neighbor information. |
| **Expected Results** | 1. The device's LLDP neighbor information is visible on the Basic network page in QPM.<br>2. The upstream switch/port is correctly identified.<br>3. The LLDP data matches the physical network topology. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > LLDP / Network |

---

## 09.b - IWS - Verify single Resense Move network topology in Q-SYS

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. A single IWS (Resense Move) device is on the network, inventory item name matches device name in Configurator.<br>5. Device is connected directly to a Q-SYS Core or managed switch.<br>6. Deploy the design to the Core. |
| **Steps** | 1. Open the network topology or status view in Q-SYS Designer.<br>2. Locate the IWS device in the topology.<br>3. Verify the displayed connection path. |
| **Expected Results** | 1. The IWS device appears in the network topology.<br>2. The connection shows the correct upstream device (switch or Core).<br>3. The port number matches the physical connection. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > LLDP / Network |

---

## 09.c - IWS - Verify daisy-chained Resense Move devices are discovered

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add two or more IWS components to the canvas.<br>4. Two or more IWS (Resense Move) devices are physically daisy-chained (Device A Ethernet out → Device B Ethernet in).<br>5. Inventory item names match device names in Configurator. |
| **Steps** | 1. Open Menu Bar > Tools > Configurator.<br>2. Review the discovered devices list. |
| **Expected Results** | 1. All daisy-chained IWS devices automatically appear in Configurator.<br>2. Each device shows a unique IP address and identifier.<br>3. All devices can be individually added to the design. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > LLDP / Network |

---

## 09.d - IWS - Verify LLDP topology shows daisy-chain order

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add IWS components to the canvas for each daisy-chained device.<br>4. Two or more IWS (Resense Move) devices are daisy-chained, inventory item names match device names in Configurator.<br>5. Deploy the design to the Core. |
| **Steps** | 1. Open the network topology or status view in Q-SYS Designer, or check the Basic network page in QPM for each device.<br>2. Locate the daisy-chained IWS devices in the topology.<br>3. Verify the displayed chain order. |
| **Expected Results** | 1. The topology correctly shows the daisy-chain order (Core/switch → Device A → Device B → ...).<br>2. Each device shows its upstream and downstream LLDP neighbor.<br>3. The first device in the chain shows the switch/Core as its upstream neighbor. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > LLDP / Network |

---

## 09.e - IWS - Verify sensor data flows through daisy-chained devices

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add IWS components for each daisy-chained device.<br>4. Two or more IWS (Resense Move) devices are daisy-chained, inventory item names match device names in Configurator.<br>5. Deploy the design to the Core. |
| **Steps** | 1. Double-click each IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. On the Status tab, verify sensor data is present in the Sensor Output section for each device.<br>3. Introduce an environmental change near each device and observe updates. |
| **Expected Results** | 1. Each daisy-chained device independently reports its own sensor data.<br>2. Sensor values update in near real-time for all devices in the chain.<br>3. No data loss or cross-contamination between daisy-chained devices. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > LLDP / Network |

---

## 09.f - IWS - Verify daisy-chain resilience when middle device is disconnected

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add IWS components for three daisy-chained devices (A → B → C).<br>4. All three devices are on the network, inventory item names match device names in Configurator.<br>5. Deploy the design to the Core and verify all devices are connected. |
| **Steps** | 1. Verify all three devices are reporting sensor data.<br>2. Disconnect Device B (middle device) from the chain by unplugging its Ethernet cable.<br>3. Observe the status of Device A and Device C.<br>4. Observe the status of Device B. |
| **Expected Results** | 1. Device A (upstream of the disconnection) continues to report sensor data normally.<br>2. Device C (downstream of the disconnection) loses connectivity and shows a fault/disconnected state.<br>3. Device B shows a fault/disconnected state.<br>4. No crash or unhandled error occurs in Q-SYS Designer. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > LLDP / Network |

---

## 09.g - IWS - Verify daisy-chain recovery when disconnected device is reconnected

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Three IWS (Resense Move) devices are daisy-chained (A → B → C).<br>4. Device B was previously disconnected, causing Device C to also lose connectivity. |
| **Steps** | 1. Reconnect Device B to the daisy-chain.<br>2. Wait for the devices to re-establish connection.<br>3. Observe the status of all three devices. |
| **Expected Results** | 1. Device B reconnects and resumes reporting sensor data.<br>2. Device C reconnects and resumes reporting sensor data.<br>3. All devices reconnect automatically without manual intervention.<br>4. The daisy-chain topology is restored correctly. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > LLDP / Network |

---

## 09.h - IWS - Verify LLDP updates when daisy-chain order changes

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Two IWS (Resense Move) devices are daisy-chained (A → B), inventory item names match device names in Configurator.<br>4. Deploy the design to the Core. |
| **Steps** | 1. Verify the current topology shows A → B order.<br>2. Physically swap the daisy-chain order to B → A.<br>3. Wait for LLDP to update the topology.<br>4. Review the network topology in Q-SYS Designer or QPM Basic network page. |
| **Expected Results** | 1. The topology updates to reflect the new B → A order.<br>2. Both devices remain functional.<br>3. Sensor data continues to flow for both devices. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > LLDP / Network |

---

## 09.i - IWS - Verify maximum daisy-chain depth

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. The maximum supported number of daisy-chained IWS (Resense Move) devices are connected in a chain.<br>4. Inventory item names match device names in Configurator. |
| **Steps** | 1. Deploy the design to the Core.<br>2. Verify all devices appear in Configurator.<br>3. Verify sensor data is flowing for all devices, including the last device in the chain. |
| **Expected Results** | 1. All devices in the chain are discovered and connected.<br>2. Sensor data is available for every device, including the last in the chain.<br>3. No degradation of data update frequency for downstream devices. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > LLDP / Network |

---

## 09.j - IWS - Verify LED control works on all daisy-chained devices

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Two or more IWS (Resense Move) devices are daisy-chained, inventory item names match device names in Configurator.<br>4. Deploy the design to the Core. |
| **Steps** | 1. Double-click each IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. Select the "LED Configuration" tab for each device.<br>3. Set a different LED color on each device (e.g., Device A = red, Device B = green).<br>4. Observe the physical devices. |
| **Expected Results** | 1. Each device's LED ring changes to the configured color independently.<br>2. LED commands reach all devices in the chain, including downstream devices.<br>3. No LED command interference between daisy-chained devices. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > LLDP / Network |

---

## 09.k - IWS - Verify firmware update on daisy-chained devices

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Two or more IWS (Resense Move) devices are daisy-chained, inventory item names match device names in Configurator.<br>4. The devices are running an older firmware version than what the Core provides. |
| **Steps** | 1. Deploy the design to the Core, triggering the automatic firmware update on all daisy-chained devices.<br>2. Monitor the update progress for each device. |
| **Expected Results** | 1. Firmware update completes successfully on all daisy-chained devices.<br>2. All devices reconnect after the update.<br>3. The daisy-chain topology is preserved after the update.<br>4. No device in the chain is bricked or left in a fault state. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > LLDP / Network |
