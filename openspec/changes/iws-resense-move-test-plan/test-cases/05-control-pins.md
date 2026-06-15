# Control Pins Test Cases

## IWS - Verify all control pins are listed

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas. |
| **Steps** | 1. Select the IWS component on Center Workspace > Canvas.<br>2. Open Right Sidebar > Properties drawer.<br>3. Scroll to the "Control Pins" section.<br>4. Review the full list of pins against the pin reference (00-pin-reference.tsv). |
| **Expected Results** | 1. All documented control pins are present: CPU Temperature, Dewpoint, Framework Version, Hostname, Humidity, Identify, Kernel Version, LED Brightness, LED Color, LED Enable, LED Pattern, LED Speed, Luminosity, Model ID, Motherboard Temperature, Occupancy State, Occupancy Timeout, People Count, Poll Rate, Presence Zone 1–5 (Enabled/Name/Presence each), Sound Level, Status, System Uptime, Temperature, TVOC, Zone JSON.<br>2. No undocumented or missing pins. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Control Pins |

---

## IWS - Verify "Occupancy State" control pin value

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Select the IWS component on Center Workspace > Canvas.<br>2. Connect the "Occupancy State" output pin to a display/indicator component.<br>3. Deploy/run the design.<br>4. Observe the pin value with the space occupied and then unoccupied. |
| **Expected Results** | 1. The "Occupancy State" pin outputs a boolean or 0/1 value.<br>2. The value changes to reflect occupied vs. unoccupied state.<br>3. The value matches the occupancy shown in Floating Window "Intelligent Workspace Sensor" > Status tab > Sensor Output section. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Control Pins |

---

## IWS - Verify "People Count" control pin value

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Connect the "People Count" output pin to a display/indicator component.<br>2. Deploy/run the design.<br>3. Observe the pin value with a known number of people in the sensor field of view. |
| **Expected Results** | 1. The "People Count" pin outputs an integer value.<br>2. The value matches the people count shown in Floating Window "Intelligent Workspace Sensor" > Status tab > Sensor Output section. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Control Pins |

---

## IWS - Verify "Luminosity" control pin value

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Connect the "Luminosity" output pin to a display/indicator component.<br>2. Deploy/run the design.<br>3. Observe the pin value. |
| **Expected Results** | 1. The "Luminosity" pin outputs a numeric value in Lux (0–4,000).<br>2. The value matches the luminosity reading shown in Floating Window "Intelligent Workspace Sensor" > Status tab > Sensor Output section. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Control Pins |

---

## IWS - Verify "Temperature" control pin value

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Connect the "Temperature" output pin to a display/indicator component.<br>2. Deploy/run the design.<br>3. Observe the pin value. |
| **Expected Results** | 1. The "Temperature" pin outputs a numeric value.<br>2. The value matches the temperature reading shown in Floating Window "Intelligent Workspace Sensor" > Status tab > Sensor Output section. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Control Pins |

---

## IWS - Verify "Humidity" control pin value

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Connect the "Humidity" output pin to a display/indicator component.<br>2. Deploy/run the design.<br>3. Observe the pin value. |
| **Expected Results** | 1. The "Humidity" pin outputs a numeric percentage value.<br>2. The value matches the humidity reading shown in Floating Window "Intelligent Workspace Sensor" > Status tab > Sensor Output section. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Control Pins |

---

## IWS - Verify "Dewpoint" control pin value

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Connect the "Dewpoint" output pin to a display/indicator component.<br>2. Deploy/run the design.<br>3. Observe the pin value. |
| **Expected Results** | 1. The "Dewpoint" pin outputs a numeric temperature value.<br>2. The value is plausible given the current temperature and humidity. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Control Pins |

---

## IWS - Verify "TVOC" control pin value

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Connect the "TVOC" output pin to a display/indicator component.<br>2. Deploy/run the design.<br>3. Observe the pin value. |
| **Expected Results** | 1. The "TVOC" pin outputs a numeric value in ppm.<br>2. The value matches the TVOC reading shown in Floating Window "Intelligent Workspace Sensor" > Status tab > Sensor Output section. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Control Pins |

---

## IWS - Verify "Sound Level" control pin value

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Connect the "Sound Level" output pin to a display/indicator component.<br>2. Deploy/run the design.<br>3. Observe the pin value. |
| **Expected Results** | 1. The "Sound Level" pin outputs a numeric value in dBA.<br>2. The value matches the sound level reading shown in Floating Window "Intelligent Workspace Sensor" > Status tab > Sensor Output section. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Control Pins |

