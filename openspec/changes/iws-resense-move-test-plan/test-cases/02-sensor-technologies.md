# Sensor Technologies Test Cases

## IWS - Verify occupancy detection status displays

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. On the Status tab, in the Sensor Output section, locate the Occupancy field.<br>3. Observe the occupancy value with the space occupied by at least one person. |
| **Expected Results** | 1. The occupancy indicator shows a boolean occupied/unoccupied state.<br>2. The value updates in near real-time as the space becomes occupied or unoccupied. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Sensor Technologies |

---

## IWS - Verify people count displays correctly

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. On the Status tab, in the Sensor Output section, locate the People Count field.<br>3. Observe the count with a known number of people in the sensor field of view. |
| **Expected Results** | 1. The people count displays as an integer value.<br>2. The count reflects the approximate number of people detected by the thermal sensor.<br>3. The value updates in near real-time. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Sensor Technologies |

---

## IWS - Verify people count with zero occupants

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network.<br>5. The sensor field of view is empty (no people present). |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. On the Status tab, in the Sensor Output section, observe the People Count value. |
| **Expected Results** | 1. The people count displays 0.<br>2. The occupancy status shows unoccupied. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Sensor Technologies |

---

## IWS - Verify luminosity sensor value and unit

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. On the Status tab, in the Sensor Output section, locate the Luminosity field.<br>3. Observe the displayed value and unit. |
| **Expected Results** | 1. The luminosity value displays in Lux.<br>2. The value is within the range of 0–4,000 Lux.<br>3. The unit label "Lux" is shown. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Sensor Technologies |

---

## IWS - Verify luminosity sensor boundary at 0 Lux

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network.<br>5. The sensor is in a completely dark environment (cover the light sensor). |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. On the Status tab, in the Sensor Output section, observe the Luminosity reading. |
| **Expected Results** | 1. The luminosity value displays 0 Lux (or near 0).<br>2. No negative values are displayed. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Sensor Technologies |

---

## IWS - Verify luminosity sensor boundary at max Lux

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network.<br>5. The sensor is exposed to bright light exceeding 4,000 Lux. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. On the Status tab, in the Sensor Output section, observe the Luminosity reading. |
| **Expected Results** | 1. The luminosity value caps at 4,000 Lux or displays a maximum indicator.<br>2. No values above the documented maximum are shown. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Sensor Technologies |

---

## IWS - Verify temperature sensor value in Celsius

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. On the Status tab, in the Sensor Output section, locate the Temperature field.<br>3. Verify the unit is displayed as °C. |
| **Expected Results** | 1. The temperature value displays with the °C unit.<br>2. The value is within the operational range (+5°C to +35°C).<br>3. The reading is plausible for the current environment. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Sensor Technologies |

---

## IWS - Verify temperature sensor value in Fahrenheit

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. On the Status tab, in the Sensor Output section, locate the Temperature field.<br>3. Change the temperature unit to °F (if unit toggle is available in properties or Floating Window). |
| **Expected Results** | 1. The temperature value displays with the °F unit.<br>2. The value is the correct Fahrenheit equivalent of the Celsius reading.<br>3. The unit label updates to "°F". |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Sensor Technologies |

---

## IWS - Verify humidity sensor value and unit

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. On the Status tab, in the Sensor Output section, locate the Humidity field.<br>3. Observe the displayed value and unit. |
| **Expected Results** | 1. The humidity value displays as a percentage (%).<br>2. The value is within a plausible range (0–100%).<br>3. The unit label "%" is shown. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Sensor Technologies |

---

## IWS - Verify TVOC sensor value and unit

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. On the Status tab, in the Sensor Output section, locate the TVOC field.<br>3. Observe the displayed value and unit. |
| **Expected Results** | 1. The TVOC value displays in ppm (parts per million).<br>2. The value is a non-negative number.<br>3. The unit label "ppm" is shown. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Sensor Technologies |

---

## IWS - Verify sound level sensor value and unit

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. On the Status tab, in the Sensor Output section, locate the Sound Level field.<br>3. Observe the displayed value and unit. |
| **Expected Results** | 1. The sound level value displays in dBA.<br>2. The value is a non-negative number.<br>3. The unit label "dBA" is shown. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Sensor Technologies |

