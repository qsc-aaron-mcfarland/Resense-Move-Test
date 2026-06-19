# Factory Reset Test Cases

## 12.a - IWS - Verify configuration resets to default on factory reset

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. IWS device is commissioned and connected.<br>3. Device has non-default configuration (custom hostname, LED settings, detection zones, network settings, etc.). |
| **Steps** | 1. Document the current non-default configuration values.<br>2. Perform a factory reset on the IWS device (via QPM, device web interface, or hardware button).<br>3. Wait for the device to complete the reset and come back online.<br>4. Review all configuration values on the device. |
| **Expected Results** | 1. All configuration values return to factory defaults.<br>2. The hostname reverts to the default.<br>3. Network settings revert to defaults (DHCP or default static).<br>4. LED settings, detection zones, and sensor configuration revert to defaults.<br>5. The device requires re-commissioning after factory reset.<br>6. No residual custom configuration remains. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Factory Reset |