---

## IWS - Verify "Status" control pin value

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Connect the "Status" output pin to a display/indicator component.<br>2. Deploy/run the design.<br>3. Observe the pin value while device is connected.<br>4. Disconnect the IWS device from the network.<br>5. Observe the pin value after disconnection. |
| **Expected Results** | 1. The "Status" pin outputs a value indicating healthy/connected state when the device is online.<br>2. The value changes to indicate fault/disconnected state when the device goes offline. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Control Pins |

---

## IWS - Verify "Identify" control pin triggers device identification

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Select the IWS component on Center Workspace > Canvas.<br>2. Locate the "Identify" control pin.<br>3. Trigger the "Identify" pin (send a trigger/true value).<br>4. Observe the physical IWS device. |
| **Expected Results** | 1. The physical IWS device performs an identification action (e.g., LED ring flashes a distinct pattern).<br>2. The identification action is clearly visible and distinguishable from normal LED operation.<br>3. The identification stops after a period or when the pin is reset. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Control Pins |

---

## IWS - Verify "LED Brightness" control pin

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Connect a control source to the "LED Brightness" pin.<br>2. Deploy/run the design.<br>3. Send a brightness value (e.g., 50%).<br>4. Observe the physical IWS device. |
| **Expected Results** | 1. The LED ring brightness on the physical device adjusts to the specified level.<br>2. Floating Window "Intelligent Workspace Sensor" > LED Configuration tab reflects the updated brightness value. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Control Pins |

---

## IWS - Verify "LED Color" control pin

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Connect a control source to the "LED Color" pin.<br>2. Deploy/run the design.<br>3. Send a color value (e.g., green).<br>4. Observe the physical IWS device. |
| **Expected Results** | 1. The LED ring color on the physical device changes to the specified color.<br>2. Floating Window "Intelligent Workspace Sensor" > LED Configuration tab reflects the updated color value. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Control Pins |

---

## IWS - Verify "LED Enable" control pin

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network.<br>5. LED ring is currently on. |
| **Steps** | 1. Connect a control source to the "LED Enable" pin.<br>2. Deploy/run the design.<br>3. Send a false/0 value to disable the LED.<br>4. Observe the physical IWS device.<br>5. Send a true/1 value to re-enable the LED. |
| **Expected Results** | 1. Sending false/0 turns off the LED ring on the physical device.<br>2. Sending true/1 turns the LED ring back on.<br>3. Floating Window "Intelligent Workspace Sensor" > LED Configuration tab reflects the current enable/disable state. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Control Pins |

---

## IWS - Verify "LED Pattern" control pin

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Connect a control source to the "LED Pattern" pin.<br>2. Deploy/run the design.<br>3. Send different pattern values to cycle through available LED patterns.<br>4. Observe the physical IWS device for each pattern. |
| **Expected Results** | 1. The LED ring on the physical device changes pattern with each value sent.<br>2. Available patterns are visually distinct from one another.<br>3. Floating Window "Intelligent Workspace Sensor" > LED Configuration tab reflects the current pattern selection. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Control Pins |

---

## IWS - Verify "LED Speed" control pin

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network.<br>5. LED Pattern is set to an animated pattern (not solid). |
| **Steps** | 1. Connect a control source to the "LED Speed" pin.<br>2. Deploy/run the design.<br>3. Send a low speed value and observe the LED animation speed.<br>4. Send a high speed value and observe the LED animation speed. |
| **Expected Results** | 1. The LED animation speed on the physical device changes with the sent values.<br>2. Lower values produce slower animation; higher values produce faster animation (or vice versa, per documentation).<br>3. Floating Window "Intelligent Workspace Sensor" > LED Configuration tab reflects the current speed value. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Control Pins |

---

## IWS - Verify "Occupancy Timeout" control pin

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Connect a control source to the "Occupancy Timeout" pin.<br>2. Set the timeout to a known value (e.g., 30 seconds).<br>3. Deploy/run the design.<br>4. Have a person enter and then leave the sensor field of view.<br>5. Observe the "Occupancy State" pin after the person leaves. |
| **Expected Results** | 1. The "Occupancy State" pin remains true/occupied for approximately the configured timeout duration after the person leaves.<br>2. After the timeout expires, "Occupancy State" changes to false/unoccupied. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Control Pins |

---

## IWS - Verify "Poll Rate" control pin

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Connect a control source to the "Poll Rate" pin.<br>2. Set the poll rate to a specific value.<br>3. Deploy/run the design.<br>4. Observe the update frequency of sensor readings. |
| **Expected Results** | 1. The sensor data update frequency changes to match the configured poll rate.<br>2. The "Poll Rate" value is reflected in the control pin. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Control Pins |

