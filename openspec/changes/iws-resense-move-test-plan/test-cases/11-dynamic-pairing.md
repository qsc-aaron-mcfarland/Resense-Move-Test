# Dynamic Pairing Test Cases

## 11.a - IWS - Verify IWS device can be dynamically paired

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design with an IWS component.<br>3. IWS device is on the network, inventory item name matches device name in Configurator.<br>4. Deploy the design to the Core. |
| **Steps** | 1. Open the dynamic pairing interface in Core Manager or Designer.<br>2. Select the IWS device from the available devices list.<br>3. Initiate dynamic pairing.<br>4. Wait for pairing to complete.<br>5. Verify the device status. |
| **Expected Results** | 1. The IWS device is successfully paired to the component.<br>2. The device reaches "OK" state.<br>3. Sensor data flows from the device to the component. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Dynamic Pairing |

---

## 11.b - IWS - Verify IWS device can be unpaired

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Design deployed to Core with an IWS component.<br>3. IWS device is dynamically paired and in "OK" state. |
| **Steps** | 1. Open the dynamic pairing interface in Core Manager or Designer.<br>2. Select the currently paired device.<br>3. Initiate unpairing/removal.<br>4. Confirm the action if prompted.<br>5. Verify the component and device status. |
| **Expected Results** | 1. The device is successfully unpaired from the component.<br>2. The component shows an unassigned/disconnected state.<br>3. Sensor data stops flowing.<br>4. The device is available for pairing to another component. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Dynamic Pairing |

---

## 11.c - IWS - Verify behavior when two components paired to same physical device

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a design with two IWS components ("IWS-1" and "IWS-2").<br>3. IWS device is on the network, inventory item names configured.<br>4. Deploy the design to the Core.<br>5. One physical IWS device is available on the network. |
| **Steps** | 1. In Core Manager or Designer, pair "IWS-1" to the physical IWS device.<br>2. Verify "IWS-1" is in "OK" state.<br>3. Attempt to pair "IWS-2" to the same physical IWS device.<br>4. Observe the behavior. |
| **Expected Results** | 1. The system either prevents the duplicate pairing with a clear error, OR<br>2. The second pairing succeeds and the first component becomes unpaired.<br>3. No crash or undefined behavior occurs.<br>4. The final state is clearly communicated to the user. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Dynamic Pairing |

---

## 11.d - IWS - Verify pairings can be swapped between two devices

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a design with two IWS components ("IWS-1" and "IWS-2").<br>3. Two physical IWS devices are on the network ("IWS-0123" and "IWS-abcd").<br>4. Deploy the design to the Core.<br>5. "IWS-1" is paired to "IWS-0123" and "IWS-2" is paired to "IWS-abcd". |
| **Steps** | 1. Verify both pairings are active and in "OK" state.<br>2. In Core Manager or Designer, swap the pairings in a single edit: pair "IWS-1" to "IWS-abcd" and "IWS-2" to "IWS-0123".<br>3. Apply the changes.<br>4. Wait for both devices to connect. |
| **Expected Results** | 1. "IWS-1" is now paired to "IWS-abcd" and receiving its sensor data.<br>2. "IWS-2" is now paired to "IWS-0123" and receiving its sensor data.<br>3. Both devices reach "OK" state.<br>4. No orphaned or conflicting pairings remain. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Dynamic Pairing |

---

## 11.e - IWS - Verify pairing via device name (hostname)

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a design with an IWS component.<br>3. IWS device is on the network with a known hostname (e.g., "IWS-LobbyA").<br>4. Deploy the design to the Core. |
| **Steps** | 1. Open the dynamic pairing interface in Core Manager or Designer.<br>2. Select or enter the device by its hostname ("IWS-LobbyA").<br>3. Initiate dynamic pairing.<br>4. Wait for pairing to complete. |
| **Expected Results** | 1. The device is successfully paired using its hostname.<br>2. The device reaches "OK" state.<br>3. Sensor data flows correctly.<br>4. If the device IP changes, the pairing remains valid via hostname resolution. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Dynamic Pairing |

---

## 11.f - IWS - Verify pairing via switch port (LLDP port information)

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a design with an IWS component.<br>3. IWS device is connected to a managed switch with LLDP enabled.<br>4. The switch port information is known (e.g., "Switch1/Port24").<br>5. Deploy the design to the Core. |
| **Steps** | 1. Open the dynamic pairing interface in Core Manager or Designer.<br>2. Select or enter the device by its switch port / LLDP port information.<br>3. Initiate dynamic pairing.<br>4. Wait for pairing to complete. |
| **Expected Results** | 1. The device is successfully paired using LLDP port information.<br>2. The device reaches "OK" state.<br>3. Sensor data flows correctly.<br>4. If the device is replaced on the same port, the new device pairs automatically. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Dynamic Pairing |
