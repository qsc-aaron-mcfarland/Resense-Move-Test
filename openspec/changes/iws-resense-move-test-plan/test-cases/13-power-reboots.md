# Power Cycles, Reboots & Interruptions Test Cases

## 13.a - IWS - Verify device reaches OK state after multiple power cycles

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Design deployed to Core with an IWS component.<br>3. IWS device is on the network, inventory item name matches device name in Configurator.<br>4. IWS device is in "OK" state. |
| **Steps** | 1. Verify the IWS device is in "OK" state.<br>2. Power cycle the IWS device by disconnecting and reconnecting power.<br>3. Wait for the device to come back online and reach "OK" state.<br>4. Repeat steps 2-3 multiple times.<br>5. After the final power cycle, verify full device functionality. |
| **Expected Results** | 1. The device reaches "OK" state after each power cycle.<br>2. The device reconnects automatically without manual intervention.<br>3. Sensor data resumes flowing after each power cycle.<br>4. The device is fully functional with no degradation.<br>5. Configuration is retained across all power cycles. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Power & Reboots |

---

## 13.b - IWS - Verify device reaches OK state after multiple reboots

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Design deployed to Core with an IWS component.<br>3. IWS device is on the network, inventory item name matches device name in Configurator.<br>4. IWS device is in "OK" state. |
| **Steps** | 1. Verify the IWS device is in "OK" state.<br>2. Reboot the IWS device via QPM.<br>3. Wait for the device to come back online and reach "OK" state.<br>4. Repeat steps 2-3 multiple times.<br>5. After the final reboot, verify full device functionality. |
| **Expected Results** | 1. The device reaches "OK" state after each reboot.<br>2. The device reconnects automatically without manual intervention.<br>3. Sensor data resumes flowing after each reboot.<br>4. The device is fully functional with no degradation.<br>5. Configuration is retained across all reboots. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Power & Reboots |

---

## 13.c - IWS - Verify device recovers after Ethernet disconnection

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Design deployed to Core with an IWS component.<br>3. IWS device is on the network, inventory item name matches device name in Configurator.<br>4. IWS device is in "OK" state. |
| **Steps** | 1. Verify the IWS device is in "OK" state.<br>2. Disconnect the Ethernet cable between the Core and the IWS device.<br>3. Wait 30 seconds.<br>4. Reconnect the Ethernet cable.<br>5. Wait for the device to reach "OK" state.<br>6. Repeat steps 2-5 multiple times.<br>7. After the final reconnection, verify full device functionality. |
| **Expected Results** | 1. The device reaches "OK" state after each Ethernet reconnection.<br>2. The device reconnects automatically without manual intervention.<br>3. Sensor data resumes flowing after each reconnection.<br>4. The device is fully functional with no degradation.<br>5. No memory leaks or resource exhaustion occurs. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Power & Reboots |