---

## IWS - Verify device info pins display correct values

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Connect display/indicator components to the following output pins: "Hostname", "Model ID", "Framework Version", "Kernel Version", "System Uptime".<br>2. Deploy/run the design.<br>3. Observe the values. |
| **Expected Results** | 1. "Hostname" displays the device hostname string.<br>2. "Model ID" displays the IWS model identifier.<br>3. "Framework Version" displays a version string.<br>4. "Kernel Version" displays a version string.<br>5. "System Uptime" displays a time value that increments. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Control Pins |

---

## IWS - Verify "CPU Temperature" and "Motherboard Temperature" pins

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Connect display/indicator components to "CPU Temperature" and "Motherboard Temperature" output pins.<br>2. Deploy/run the design.<br>3. Observe the values. |
| **Expected Results** | 1. "CPU Temperature" displays a numeric temperature value.<br>2. "Motherboard Temperature" displays a numeric temperature value.<br>3. Both values are within plausible hardware temperature ranges. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Control Pins |

---

## IWS - Verify "Zone JSON" control pin outputs valid JSON

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network.<br>5. At least one Presence Zone is enabled. |
| **Steps** | 1. Connect the "Zone JSON" output pin to a display/text component.<br>2. Deploy/run the design.<br>3. Observe the output string. |
| **Expected Results** | 1. The "Zone JSON" pin outputs a valid JSON string.<br>2. The JSON contains zone data for all enabled presence zones.<br>3. The JSON structure includes zone names, enable states, and presence values. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Control Pins |

---

## IWS - Verify Presence Zone control pins (per zone)

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Connect display components to "Presence Zone 1 Enabled", "Presence Zone 1 Name", and "Presence Zone 1 Presence" output pins.<br>2. Deploy/run the design.<br>3. Enable Presence Zone 1 via its "Enabled" pin or configuration.<br>4. Set the zone name.<br>5. Observe presence detection in Zone 1. |
| **Expected Results** | 1. "Presence Zone 1 Enabled" reflects whether the zone is enabled (true/false).<br>2. "Presence Zone 1 Name" displays the configured zone name.<br>3. "Presence Zone 1 Presence" indicates presence detection within that zone.<br>4. The same pattern applies to Zones 2–5. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Control Pins |

---

## IWS - Verify control pin values update in real-time

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network.<br>5. All sensor output pins are connected to display components. |
| **Steps** | 1. Deploy/run the design.<br>2. Introduce an environmental change (e.g., person enters the room, lights change).<br>3. Observe the connected display components for value updates. |
| **Expected Results** | 1. All affected control pin values update in near real-time.<br>2. Pin values match the corresponding sensor readings in Floating Window "Intelligent Workspace Sensor" > Status tab > Sensor Output section. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Control Pins |

---

## IWS - Verify control pin values when device is disconnected

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected.<br>5. Sensor output pins are connected to display components. |
| **Steps** | 1. Deploy/run the design.<br>2. Disconnect the IWS device from the network.<br>3. Observe the connected display components for value changes.<br>4. Check the "Status" pin value. |
| **Expected Results** | 1. Sensor control pin values stop updating or go to a default/fault state.<br>2. The "Status" pin indicates a disconnected/fault state.<br>3. No crash or unhandled error occurs. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Control Pins |

---

## IWS - Connect control pins via wiring on canvas

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component and a Script component to the canvas. |
| **Steps** | 1. Click on the "Temperature" output pin of the IWS component.<br>2. Drag a wire to an input pin of the Script component.<br>3. Release to create the connection. |
| **Expected Results** | 1. A wire/connection line appears between the two pins on the canvas.<br>2. The connection is listed in the component's connections or wiring view.<br>3. The wire can be selected and deleted. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Control Pins |

---

## IWS - Verify control pin naming convention

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas. |
| **Steps** | 1. Select the IWS component on Center Workspace > Canvas.<br>2. Open Right Sidebar > Properties drawer.<br>3. Scroll to the "Control Pins" section.<br>4. Review all pin display names and script names. |
| **Expected Results** | 1. All pin display names are human-readable and clearly identify their function.<br>2. All script names follow the "iws_" prefix convention.<br>3. Presence Zone pins follow the pattern "Presence Zone N Enabled/Name/Presence".<br>4. No unnamed or ambiguously named pins exist. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Control Pins |