---

## IWS - Verify all sensor values update in near real-time

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. On the Status tab, in the Sensor Output section, observe all sensor readings (Occupancy, People Count, Luminosity, temperature, humidity, TVOC, sound level).<br>3. Introduce a change in the environment (e.g., turn lights on/off, enter/exit the room, make noise).<br>4. Observe sensor values for updates. |
| **Expected Results** | 1. All affected sensor values update within a few seconds of the environmental change.<br>2. No sensor reading is frozen or displaying stale data. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Sensor Technologies |

---

## IWS - Verify sensor values when device is disconnected

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device was previously commissioned and connected. |
| **Steps** | 1. Disconnect the IWS device from the network (unplug Ethernet cable).<br>2. Observe Floating Window "Intelligent Workspace Sensor" > Status tab > Sensor Output section readings.<br>3. Observe the component status on Center Workspace > Canvas. |
| **Expected Results** | 1. Sensor values stop updating or display a "no data" / fault indicator.<br>2. The component status on the canvas changes to indicate disconnected/fault state.<br>3. No crash or UI hang occurs. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Sensor Technologies |

---

## IWS - Verify sensor values restore after reconnection

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device was previously commissioned, then disconnected. |
| **Steps** | 1. Reconnect the IWS device to the network (plug Ethernet cable back in).<br>2. Wait for the device to re-establish connection.<br>3. Observe Floating Window "Intelligent Workspace Sensor" > Status tab > Sensor Output section readings.<br>4. Observe the component status on the canvas. |
| **Expected Results** | 1. Sensor values resume updating with live data.<br>2. The component status returns to normal/connected state.<br>3. No manual intervention is required to restore data flow. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Sensor Technologies |

---

## IWS - Verify dewpoint sensor value

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. On the Status tab, in the Sensor Output section, locate the Dewpoint field.<br>3. Observe the displayed value. |
| **Expected Results** | 1. The dewpoint value displays as a numeric temperature value.<br>2. The value is plausible given the current temperature and humidity readings.<br>3. The unit matches the configured temperature unit (°C or °F). |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Sensor Technologies |

---

## IWS - Verify all sensor types are listed

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. On the Status tab, review the Sensor Output section. |
| **Expected Results** | 1. All sensor types are present: Occupancy State, People Count, Luminosity, Temperature, Dewpoint, Humidity, TVOC, Sound Level.<br>2. Each sensor type has its correct unit label.<br>3. No sensor types are missing. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Sensor Technologies |

---

## IWS - Verify sensor data with multiple IWS devices

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add two IWS components to the canvas.<br>4. Both IWS devices are commissioned and connected on the network. |
| **Steps** | 1. Double-click the first IWS component to open Floating Window "Intelligent Workspace Sensor" for IWS 1.<br>2. Double-click the second IWS component to open Floating Window "Intelligent Workspace Sensor" for IWS 2.<br>3. Compare sensor readings between the two devices. |
| **Expected Results** | 1. Each Floating Window displays independent sensor data for its respective device.<br>2. Sensor values are not cross-contaminated between devices.<br>3. Both windows can be open simultaneously. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Sensor Technologies |

---

## IWS - Verify sensor data display in emulate mode

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. No physical IWS device is connected (emulate mode). |
| **Steps** | 1. Run the design in emulate mode.<br>2. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>3. On the Status tab, observe the Sensor Output section. |
| **Expected Results** | 1. Sensor fields are present but may show default/zero values or "N/A".<br>2. The component does not display errors for missing hardware in emulate mode.<br>3. The UI remains fully navigable. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Sensor Technologies |

---

## IWS - Verify sensor reading precision and formatting

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. On the Status tab, in the Sensor Output section, review the decimal precision of each sensor value.<br>3. Note the formatting (decimal places, rounding). |
| **Expected Results** | 1. Luminosity displays as a whole number (Lux).<br>2. Temperature displays with appropriate precision (e.g., 1 decimal place).<br>3. Humidity displays with appropriate precision.<br>4. All values are formatted consistently and are human-readable. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Sensor Technologies |
