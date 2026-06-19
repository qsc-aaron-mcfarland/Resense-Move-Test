# Deployment Persistence Test Cases

## 07.g - IWS - Verify LED configuration persists through deploy cycle

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design with an IWS component.<br>3. IWS device is on the network, inventory item name matches device name in Configurator.<br>4. Configure the LED ring to color blue, brightness 50%. |
| **Steps** | 1. Deploy the design to the Core (F5).<br>2. Verify the LED configuration is active on the device.<br>3. Disconnect from the Core (F7).<br>4. Emulate the design (F6).<br>5. Change the LED ring to color red, brightness 100%.<br>6. Disconnect from emulation (F7).<br>7. Deploy the design to the Core again (F5).<br>8. Verify the LED configuration on the device. |
| **Expected Results** | 1. After step 8, the LED ring is set to red at 100% brightness.<br>2. The values match those set in emulation (step 5), not the original values (step 4).<br>3. The physical device LED ring reflects the updated configuration. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Deployment Persistence |

---

## 07.h - IWS - Verify detection zone settings persist through deploy cycle

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design with an IWS component.<br>3. IWS device is on the network, inventory item name matches device name in Configurator.<br>4. Deploy the design to the Core (F5).<br>5. Configure detection zone sensitivity to 50% and range to Medium via the device Web UI. |
| **Steps** | 1. Verify detection zone settings are active on the device.<br>2. Open the device Web UI and change detection zone sensitivity to 80% and range to High.<br>3. Disconnect from the Core (F7).<br>4. Deploy the design to the Core again (F5).<br>5. Verify detection zone settings on the device. |
| **Expected Results** | 1. After step 5, sensitivity is 80% and range is High.<br>2. The values match those set in the Web UI (step 2), not the original values.<br>3. Design deployment does not overwrite detection zone settings configured via the device Web UI. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Deployment Persistence |

---

## 07.i - IWS - Verify component properties persist through deploy cycle

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design with an IWS component.<br>3. IWS device is on the network, inventory item name matches device name in Configurator.<br>4. Set component name to "Lobby Sensor" and temperature unit to °C. |
| **Steps** | 1. Deploy the design to the Core (F5).<br>2. Verify component properties are active.<br>3. Disconnect from the Core (F7).<br>4. Emulate the design (F6).<br>5. Change the component name to "Conference Room" and temperature unit to °F.<br>6. Disconnect from emulation (F7).<br>7. Deploy the design to the Core again (F5).<br>8. Verify component properties. |
| **Expected Results** | 1. After step 8, the component name is "Conference Room" and temperature unit is °F.<br>2. The values match those set in emulation (step 5), not the original values (step 4).<br>3. The deployed design reflects all updated properties. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Deployment Persistence |
