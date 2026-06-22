# Factory Reset Test Cases

## 12.a - IWS - Verify configuration resets to default on factory reset

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Design deployed to Core with an IWS component.<br>3. IWS device is on the network, inventory item name matches device name in Configurator.<br>4. IWS device is in "OK" state with non-default configuration applied (custom hostname, LED settings, detection zones, network settings, etc.). |
| **Steps** | 1. Perform a factory reset on the IWS device (via QPM, device web interface, or hardware button).<br>2. Wait for the device to complete the reset and reboot.<br>3. Observe the device status in the inventory.<br>4. Review all configuration values on the device. |
| **Expected Results** | 1. All configuration values return to factory defaults.<br>2. The hostname reverts to the default device name.<br>3. Network settings revert to defaults (DHCP or default static).<br>4. LED settings, detection zones, and sensor configuration revert to defaults.<br>5. The device no longer has a relationship with the Core and requires re-commissioning from scratch.<br>6. No residual custom configuration remains on the device.<br>7. The Designer component reports the device as "Missing" with no values populated from the device.<br>8. The device appears as an unpaired/unmatched device on the Q-SYS network. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Factory Reset |
