# Firmware Interruption Test Cases

## 15.a - IWS - Verify device recovers from interrupted firmware update (power loss)

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Design deployed to Core with an IWS component.<br>3. IWS device is on the network, inventory item name matches device name in Configurator.<br>4. The IWS device is running an older firmware version than what the Core provides. |
| **Steps** | 1. Deploy a design with a newer firmware version to the Core, triggering the automatic firmware update on the IWS device.<br>2. While the firmware update is in progress (approximately 50% complete), disconnect power from the IWS device.<br>3. Wait 10 seconds.<br>4. Reconnect power to the IWS device.<br>5. Wait for the device to boot.<br>6. Observe the device status and behavior. |
| **Expected Results** | 1. The device does not brick (become permanently non-functional).<br>2. The device boots into either its previous firmware version or a recovery mode.<br>3. The device is discoverable on the network after power restoration.<br>4. A firmware update can be reattempted and completed successfully.<br>5. After a successful firmware update, the device reaches "OK" state. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Firmware Interruption |
