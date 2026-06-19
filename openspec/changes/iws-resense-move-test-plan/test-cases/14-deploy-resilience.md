# Deploy Resilience Test Cases

## 14.a - IWS - Verify device reaches OK state after multiple design deployments

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a design with an IWS component.<br>3. IWS device is on the network, inventory item name matches device name in Configurator. |
| **Steps** | 1. Deploy the design to the Core (F5).<br>2. Verify the IWS device reaches "OK" state.<br>3. Verify sensor data is flowing.<br>4. Disconnect from the Core (F7).<br>5. Deploy the design to the Core again (F5).<br>6. Repeat steps 2-5 multiple times.<br>7. After the final deployment, verify full device functionality. |
| **Expected Results** | 1. The IWS device reaches "OK" state on each deployment.<br>2. Sensor data flows correctly after each deployment.<br>3. The device reconnects automatically without manual intervention on each deployment.<br>4. The device is fully functional with no degradation.<br>5. No degradation in connection time or sensor responsiveness. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Deploy Resilience |
